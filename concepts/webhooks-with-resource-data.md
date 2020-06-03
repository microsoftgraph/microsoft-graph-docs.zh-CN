---
title: 设置包含资源数据的更改通知（预览版）
description: Microsoft Graph 使用 Webhook 机制将更改通知传递到客户端。 更改通知可以包括资源属性。
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 9135a50f8dfa631ed85a23a12e2a146893b9994f
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429556"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a>设置包含资源数据的更改通知（预览版）

Microsoft Graph 允许应用通过 [webhooks](webhooks.md)来订阅资源更改通知。 您现在可以将订阅设置为在 "更改通知" 中包含已更改的资源数据（如 Microsoft 团队聊天消息的内容）。 随后，应用程序可运行其业务逻辑，无需调用单独的 API 来获取更改的资源。 因此，应用程序的 API 调用更少，对于大型方案非常有用。

在更改通知中包含资源数据时，需要实现以下附加逻辑来满足数据访问和安全要求： 

- [处理](#subscription-lifecycle-notifications)特殊的订阅生命周期通知，以保持不间断的数据流。 Microsoft Graph 会及时发送生命周期通知，以要求应用程序重新授权，以确保在更改通知中包括资源数据的访问问题未发生意外的裁剪。
- [验证](#validating-the-authenticity-of-notifications)更改通知的真实性是否源自 Microsoft Graph。
- [提供](#decrypting-resource-data-from-change-notifications)公用加密密钥，并使用私钥解密通过更改通知接收的资源数据。

## <a name="resource-data-in-notification-payload"></a>通知负载中的资源数据

通常情况下，此类更改通知包括负载中的以下资源数据：

- **resourceData**属性中返回的已更改资源实例的ID和类型。
- 按照订阅中规定内容加密、在 **encryptedContent** 属性中返回的资源实例的所有属性值。
- 或者，具体取决于资源、**resourceData**属性中返回的特定属性。 若要仅获取特定属性，请使用 `$select` 参数，将其指定为订阅中的**资源**URL 的一部分。  


## <a name="supported-resources"></a>支持的资源

目前，Microsoft 团队 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) （预览版）资源支持包括资源数据的更改通知。 具体而言，可设置应用以下内容之一的订阅：

- 特定 Teams 频道中新增或已更改的消息：`/teams/{id}/channels/{id}/messages`
- 指定团队聊天中的新增或已更改消息： `/chats/{id}/messages`

**了 chatmessage**资源支持在更改通知中包含更改的实例的所有属性。 它不支持只返回指定实例属性。 

本文介绍了如何在团队频道中订阅更改邮件通知的示例，以及每个更改通知，包括已更改的**了 chatmessage**实例的完整资源数据。

## <a name="creating-a-subscription"></a>创建订阅

若要将资源数据包含在更改通知中，除了[创建订阅](webhooks.md#creating-a-subscription)时通常指定的属性外，**必须**指定下列属性：

- **includeResourceData**，应设置为 `true` 以明确请求资源数据。
- **lifecycleNotificationUrl** ，它是[生命周期通知](#subscription-lifecycle-notifications)传递到的终结点。 这可以与**notificationUrl**相同或不同。
- **encryptionCertificate**，仅包含 Microsoft Graph 用于加密资源数据的公钥。 保留相应的私钥，以[解密内容](#decrypting-resource-data-from-change-notifications)。
- **encryptionCertificateId**，是证书的自有标识符。 使用此 ID 在每个更改通知中匹配，用于解密的证书。

请注意下列事项：

- 对这两个更改通知终结点（**notificationUrl**和**lifecycleNotificationUrl**）使用相同的主机名。
- 按[此处](webhooks.md#notification-endpoint-validation)所述验证这两个终结点。 如果选择针对两个终结点使用同一 URL，将收到并响应两个验证请求。
- 无法更新（`PATCH`）现有订阅来添加**lifecycleNotificationUrl**属性。 应删除此类现有订阅，创建新订阅以包含 **lifecycleNotificationUrl** 属性。

### <a name="subscription-request-example"></a>订阅请求示例

下面的示例订阅了两种类型的通知： 

- 资源更改-Microsoft 团队中创建或更新的频道消息
- 可能影响更改通知流的订阅生命周期事件。 有关详细信息，请参阅[下一节](#subscription-lifecycle-notifications)中有关生命周期通知的详细信息。

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
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
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications"></a>订阅生命周期通知

某些事件可能会影响现有订阅中的更改通知流。 订阅生命周期通知会通知您要采取的操作以保持不中断的流。 与通知资源实例更改的资源更改通知不同，生命周期通知就是订阅本身以及生命周期中的当前状态。 

将生命周期通知传递到**lifecycleNotificationUrl**。 

本节内容：

- [质询订阅授权的生命周期通知](#lifecycle-notification-that-challenges-subscription-authorization)
- [授权质询流](#authorization-challenge-flow)
- [授权质询示例](#example-authorization-challenge)
- [授权质询响应](#responding-to-an-authorization-challenge)
- [提示](#tips)
- [经得起未来考验的代码，以处理其他类型的生命周期通知](#future-proof-your-code-to-handle-other-types-of-lifecycle-notifications)

### <a name="lifecycle-notification-that-challenges-subscription-authorization"></a>质询订阅授权的生命周期通知

一种类型的生命周期通知挑战活动订阅的授权状态。 当通知中的 **lifecycleEvent** 属性表示 `reauthorizationRequired`时，必须重新授权该订阅，以保持数据流。

当您创建长期订阅（例如，一个持续3天的订阅）时，会将通知流到**notificationUrl**中指示的位置。 但是，在任何时候，Microsoft Graph 可能要求您重新授权订阅，以证明自订阅创建起访问条件发生变化时，仍能访问资源数据。 下面是影响数据访问的更改示例：

- 租户管理员可能会吊销应用程序读取资源的权限。
- 在交互方案中，向应用程序提供身份验证令牌的用户，可能会受限于基于多种因素的动态策略，如位置、设备状态或风险评估。 例如，如果用户更改了物理位置，则该用户可能无法再访问该数据，并且应用程序无法重新授权订阅。 有关控制访问的动态策略的详细信息，请参阅 [Azure AD 条件性访问策略](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)。 

### <a name="authorization-challenge-flow"></a>授权质询流

活动的、未过期订阅的授权质询流如下所示：

1. Microsoft Graph 需要重新授权的订阅
    
    发生这种情况的原因可能随资源而异，可能随着时间推移而发生变化。 无论重新授权事件的原因，都需要对其进行响应。

2. Microsoft Graph 向 **lifecycleNotificationUrl** 发送授权质询通知

    请注意，更改通知流可能会持续一段时间，为你提供额外的响应时间。 但是，最终更改通知传递将暂停，直到您执行所需的操作。

3. 通过以下两种方式之一响应此生命周期通知：
    1. 重新授权订阅。 这不会延长订阅的到期日期。
    2. 续订订阅。 这将重新授权并延长到期日期。

    注意：两项操作都要求提供有效的身份验证令牌，类似于[新建订阅](webhooks.md#creating-a-subscription)或[到期前续订订阅](webhooks.md#renewing-a-subscription)。

4. 如果成功重新授权或续订订阅，则更改通知将继续进行。 否则，更改通知将保持暂停状态。
    
### <a name="example-authorization-challenge"></a>授权质询示例

以下是请求重新授权订阅的示例生命周期通知。 

请注意以下几点：

- "`"lifecycleEvent": "reauthorizationRequired"`" 字段将通知标识为授权质询。
- 生命周期通知不包含有关特定资源的任何信息，因为它与资源更改无关，而是订阅状态更改。
- 与更改通知类似，您可以将生命周期通知一起批处理（在**值**集合中），每个都有可能不同的**lifecycleEvent**值。 相应地处理批次中的每个生命周期通知。

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

> **注意：** 有关在传递更改通知时发送的数据的完整说明，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="responding-to-an-authorization-challenge"></a>授权质询响应

执行以下步骤来处理授权质询生命周期通知。 确认和验证生命周期通知的前两个步骤类似于[响应资源更改通知](webhooks.md#processing-the-change-notification)。

1. 通过使用对 POST 呼叫做出响应来确认收到生命周期通知 `HTTP 202 Accepted` 。
2. 验证生命周期通知的真实性。 更多详情参见[下列内容](#validating-the-authenticity-of-notifications)。
3. 确保应用程序具有执行下一步的有效的访问令牌。 

    如果正在使用一个[身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)，则库会通过重用有效的缓存令牌，或通过提示用户使用新密码再次登录，来处理此问题。 但是，获得新的令牌可能会失败，因为存取条件可能已更改，用户可能不再被允许访问资源数据。

4. 调用下列两个API中的任意一个。 如果 API 调用成功，则会恢复更改通知流。

    - 调用`/reauthorize`操作以重新批准订阅，但不延长到期日期：
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - 执行定期续订操作，以同时进行重新授权和续订：
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      续订可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户对资源的访问权限。 应用程序可能需要从用户获取新的访问令牌以成功重新授权订阅。 
      
      以后可以随时重试这些操作，例如访问条件发生变化时。 有关在发送生命周期通知之间发生的资源更改的任何通知，以及应用最终成功重新创建订阅的时间是否将丢失。 在这种情况下，应用程序应单独获取这些更改。

### <a name="tips"></a>提示

请注意下列事项：

1. 授权质询不会替代到期前续订资源更改通知的需要。 

    虽然可以选择在收到授权质询时续订订阅，但 Microsoft Graph 可能不会对所有订阅进行质询。 例如，没有任何活动且没有任何更改通知挂起传递的订阅可能无法向应用发出任何重新授权质询。 请务必在订阅到期前 [续订订阅](webhooks.md#renewing-a-subscription)。

2. 授权质询的频率可能会发生更改。

    不要对授权质询频率进行假设。 这些生命周期通知会告诉你何时采取措施，让你无需跟踪需要重新授权的订阅。 准备好每隔几分钟处理每个订阅的授权质询，极少情况下，只针对部分订阅。

### <a name="future-proof-your-code-to-handle-other-types-of-lifecycle-notifications"></a>经得起未来考验的代码，以处理其他类型的生命周期通知

应将订阅生命周期通知发布到**lifecycleNotificationUrl**指定的同一个终结点。 它们通过 **lifecycleEvent** 属性进行区分，可能包含略微不同的架构和属性，以提供它们所解决的方案。

在预测新类型的生命周期通知时实现您的代码：

1. 使用 **lifecycleEvent** 属性标识通知类型，以确定相应的响应。 例如，查找 `"lifecycleEvent": "reauthorizationRequired"` 属性标识特定事件并处理它。

1. 记录应用程序无法识别的任何生命周期事件以获取感知。

1. 订阅[Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/)，以监视有关新方案的生命周期通知的公告。

1. 查找有关新生命周期通知的相关文档，并根据需要对其实施支持。

## <a name="validating-the-authenticity-of-notifications"></a>正在验证通知的真实性

应用程序通常根据更改通知中包含的资源数据执行业务逻辑。 先验证每个更改通知的真实性是非常重要的。 否则，第三方可以使用错误更改通知欺骗您的应用程序，使其无法正确执行业务逻辑，并导致安全事件。

对于不包含资源数据的基本更改通知，仅根据[此处](webhooks.md#processing-the-change-notification)所述的**clientState**值对其进行验证。 这是可以接受的，因为可以进行后续调用受信任的 Microsoft Graph 来访问资源数据，因此，任何尝试欺骗的影响都是有限的。 

对于提供资源数据的更改通知，请在处理数据之前执行更全面的验证。

本节内容：

- [更改通知中的验证令牌](#validation-tokens-in-the-change-notification)
- [如何验证](#how-to-validate)
- [ JWT 令牌示例](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a>更改通知中的验证令牌

资源数据的更改通知包含一个附加属性**validationTokens**，其中包含由 Microsoft Graph 生成的 JWT 令牌组成的数组。 Microsoft Graph 将为每个不同的应用和在**值**数组中有项的租户对，生成单独的令牌。 请注意，更改通知可能包含使用同一**notificationUrl**订阅的各种应用和租户的项目组合。

在下面的示例中，更改通知包含同一应用程序的两个项目以及两个不同租户，因此**validationTokens**数组包含两个需要验证的令牌。

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

> **注意：** 有关在传递更改通知时发送的数据的完整说明，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection)。

### <a name="how-to-validate"></a>如何验证

如果你刚刚使用令牌验证，请参阅[令牌验证的原则](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/)获取概述。 使用 SDK，例如用于 .NET 的[Microsoft.identitymodel.dll Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/)库，或用于不同平台的第三方库。

注意以下事项： 

- 请务必始终在 `HTTP 202 Accepted` 更改通知的响应中发送状态代码。 
- 在验证更改通知之前（例如，在队列中存储更改通知以供以后处理时）或在（如果您即时处理这些更改）时执行此操作，即使验证失败也是如此。
- 接受更改通知可防止不必要的传递重试，还可防止任何潜在的恶意参与者发现它们是否通过验证或未通过验证。 您始终可以选择在接受无效的更改通知之后将其忽略。

具体而言，针对**validationTokens**集中各JWT令牌进行验证。 如果任何令牌失败，请考虑更改通知可疑并进一步调查。 

使用下列步骤验证令牌和生成令牌的应用程序：

1. 验证令牌是否未过期。

2. 验证令牌未被篡改，并且由预期机构（Microsoft Azure Active Directory）颁发：

    - 从公用配置终结点获取签名密钥：`https://login.microsoftonline.com/common/.well-known/openid-configuration`。 此配置由应用程序缓存一段时间。 请注意，由于签名密钥每日都会轮换，因此配置会经常更新。
    - 使用这些密钥验证 JWT 令牌的签名。

    不要接受任何其他机构颁发的令牌。

3. 验证口令已为订阅更改通知的应用程序颁发。

    下列步骤是 JWT 令牌库中标准验证逻辑的一部分，通常可作为单个函数调用执行。 
    - 在与应用程序ID匹配的令牌中验证“受众”。
    - 如果有多个应用收到更改通知，请务必检查是否有多个 Id。


4. **关键**：验证生成令牌的应用程序是否代表着 Microsoft Graph 更改通知的发布者。 

    - 在与 `0bf30f3b-4a52-48df-9a82-234910c4a086`期望值匹配的令牌中检查 **appid** 属性。
    - 这可确保更改通知不是由不是 Microsoft Graph 的不同应用程序发送的。


### <a name="example-jwt-token"></a>JWT 令牌示例

以下是在验证所需的 JWT 令牌中包含的属性的示例。

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

更改通知的**resourceData**属性仅包括资源实例的基本 ID 和类型信息。 **encryptedData**属性包含由 Microsoft Graph 使用订阅中所提供密钥解密的完整资源数据。 此属性还含有验证和解密所需的数值。 这样做是为了提高通过更改通知访问的客户数据的安全性。 保护私钥以确保客户数据不能被第三方解密，即使他们管理以截获原始更改通知，也是您的责任。

本节内容：

- [管理加密密钥](#managing-encryption-keys)
- [解密资源数据](#decrypting-resource-data)
- [示例：使用加密资源数据解密通知](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a>管理加密密钥

1. 使用非对称密钥对获取证书。

    - 可自行对证书进行签名，因为 Microsoft Graph 不会验证证书颁发者，并且仅将公共密钥用于加密。 
    - 使用[Azure 密钥存储库](https://docs.microsoft.com/azure/key-vault/key-vault-whatis)作为创建、轮换和安全管理证书的解决方案。 确保密钥符合下列条件：

        - 密钥必须属于类型 `RSA`
        - 密钥大小必须在2048和4096位之间。

2. 采用base64编码X.509格式导出证书，且**仅包括公钥**。 

3. 创建订阅时：

    - 使用导入证书的base64基编码内容，在**encryptionCertificate**属性中提供证书。
    - 在 **encryptionCertificateId** 属性中提供自己的标识符。 
  
        此标识符允许您将证书与接收的更改通知相匹配，并从证书存储中检索证书。 标识符最长 128 个字符。

4. 安全地管理私钥，以便更改通知处理代码可以访问私钥以解密资源数据。

#### <a name="rotating-keys"></a>轮换密钥

若要将私钥泄露的风险降至最低，请定期更改非对称密钥。 请按照以下步骤介绍一对新密钥：

1. 使用新非对称密钥对获取新证书。 将其用于创建的所有新订阅。

2. 使用新的证书密钥更新现有订阅。

    - 作为定期续订订阅的一部分执行此操作。 
    - 或者，枚举所有订阅并提供密钥。 使用[订阅修补程序操作](/graph/api/subscription-update?view=graph-rest-1.0)并更新**encryptionCertificate**和**encryptionCertificateId**属性。

3. 请记住下列事项：
    - 在一段时间内，旧证书仍可用于加密。 应用程序必须具有访问新旧证书的权限，以能够对内容进行解密。
    - 在每个更改通知中使用**encryptionCertificateId**属性，以确定要使用的正确密钥。
    - 仅当未看到旧证书引用的最近更改通知时，才放弃旧证书。

### <a name="decrypting-resource-data"></a>解密资源数据

为优化性能，Microsoft Graph 使用两步加密过程：
  - 它会生成一个使用对称密钥，并用来加密资源数据。
  - 它使用公用非对称密钥（在订阅时提供）来加密对称密钥，并将其包含在该订阅的每个更改通知中。

始终假定更改通知中的每个项目的对称密钥不同。

若要解密资源数据，您的应用程序应在每次更改通知中使用**encryptedContent**下的属性执行反向步骤：

1. 使用 **encryptionCertificateId** 属性标识要使用的证书。

2. 使用私钥初始化 RSA 加密组件（如 .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)）。

3. 解密在更改通知中的每个项目的**dataKey**属性中传递的对称密钥。

    使用适用于解密算法的最佳非对称加密填充（OAEP）。

4. 使用对称密钥计算**数据**中数值的 HMAC-SHA256 签名。
  
    将其与 **dataSignature**中的值进行比较。 如果不匹配，则假定有效负载已被篡改，并且不对其进行解密。

5. 将对称密钥与高级加密标准（AES）（例如 .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)）结合使用，解密 **数据**中的内容。

    - 将以下解密参数用于 AES 算法：

        - 填充： PKCS7
        - 密码模式： CBC
    - 通过复制用于解密的对称密钥的前16个字节来设置 "初始化向量"。

6. 解密的值是一个 JSON 字符串，表示更改通知中的资源实例。


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>示例：使用加密资源数据解密通知

下面是一个示例更改通知，其中包含通道消息中的**了 chatmessage**实例的加密属性值。 实例由 `@odata.id` 值指定。

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

> **注意：** 有关在传递更改通知时发送的数据的完整说明，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection)。


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
- [订阅资源类型](/graph/api/resources/subscription?view=graph-rest-beta)
- [获取订阅](/graph/api/subscription-get?view=graph-rest-1.0)
- [创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [更新订阅](/graph/api/subscription-update?view=graph-rest-1.0)
