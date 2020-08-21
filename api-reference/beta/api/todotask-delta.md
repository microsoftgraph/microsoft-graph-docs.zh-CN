---
title: todoTask：delta
description: 获取一组已在指定的 todoTaskList 中添加、删除或更新的 todoTask 资源。
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 56f114cc8bb24b7cfb250839a3711459cafd6104
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849894"
---
# <a name="todotask-delta"></a>todoTask：delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取一组已 [在指定的 todoTaskList](../resources/todotask.md) 中添加、删除或更新的 [todoTask 资源](../resources/todotasklist.md)。

**todoTaskList**中**todoTask**资源的**delta**函数调用与 GET 请求相似，但可通过在[state tokens](/graph/delta-query-overview)上述一次或多次调用中适当应用状态令牌来查询**todoTaskList**中的增量**更改这一点除外**。 这允许你维护和同步用户的 **todoTask** 资源的本地存储，而无需每次都从服务器中获取整个集。  

## <a name="permissions"></a>权限
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

跟踪 **todoTask 集合中的** 更改会引引一个或多个 **delta 函数** 调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。 只需预先指定所需的任何查询参数一次。 在后续请求中，只需复制并应用之前响应中的或 `nextLink` `deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 在 [针对同](/graph/delta-query-overview) 一 `deltaLink` todoTask 集合的 **上一个 delta** 函数调用的 URL 中返回的状态令牌，指示该组更改跟踪的完成状态。 将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 在 [上一](/graph/delta-query-overview) `nextLink` **个 delta 函数调用** 的 URL 中返回的状态令牌，指示同一 todoTask 集合中有进一步的更改需要跟踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 
- Delta 查询 `$select` 支持 `$top` 和 `$expand` todoTask。 
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

如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 todoTask](../resources/todotask.md) 集合对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例演示了如何执行单 **一 delta 函数** 调用，并将 **响应正文中的 todoTask** 最大数目限制为 2。

若要跟踪**todoTaskList 中 todoTask 资源的更改**，要执行一次或多次**delta**函数调用来获取上一次增量查询后的增量更改集。 **todoTask** 
 

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

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
  "value": [
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
      },
  ]
}
```

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](/graph/delta-query-overview)