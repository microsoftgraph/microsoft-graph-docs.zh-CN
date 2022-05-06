---
title: todoTask： delta
description: 获取一组已在指定 todoTaskList 中添加、删除或更新的 todoTask 资源。
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d99309243461dd5d424299b21c8bbd2532fea66a
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247271"
---
# <a name="todotask-delta"></a>todoTask： delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取一组已在指定 [todoTaskList](../resources/todotask.md) 中添加、删除或更新的 [todoTask](../resources/todotasklist.md) 资源。

**todoTaskList** 中 **对 todoTask** 资源的 **增量** 函数调用类似于 GET 请求，只是通过在其中一个或多个调用中适当应用 [状态令牌](/graph/delta-query-overview)，可以查询 **该 todoTaskList 中的 todoTask** 中的增量更改。 这样便可以维护和同步用户 **todoTask** 资源的本地存储，而无需每次从服务器提取整个集。  

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
GET /me/todo/lists/{id}/tasks/delta
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/delta
```

## <a name="query-parameters"></a>查询参数

跟踪 **todoTask** 集合中的更改会产生一轮或多次 **增量** 函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `@odata.nextLink` 或 `@odata.deltaLink` URL 的令牌部分。 只需预先指定所需的任何查询参数一次。 在后续请求中`@odata.nextLink``@odata.deltaLink`，只需复制并应用上一个响应中的 URL，因为该 URL 已包含编码的所需参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 在上一个 **增量** 函数的 URL 中`@odata.deltaLink`返回的 [状态令牌](/graph/delta-query-overview)调用同一 todoTask 集合，指示完成该轮更改跟踪。 将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `@odata.deltaLink` URL。|
| $skiptoken | string | 在上一个 **增量** 函数调用的 URL 中`@odata.nextLink`返回的 [状态令牌](/graph/delta-query-overview)，指示要在同一 todoTask 集合中跟踪进一步的更改。 |

### <a name="odata-query-parameters"></a>OData 查询参数

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 
- Delta 查询支持`$select`和 `$top``$expand` todoTask。 
- 提供对 `$filter` 和 `$orderby` 的有限支持：
  * 唯一支持的 `$filter` 表达式是 `$filter=receivedDateTime+ge+{value}` 或 `$filter=receivedDateTime+gt+{value}`。
  * 唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。 
- 不支持 `$search`。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}。可选。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [todoTask](../resources/todotask.md) 集合对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
若要跟踪自上一轮更改跟踪以来 **todoTaskList** 中 **todoTask** 资源的更改，需要进行一个或多个 **增量** 函数调用以获取一组增量更改。 以下示例演示如何开始下一轮更改跟踪，使用上一轮最后一次 **增量** 函数调用中`@odata.deltaLink`返回的 URL，其中包含一个`deltaToken`。 此 **增量** 函数调用将响应正文中的最大 **todoTask** 数限制为 2。
 

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
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
   "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
   "value":[
      {
         "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ9xQ==\"",
         "importance":"normal",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"empty task3",
         "createdDateTime":"2020-08-12T04:54:29.1925206Z",
         "lastModifiedDateTime":"2020-08-12T04:54:29.4903939Z",
         "id":"AAMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZDEwMwBGAAAAAAB5M0K0qlJySLOAgV22zPnuBwDit9FUg_L0SpeANtzxTscbAAMNmhwmAADit9FUg_L0SpeANtzxTscbAAMxlnrYAAA=",
         "body":{
            "content":"",
            "contentType":"text"
         }
      }
   ]
}
```

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](/graph/delta-query-overview)

