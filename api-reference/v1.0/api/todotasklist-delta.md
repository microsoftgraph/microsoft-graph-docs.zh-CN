---
title: todoTaskList： delta
description: 获取已添加、删除或删除的一组 todoTaskList 微软待办。
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5d9f9339178dd2f3c3d610f31c9316e9b8e71309
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60938121"
---
# <a name="todotasklist-delta"></a>todoTaskList： delta

命名空间：microsoft.graph

获取一组已在 微软待办 中添加、删除或删除的[todoTaskList](../resources/todotasklist.md)微软待办。

**todoTaskList** 的 **delta** 函数调用类似于 GET 请求，只不过通过在这些调用中的一 [](/graph/delta-query-overview)个或多个调用中正确应用状态令牌，您可以查询 **todoTaskList** 中的增量更改。 这样，您即可维护和同步用户的 **todoTaskList** 的本地存储，而无需每次从服务器获取所有 **todoTaskList。**

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Tasks.ReadWrite    |
|委派（个人 Microsoft 帐户） | Tasks.ReadWrite    |
|应用 | 不支持 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a>查询参数

跟踪 **todoTaskList** 资源中的更改将引发一组 delta函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。 只需预先指定所需的任何查询参数一次。 在后续请求中，只需复制并应用上一响应中的 或 URL，因为此 URL 已包含所需的编码 `nextLink` `deltaLink` 参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对 [同](/graph/delta-query-overview)一 `deltaLink` **todoTaskList** 集合的上一 **个 delta** 函数调用的 URL 中返回的状态令牌，指示完成这一轮更改跟踪。 将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 之前的 [delta](/graph/delta-query-overview)函数调用的 URL 中返回的状态令牌，指示同一 `nextLink` **todoTaskList** 集合中还有进一步的更改需要跟踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 

## <a name="request-headers"></a>请求头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}。可选。 |

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [todoTaskList](../resources/todotasklist.md) 集合对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例演示如何进行初始 **delta** 函数调用，将响应正文中 **todoTaskList** 的最大数目限制为 2。

若要跟踪 **todoTaskList** 中的更改，可以使用适当的状态令牌进行一次或多个 **delta** 函数调用，获取自上次 delta 查询以来的增量更改集。 

跟踪 **todoTaskList** 和跟踪列表中的 **todoTask** 资源之间的主要区别是 delta 查询请求 URL，查询响应返回 **todoTaskList** 而不是 **todoTask 集合** 。

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a>响应

如果请求成功，响应将包含一个状态令牌，其为 _skipToken_  
（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。

以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。

注意：为了提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD"
    }
  ]
}
```

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](/graph/delta-query-overview)

