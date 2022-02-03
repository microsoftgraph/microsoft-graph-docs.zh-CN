---
title: servicePrincipal： removeKey
description: 从 servicePrincipal 中删除密钥凭据
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 70fcb44414bae5f22ab42a01be52f45aa6c1b738
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344123"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal： removeKey

命名空间：microsoft.graph

从 [servicePrincipal 中删除密钥凭据](../resources/serviceprincipal.md)。 servicePrincipal 可以使用此方法和 [addKey](serviceprincipal-addkey.md) 自动滚动其过期密钥。

> [!NOTE]
> [Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) 和更新 [servicePrincipal](../api/serviceprincipal-update.md) 操作可以继续用于添加和更新具有或不带用户上下文的任何 servicePrincipal 的关键凭据。

作为此方法的请求验证的一部分，将验证拥有现有密钥的证明，然后才能执行该操作。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All、Application.ReadWrite.All、Directory.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removeKey
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供以下必需属性。

| 属性  | 类型 | 说明|
|:----------|:-----|:-----------|
| keyId     | GUID | 密码的唯一标识符。|
| proof | String | 用作现有密钥拥有证明的自签名 JWT 令牌。 必须使用 servicePrincipal 的现有有效证书之一的私钥对此 JWT 令牌进行签名。 令牌应包含以下声明：<ul><li>`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</li><li>`iss`- 颁发者需要是发出调用的 servicePrincipal 的 ID。</li><li>`nbf` -“不早于”时间。</li><li>`exp` - 过期时间应该是“不早于”+ 10 分钟。</li></ul><br>下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No content` 响应代码。

## <a name="examples"></a>示例

下面的示例展示了如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-removekey-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-removekey-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

