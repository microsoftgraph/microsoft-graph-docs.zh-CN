---
title: servicePrincipal： addKey
description: 向 servicePrincipal 添加密钥凭据。
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e354dd264633b2acb2f178106843bfa168dde710
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346639"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipal： addKey

命名空间：microsoft.graph

将密钥凭据添加到 [servicePrincipal](../resources/serviceprincipal.md)。 servicePrincipal 可以使用此方法和 [removeKey](serviceprincipal-removekey.md) 自动滚动其过期密钥。

> [!NOTE]
> [Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) 和更新 [servicePrincipal](../api/serviceprincipal-update.md) 操作可以继续用于添加和更新具有或不带用户上下文的任何 servicePrincipal 的关键凭据。

作为此方法的请求验证的一部分，将验证拥有现有密钥的证明，然后才能执行该操作。 

没有任何现有有效证书的 ServicePrincipals (即：尚未添加任何证书，或所有证书都已过期) ，将不能使用此服务操作。 [Update servicePrincipal](../api/serviceprincipal-update.md) 可用于执行更新。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All、Application.ReadWrite.All、Directory.ReadWrite.All  |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |


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
| keyCredential | [keyCredential](../resources/keycredential.md) | 要添加的新 servicePrincipal 密钥凭据。 __类型__、__用法____和密钥__ 是此用法的必需属性。 受支持的密钥类型包括：<br><ul><li>`AsymmetricX509Cert`：用法必须为 `Verify`。</li><li>`X509CertAndPassword`：用法必须为 `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | 仅需要设置应包含密钥密码的 __secretText__ 。 此属性仅对类型 为 的键是必需的 `X509CertAndPassword`。 否则，设置为 `null` 。|
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
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addKey
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
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addkey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addkey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addkey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-addkey-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-addkey-1-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
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
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addKey
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addkey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addkey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addkey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-addkey-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-addkey-2-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
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

