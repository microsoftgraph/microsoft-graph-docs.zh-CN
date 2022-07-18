---
title: directoryRole： delta
description: 获取新创建、更新或删除的目录角色，而无需对整个资源集合执行完整读取。 有关详细信息，请参阅使用 Delta 查询。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cf63fe996cb023e4aa70818d5319260d40023b19
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247124"
---
# <a name="directoryrole-delta"></a>directoryRole： delta

命名空间：microsoft.graph

获取新创建、更新或删除的目录角色，而无需对整个资源集合执行完整读取。 有关详细信息，请参阅 [使用 Delta 查询](/graph/delta-query-overview) 。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要开始跟踪更改，请发出一个请求，包括 [directoryRole](../resources/directoryrole.md) 资源上的 **增量** 函数。

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a>查询参数

跟踪更改会产生一轮或多次 **增量** 函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `@odata.nextLink` 或 `@odata.deltaLink` URL 的令牌部分。 只需预先指定所需的任何查询参数一次。 在后续请求中，可以复制并应用之前响应中返回的 `@odata.nextLink` 或 `@odata.deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 在上一个 **增量** 函数调用同一资源集合的 URL 中`@odata.deltaLink`返回的 [状态令牌](/graph/delta-query-overview)，指示完成这一轮更改跟踪。 将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `@odata.deltaLink` URL。|
| $skiptoken | string | 在上一个 **增量** 函数调用的 URL 中`@odata.nextLink`返回的 [状态令](/graph/delta-query-overview)牌，指示要在同一资源集合中跟踪进一步的更改。 |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。

- 提供对 `$filter` 的有限支持：

  - 唯一支持的 `$filter` 表达式是跟踪特定资源的更改，按其 ID：  `$filter=id+eq+{value}` 或 `$filter=id+eq+{value1}+or+id+eq+{value2}`。 可以指定的 ID 数受最大 URL 长度的限制。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 集合对象。 该响应还包括 `@odata.nextLink`URL 或 `@odata.deltaLink`URL。

- `@odata.nextLink`如果返回 URL，则会话中将检索其他数据页。 应用程序继续使用 `@odata.nextLink` URL 发出请求，直到响应中包含 `@odata.deltaLink` URL。

- `@odata.deltaLink`如果返回 URL，则不再有关于要返回的资源的现有状态的数据。 保存 `@odata.deltaLink` URL 并在下一次 **增量** 调用中应用它，了解将来对资源所做的更改。

### <a name="example"></a>示例

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryrole-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryrole-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryrole-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryrole-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryrole-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryrole-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pkXMyA5aFCIMmH1Kk1XEAnf2X-fodqXKXF03gYPQknSHRxogVsxvSq_26nhos-O2-shortened",
  "value": [
    {
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8",
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "members@delta": [
        {
          "@odata.type": "#microsoft.graph.user",
          "id": "bb165b45-151c-4cf6-9911-cd7188912848",
          "@removed": {
            "reason": "deleted"
          }
        }
      ]
    }
  ]
}
```

### <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph数据中的更改](/graph/delta-query-overview)以获取更多详细信息
- [获取用户的增量更改](/graph/delta-query-users)获取示例请求。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

