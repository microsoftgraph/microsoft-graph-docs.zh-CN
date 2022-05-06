---
title: oauth2permissiongrant： delta
description: 获取新创建、更新或删除的 oauth2permissiongrants，而无需对整个资源集合执行完整读取。
ms.localizationpriority: medium
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a145d3c3fef579d615bf5511cf993afbdf06d89e
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247089"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant： delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需对整个资源集合执行完整读取。 有关详细信息，请参阅 [使用增量查询](/graph/delta-query-overview)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|oauth2permissiongrant | .Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要开始跟踪更改，请发出一个请求，包括 **oauth2permissiongrant** 资源上的增量函数。

<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a>查询参数

跟踪更改会产生一轮或多次 **增量** 函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `@odata.nextLink` 或 `@odata.deltaLink` URL 的令牌部分。 只需预先指定任何查询参数一次。 在后续请求中 `@odata.nextLink` ，复制并应用上一响应中的或 `@odata.deltaLink` URL。 该 URL 已包含编码的参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 在上一个 **增量** 函数调用同一资源集合的 URL 中`@odata.deltaLink`返回的 [状态令牌](/graph/delta-query-overview)，指示完成这一轮更改跟踪。 在该集合的下一轮更改跟踪的第一个请求中保存并应用整个 `@odata.deltaLink` URL（包括此令牌）。|
| $skiptoken | string | 在上一个 **增量** 函数调用的 URL 中`@odata.nextLink`返回的 [状态令牌](/graph/delta-query-overview)，指示要在同一资源集合中跟踪进一步的更改。 |

### <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 **id** 属性。
- 提供对 `$filter` 的有限支持：
  * 唯一支持的 `$filter` 表达式是跟踪特定资源的更改，按其 ID：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}`。 可以指定的 ID 数受最大 URL 长度的限制。


## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者 &lt;token&gt;。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [oauth2permissiongrant](../resources/oauth2permissiongrant.md) 集合对象。 该响应还包括 `@odata.nextLink`URL 或 `@odata.deltaLink`URL。

- `@odata.nextLink`如果返回 URL，则会话中将检索其他数据页。 **oauth2permissiongrant** 继续使用 URL 发出请求，`@odata.nextLink`直到`@odata.deltaLink`响应中包含 URL。
- `@odata.deltaLink`如果返回 URL，则不再有关于要返回的资源的现有状态的数据。 保留并使用 `@odata.deltaLink` URL 了解将来对资源所做的更改。

有关详细信息，请参阅 [使用增量查询](/graph/delta-query-overview)。 有关请求的示例，请参阅 [获取用户的增量更改](/graph/delta-query-users)。

## <a name="example"></a>示例
### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/oauth2permissiongrant-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/oauth2permissiongrant-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/beta/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "expiryTime": "2017-08-13T21:41:23.3929007Z",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "startTime": "0001-01-01T00:00:00Z",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


