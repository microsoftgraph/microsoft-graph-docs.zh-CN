---
title: 更新 externalConnection
description: 更新 externalConnection 对象的属性。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7d93dfffa3b28a5ab9877046b6e38a7ad3dd6a8f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088689"
---
# <a name="update-externalconnection"></a>更新 externalConnection

命名空间：microsoft.graph.externalConnectors

更新 [externalConnection 对象](../resources/externalconnectors-externalconnection.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /external/connections/{connectionsId}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。 可更新以下属性。

| 属性      | 类型                                           | 说明 |
|:--------------|:-----------------------------------------------|:------------|
| configuration | [microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md) | 指定允许管理连接和索引连接内容的其他应用程序 ID。 |
| 说明   | String                                         | 网站中显示的连接Microsoft 365 管理中心。 |
| name          | String                                         | 要显示名称中显示的连接的Microsoft 365 管理中心。 最大长度为 128 个字符。 |


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/external/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-externalconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-externalconnection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-externalconnection-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
