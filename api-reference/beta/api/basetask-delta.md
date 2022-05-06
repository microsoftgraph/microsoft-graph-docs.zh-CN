---
title: baseTask： delta
description: 获取一组已在特定 baseTaskList 中添加、删除或更新的 baseTask 资源。
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c788b04c31b65ee46b7af0416c21bf21822b564e
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247180"
---
# <a name="basetask-delta"></a>baseTask： delta
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取一组已在特定 [baseTaskList](../resources/basetask.md) 中添加、删除或更新的 [baseTask](../resources/basetasklist.md) 资源。

**baseTaskList** 中 **baseTask** 资源的 **增量** 函数调用类似于 GET 请求，只是通过在其中一个或多个调用中适当应用 [状态令牌](/graph/delta-query-overview)，可以查询该 **baseTaskList 中的 baseTask** 中的增量更改。 这样便可以维护和同步用户 **的 baseTask** 资源的本地存储，而无需每次从服务器提取整个集。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.Read、Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.Read、Tasks.ReadWrite|
|应用|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/tasks/lists/{baseTaskListId}/tasks/delta
GET /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/delta
```

## <a name="query-parameters"></a>查询参数

跟踪 **baseTask** 集合中的更改会产生一轮或多次 **增量** 函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `@odata.nextLink` 或 `@odata.deltaLink` URL 的令牌部分。 只需预先指定所需的任何查询参数一次。 在后续请求中`@odata.nextLink``@odata.deltaLink`，只需复制并应用上一个响应中的 URL，因为该 URL 已包含编码的所需参数。

| 查询参数    | 类型 |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 在上一个 **增量** 函数调用同一 baseTask 集合的 URL 中`@odata.deltaLink`返回的 [状态令](/graph/delta-query-overview)牌，指示完成该轮更改跟踪。 将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `@odata.deltaLink` URL。|
| $skiptoken | string | 在上一个 **增量** 函数调用的 URL 中`@odata.nextLink`返回的 [状态令牌](/graph/delta-query-overview)，指示要在同一 baseTask 集合中进行进一步的更改。 |

### <a name="odata-query-parameters"></a>OData 查询参数

- Delta 查询支持`$filter``$top`以及 `$expand` **baseTask** 的查询参数。 
- 不支持 `$search`。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Prefer | string  | odata.maxpagesize={x}。可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 `200 OK` 响应代码和 [baseTask](../resources/basetask.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "basetask_delta"
}
-->
``` http
GET /me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=/tasks/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/basetask-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/basetask-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/basetask-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/basetask-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/basetask-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/basetask-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.baseTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(baseTask)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=/tasks/delta?$deltatoken=AVCnFFj2r7PtnjtkD-g_6dgDSPbEboZhaMYEytpd57pcJMrR9oGkCIjK_dyVkhNB1EQn1zcQt7YZTwCS0V5MNQo6Iy0-T0csAkLZTMlbiII.lVEHqD5xdDrH30csYKP6tEvoYa3WtFhmYLtKBSxCPpQ",
    "value": [
        {
            "@odata.type": "#microsoft.graph.task",
            "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAymRBQ==\"",
            "importance": "normal",
            "status": "notStarted",
            "displayName": "Read documentation",
            "createdDateTime": "2021-11-15T13:16:53.0831814Z",
            "lastModifiedDateTime": "2021-11-15T13:17:08.8273666Z",
            "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA",
            "body": {
                "content": "",
                "contentType": "text"
            },
            "parentList": {
                "id": "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA="
            }
        }
    ]
}
```

