---
title: 应用程序： addKey
description: 将密钥凭据添加到应用程序中。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f61f463e7071a168328781a8fbd4d990a5fdfd
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288695"
---
# <a name="application-addkey"></a>应用程序： addKey

命名空间：microsoft.graph

将密钥凭据添加到[应用程序](../resources/application.md)中。 应用程序可以使用此方法和[removeKey](application-removekey.md)来自动滚动其过期密钥。

> [!NOTE]
> [创建应用程序](../api/application-post-applications.md)和[更新应用程序](../api/application-update.md)操作可继续用于添加和更新具有或不具有用户上下文的任何应用程序的密钥凭据。

作为此方法的请求验证的一部分，在可以执行操作之前，将验证已拥有现有密钥的证明。 

没有任何现有有效证书的应用程序（尚未添加任何证书，或所有证书已过期）将无法使用此服务操作。 可以使用[更新应用程序](../api/application-update.md)操作来改为执行更新。

## <a name="permissions"></a>Permissions

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 无。  |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | 无。 |

> [!NOTE] 
> 应用程序不需要任何特定权限即可滚动其自己的键。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供以下必需属性。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
| keyCredential | [keyCredential](../resources/keycredential.md) | 要添加的新应用程序密钥凭据。 __Type__、 __usage__和__key__是此用法的必需属性。 受支持的密钥类型包括：<br><ul><li>`AsymmetricX509Cert`：使用必须为 `Verify` 。</li><li>`X509CertAndPassword`：使用必须`Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | 仅需要设置应包含密钥密码的__secretText__ 。 仅对于类型的键，此属性是必需的 `X509CertAndPassword` 。 将其设置为 `null` 其他。|
| 证明 | String | 自签名的 JWT 令牌，用作已有密钥的所有权证明。 必须使用应用程序的现有有效证书之一的私钥对此 JWT 令牌进行签名。 令牌应包含以下声明：<ul><li>`aud`-需要访问群体 `00000002-0000-0000-c000-000000000000` 。</li><li>`iss`-颁发者必须是正在进行呼叫的应用程序的__id__ 。</li><li>`nbf`-不早时间。</li><li>`exp`-过期时间应为 "nbf" + 10 分钟。</li></ul><br>下面是可用于生成此已占有令牌证明的代码[示例](/graph/application-rollkey-prooftoken)。|

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的[keyCredential](../resources/keycredential.md)对象。

## <a name="examples"></a>示例

### <a name="example-1-add-a-new-key-credential-to-an-application"></a>示例1：将新的密钥凭据添加到应用程序

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```

#### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a>示例2：为密钥添加密钥凭据和关联密码

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
