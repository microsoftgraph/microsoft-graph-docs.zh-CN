---
title: application： addKey
description: 向应用程序添加密钥凭据。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9a6dcc39a529f3f2b84070dc0e6d2a0699b988cc
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292033"
---
# <a name="application-addkey"></a>application： addKey

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向应用程序添加密钥 [凭据](../resources/application.md)。 此方法与 [removeKey](application-removekey.md)一起可用于应用程序自动滚动其过期密钥。

> [!NOTE]
> You can continue to use the [Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) application operations to add and update key credentials for any application with or without a user's context. 

作为此方法的请求验证的一部分，先验证现有密钥的拥有证明，然后才能执行该操作。 

没有现有有效证书的应用程序 (尚未添加任何证书，或者所有证书都已过期) 将无法使用此服务操作。 可改用[更新应用程序](../api/application-update.md)操作来执行更新。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 无。  |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | 无。 |

> [!NOTE]
> 应用程序不需要任何特定权限来滚动自己的密钥。 

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

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| keyCredential | [keyCredential](../resources/keycredential.md) | 要添加的新应用程序密钥凭据。 __类型____、用法____和密钥__ 是此用法的必需属性。 受支持的密钥类型包括：<br><ul><li>`AsymmetricX509Cert`：用法必须为 `Verify` 。</li><li>`X509CertAndPassword`：用法必须为 `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | 只需设置应包含密钥密码的 __secretText。__ 此属性仅对于类型键是必需的 `X509CertAndPassword` 。 设置为 `null` 其他方式。|
| proof | String | 自签名 JWT 令牌，用于证明拥有现有密钥。 此 JWT 令牌必须使用应用程序现有有效证书之一的私钥进行签名。 令牌应包含以下声明：<ul><li>`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</li><li>`iss` -颁发者必须是正在进行呼叫的应用程序的 __ID__。</li><li>`nbf` -“不早于”时间。</li><li>`exp` - 过期时间应该是“不早于”+ 10 分钟。</li></ul><br>下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和新 `200 OK` [keyCredential](../resources/keycredential.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-add-a-new-key-credential-to-an-application"></a>示例 1：向应用程序添加新密钥凭据

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a>示例 2：为密钥添加密钥凭据和关联密码

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
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
  ]
}-->



