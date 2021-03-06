---
title: servicePrincipal： addKey
description: 向 servicePrincipal 添加密钥凭据。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8f158edb52b67d70c8878ae33311c648be2dca9e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955496"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipal： addKey

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将密钥凭据添加到 [servicePrincipal](../resources/serviceprincipal.md)。 servicePrincipal 可以使用此方法和 [removeKey](serviceprincipal-removekey.md) 自动滚动其过期密钥。

> [!NOTE]
> [Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) 和更新 [servicePrincipal](../api/serviceprincipal-update.md) 操作可以继续用于添加和更新具有或不带用户上下文的任何 servicePrincipal 的关键凭据。

作为此方法的请求验证的一部分，将先验证现有密钥的证明，然后才能执行该操作。 

没有任何现有有效证书的 ServicePrincipals (即尚未添加任何证书，或者所有证书都已过期) ，将不能使用此服务操作。 [Update servicePrincipal](../api/serviceprincipal-update.md) 可用于执行更新。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 无。  |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | 无。 |

> [!NOTE]
> servicePrincipal 不需要任何特定权限来滚动自己的密钥。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addKey
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
| keyCredential | [keyCredential](../resources/keycredential.md) | 要添加的新 servicePrincipal 密钥凭据。 __type、usage__ 和 __key__ 是此用法的必需属性。  受支持的密钥类型包括：<br><ul><li>`AsymmetricX509Cert`：用法必须为 `Verify` 。</li><li>`X509CertAndPassword`：用法必须为 `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | 仅需要设置应包含密钥密码的 __secretText。__ 此属性仅对类型 为 的键是必需的 `X509CertAndPassword` 。 否则， `null` 设置为 。|
| proof | String | 用作现有密钥拥有证明的自签名 JWT 令牌。 必须使用 servicePrincipal 的现有有效证书之一的私钥对此 JWT 令牌进行签名。 令牌应包含以下声明：<ul><li>`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</li><li>`iss`- 颁发者需要是发出调用的 servicePrincipal 的 ID。</li><li>`nbf` -“不早于”时间。</li><li>`exp` - 过期时间应该是“不早于”+ 10 分钟。</li></ul><br>下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。|

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [keyCredential](../resources/keycredential.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a>示例 1：将新的密钥凭据添加到 servicePrincipal

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_1"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-1-javascript-snippets.md)]
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

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a>示例 2：为密钥添加密钥凭据和关联密码

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_2"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-2-javascript-snippets.md)]
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



