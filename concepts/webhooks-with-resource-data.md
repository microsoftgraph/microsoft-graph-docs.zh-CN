---
title: 设置包含资源数据的更改通知
description: Microsoft Graph 使用 Webhook 机制将更改通知传递到客户端。 更改通知可以包含资源属性。
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 867d192a2516a82a7ca4fbe07b6a9628285f9c25bf89c2400862e33065a8546c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54208634"
---
# <a name="set-up-change-notifications-that-include-resource-data"></a>设置包含资源数据的更改通知

Microsoft Graph 允许应用通过 [webhooks](webhooks.md)来订阅资源更改通知。 你可以设置订阅，以将更改后的资源数据（例如 Microsoft Teams 聊天消息的内容或 Microsoft Teams 状态信息）包括在更改通知中。 随后，应用程序可运行其业务逻辑，无需调用单独的 API 来获取更改的资源。 因此，应用程序的 API 调用更少，对于大型方案非常有用。

若要将资源数据作为更改通知的一部分，需要实现以下附加逻辑，来满足数据访问和安全要求： 

- [处理](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)）特殊订阅生命周期通知（预览），以保持数据的不间断流动。 Microsoft Graph 会不时发送生命周期通知，以要求应用重新授权，确保更改通知中所包含的数据不会意外发生访问问题。
- [验证](#validating-the-authenticity-of-notifications)来自 Microsoft Graph 的更改通知的真实性。
- [提供](#decrypting-resource-data-from-change-notifications)公共加密密钥并使用私钥解密通过更改通知所接收的资源数据。

## <a name="resource-data-in-notification-payload"></a>通知负载中的资源数据

通常情况下，此类更改通知包括负载中的以下资源数据：

- **resourceData** 属性中返回的已更改资源实例的ID和类型。
- 按照订阅中规定内容加密、在 **encryptedContent** 属性中返回的资源实例的所有属性值。
- 或者，具体取决于资源、**resourceData** 属性中返回的特定属性。 若要仅获取特定属性，请使用 `$select` 参数，将其指定为订阅中的 **资源** URL 的一部分。  


## <a name="supported-resources"></a>支持的资源

目前，Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) 以及 Microsoft Teams [presence](/graph/api/resources/presence)（预览）资源支持包括资源数据的更改通知。 具体而言，可设置应用以下内容之一的订阅：

- 特定 Teams 频道中新增或已更改的消息：`/teams/{id}/channels/{id}/messages`
- 整个组织（租户）中所有团队频道中的新消息或已更改消息： `/teams/getAllMessages`
- 指定团队聊天中的新增或已更改消息： `/chats/{id}/messages`
- 整个组织（租户）中所有聊天的新消息或已更改消息： `/chats/getAllMessages`
- 用户的状态信息更新：`/communications/presences/{id}`

含有更改通知中所有已更改实例属性的 **chatMessage** 和 **presence** （预览）支持。 它们不支持仅返回实例的选择性属性。 

本文介绍订阅 Teams 通道中的消息更改通知的示例，各更改通知包含已更改 **chatMessage** 实例的完整资源数据。 有关基于 **chatMessage** 的订阅的更多详细信息，请参阅 [获取聊天和频道消息的更改通知](teams-changenotifications-chatmessage.md)。

## <a name="creating-a-subscription"></a>创建订阅

若要将资源数据包含在更改通知中，除了 [创建订阅](webhooks.md#creating-a-subscription)时通常指定的属性外，**必须** 指定下列属性：

- **includeResourceData**，应设置为 `true` 以明确请求资源数据。
- **encryptionCertificate**，仅包含 Microsoft Graph 用于加密资源数据的公钥。 保留相应的私钥，以[解密内容](#decrypting-resource-data-from-change-notifications)。
- **encryptionCertificateId**，是证书的自有标识符。 使用此 ID 在各更改通知中匹配用于解密的证书。

请注意下列事项：

- 按[通知终结点验证](webhooks.md#notification-endpoint-validation)中所述，验证两个终结点。 如果选择针对两个终结点使用同一 URL，将收到并响应两个验证请求。

### <a name="subscription-request-example"></a>订阅请求示例

以下示例为订阅 Microsoft Teams 中创建或更新的频道消息。

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a>订阅响应
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications-preview"></a>订阅生命周期通知（预览）

某些事件可能会干扰现有订阅中的更改通知流。 订阅生命周期通知将通知你要采取的操作，以保持流不中断。 不同于资源更改通知（用于通知资源实例更改），生命周期通知涉及订阅自身及其在生命周期中的最新状态。 

有关如何接收和响应生命周期通知（预览）的详细信息，请参阅[减少缺失的订阅和更改通知（预览）](webhooks-lifecycle.md)

## <a name="validating-the-authenticity-of-notifications"></a>验证通知的真实性

应用通常根据更改通知中包含的资源数据运行业务逻辑。 首先验证每个更改通知的真实性非常重要。 否则，第三方可能会以错误的更改通知欺骗你的应用，使其错误地运行其业务逻辑并导致安全事件。

对于不包含资源数据的基本更改通知，只需根据 [处理更改通知](webhooks.md#processing-the-change-notification)中所述的 **clientState** 值来验证它们。 这是可以接受的，因为可以进行后续调用受信任的 Microsoft Graph 来访问资源数据，因此，任何尝试欺骗的影响都是有限的。 

对于传递资源数据的更改通知，请在处理数据之前执行更全面的验证。

本节内容：

- [更改通知中的验证令牌](#validation-tokens-in-the-change-notification)
- [如何验证](#how-to-validate)
- [ JWT 令牌示例](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a>更改通知中的验证令牌

带有资源数据的更改通知包含一个附加属性 **validationTokens**，其包含 Microsoft Graph 生成的 JWT 令牌数组。 Microsoft Graph 将为每个不同的应用和在 **值** 数组中有项的租户对，生成单独的令牌。 请记住，通知可能包含使用同一 **notificationUrl** 订阅的各种应用和租户的混合项。

在以下示例中，更改通知包含同一应用和两个不同租户的两个项目，因此 **validationTokens** 数组包含两个需要验证的令牌。

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="how-to-validate"></a>如何验证

如果你没有使用过令牌验证，请参阅[令牌验证原理](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/)以获取概述。 使用 SDK，例如用于 .NET 的 [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) 库或用于不同平台的第三方库。

注意以下事项： 

- 确保始终发送 `HTTP 202 Accepted` 状态代码作为更改通知响应的一部分。 
- 可在验证更改通知前（例如，将更改通知存储在队列中以供后续处理）或在验证更改通知后（如果即时处理了通知）进行响应，即使验证失败也是如此。
- 接受更改通知可以防止不必要的传递重试，还可以防止任何潜在的恶意行为者查明他们是否通过了验证。 接受无效的更改通知后，你始终可以选择忽略它。

具体而言，针对 **validationTokens** 集合中的各个 JWT 令牌进行验证。 如果任何令牌失败，请考虑更改通知可疑并进一步调查。 

使用下列步骤验证令牌和生成令牌的应用程序：

1. 验证令牌是否未过期。

2. 验证令牌未被篡改，并且由预期机构（Microsoft 标识平台）颁发：

    - 从公用配置终结点获取签名密钥：`https://login.microsoftonline.com/common/.well-known/openid-configuration`。 此配置由应用程序缓存一段时间。 请注意，由于签名密钥每日都会轮换，因此配置会经常更新。
    - 使用这些密钥验证 JWT 令牌的签名。

    不要接受任何其他机构颁发的令牌。

3. 验证口令已为订阅更改通知的应用程序颁发。

    下列步骤是 JWT 令牌库中标准验证逻辑的一部分，通常可作为单个函数调用执行。 
    - 在与应用程序ID匹配的令牌中验证“受众”。
    - 如果有多个应用收到更改通知，请务必检查是否有多个 ID。


4. **关键**：验证生成令牌的应用程序是否代表着 Microsoft Graph 更改通知的发布者。 

    - 在与 `0bf30f3b-4a52-48df-9a82-234910c4a086`期望值匹配的令牌中检查 **appid** 属性。
    - 这样可以确保更改通知不会由不是 Microsoft Graph 的其他应用发送的。


### <a name="example-jwt-token"></a>JWT 令牌示例

下面是验证所需的 JWT 令牌中所含属性的示例。

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a>示例：对验证令牌进行验证

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
还必须实现 `JwkKeyResolver`，这样 Java 示例才能正常运行。  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a>解密更改通知资源数据

更改通知的 **resourceData** 属性仅包含资源实例的基本 ID 和类型信息。 **encryptedData** 属性包含由 Microsoft Graph 使用订阅中所提供密钥解密的完整资源数据。 此属性还含有验证和解密所需的数值。 这样做是为了提高通过更改通知访问的客户数据的安全性。 你有责任保护私钥，以确保客户数据不能由第三方解密，即使他们设法截取原始更改通知也是如此。

本节内容：

- [管理加密密钥](#managing-encryption-keys)
- [解密资源数据](#decrypting-resource-data)
- [示例：使用加密资源数据解密通知](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a>管理加密密钥

1. 使用非对称密钥对获取证书。

    - 可自行对证书进行签名，因为 Microsoft Graph 不会验证证书颁发者，并且仅将公共密钥用于加密。 
    - 使用[Azure 密钥存储库](/azure/key-vault/key-vault-whatis)作为创建、轮换和安全管理证书的解决方案。 确保密钥符合下列条件：

        - 密钥必须属于类型 `RSA`
        - 密钥大小必须在2048和4096位之间。

2. 采用base64编码X.509格式导出证书，且 **仅包括公钥**。 

3. 创建订阅时：

    - 使用导入证书的base64基编码内容，在 **encryptionCertificate** 属性中提供证书。
    - 在 **encryptionCertificateId** 属性中提供自己的标识符。 
  
        此标识符能够将你的证书与接收的更改通知匹配，并从证书存储中检索证书。标识符最长 128 个字符。

4. 安全地管理私钥，以便更改通知处理代码可以访问私钥来解密资源数据。

#### <a name="rotating-keys"></a>轮换密钥

若要将私钥泄露的风险降至最低，请定期更改非对称密钥。 请按照以下步骤介绍一对新密钥：

1. 使用新非对称密钥对获取新证书。 将其用于创建的所有新订阅。

2. 使用新的证书密钥更新现有订阅。

    - 作为定期续订订阅的一部分执行此操作。 
    - 或者，枚举所有订阅并提供密钥。 使用 [订阅修补程序操作](/graph/api/subscription-update)并更新 **encryptionCertificate** 和 **encryptionCertificateId** 属性。

3. 请记住下列事项：
    - 在一段时间内，旧证书仍可用于加密。 应用程序必须具有访问新旧证书的权限，以能够对内容进行解密。
    - 使用各更改通知中的 **encryptionCertificateId** 属性来确定要使用的正确密钥。
    - 只有在没有看到最近任何更改通知引用旧证书时，才可以丢弃旧证书。

### <a name="decrypting-resource-data"></a>解密资源数据

为优化性能，Microsoft Graph 使用两步加密过程：
  - 它会生成一个使用对称密钥，并用来加密资源数据。
  - 它使用公共非对称密钥（订阅时提供）加密对称密钥，并将之包含在订阅的各更改通知中。

始终假设更改通知中各项的对称密钥不同。

若要对资源数据进行解密，应用应使用各更改通知 **encryptedContent** 下的属性执行反向操作：

1. 使用 **encryptionCertificateId** 属性标识要使用的证书。

2. 使用私钥初始化 RSA 加密组件（如 .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)）。

3. 解密更改通知中各项的 **dataKey** 属性中提供的对称密钥。

    使用适用于解密算法的最佳非对称加密填充（OAEP）。

4. 使用对称密钥计算 **数据** 中数值的 HMAC-SHA256 签名。
  
    将其与 **dataSignature** 中的值进行比较。 如果不匹配，则假定有效负载已被篡改，并且不对其进行解密。

5. 将对称密钥与高级加密标准（AES）（例如 .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)）结合使用，解密 **数据** 中的内容。

    - 将以下解密参数用于 AES 算法：

        - 填充： PKCS7
        - 密码模式： CBC
    - 通过复制用于解密的对称密钥的前16个字节来设置 "初始化向量"。

6. 解密值是一个 JSON 字符串，表示更改通知中的资源实例。


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>示例：使用加密资源数据解密通知

下面是一个示例更改通知，其中包含频道消息中 **chatMessage** 实例的解密属性值。 实例由 `@odata.id` 值指定。

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

> **注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。


本节包含一些有用的代码片段，它们针对解密的各个阶段使用C# 和NET。

#### <a name="decrypt-the-symmetric-key"></a>解密对称密钥

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a>使用 HMAC-SHA256 比较数据签名

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a>解密资源数据内容

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a>另请参阅

- [设置用户数据更改的通知](webhooks.md)
- [订阅资源类型](/graph/api/resources/subscription)
- [获取订阅](/graph/api/subscription-get)
- [创建订阅](/graph/api/subscription-post-subscriptions)
- [更新订阅](/graph/api/subscription-update)
