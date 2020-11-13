---
title: 'chatMessages: delta'
description: 检索团队频道中的消息列表（无回复）。可以通过使用 delta 查询获取频道中的新消息或更新消息。
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: b02032e06929a20f9835bed9249b68b2cada2b8e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000656"
---
# <a name="chatmessages-delta"></a>chatMessages: delta

命名空间：microsoft.graph

检索[团队](../resources/channel.md)[频道](../resources/team.md)中的[消息](../resources/chatmessage.md)列表（无回复）。可以通过使用 delta 查询获取频道中的新消息或更新消息。

> **注意：** Delta 将近返回过去 8 个月内的消息。可以使用 [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) 检索更早的消息。

Delta 查询既支持可检索指定频道中所有消息的完全同步，也支持可检索自上次同步后频道中添加或更改的消息的增量同步。通常情况下，开始时会执行一次完全同步，然后会定期获取相应日历视图的增量更改。

若要获取消息的回复，请使用[列出消息回复](channel-get-messagereply.md)或[获取消息回复](channel-list-messagereplies.md)操作。

使用 delta 函数的 GET 请求返回以下任一内容：

- `nextLink`（包含具有 **delta** 函数调用和 `skipToken` 的 URL），或
- `deltaLink`（包含具有 **delta** 函数调用和 `deltaToken` 的 URL）。

状态令牌对客户端完全不透明。若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 delta 函数调用即可。响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `deltaLink` URL，并在开始下一轮时使用。

有关详细信息，请参阅 [delta 查询](/graph/delta-query-overview)文档。

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference.md)。

|权限类型                        |权限（从最低特权到最高特权）  |
|---------------------------------------|---------------------------------------------|
|委派（工作或学校帐户）| ChannelMessage.Read.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

> **注意** ：标有 * 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。

> [!NOTE]
> 在使用应用程序权限调用此 API 之前，你必须先请求访问权限。有关详细信息，请参阅 [Microsoft Teams 中受保护的 API](/graph/teams-protected-apis)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a>查询参数

跟踪频道消息中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。

只需预先指定任何查询参数一次。

在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| `$deltatoken` | 字符串 | 之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| `$skiptoken` | 字符串 | 上一个 **delta** 函数调用中的 `nextLink` URL 返回的 [状态令牌](/graph/delta-query-overview)，指示需要跟踪进一步的更改。 |

### <a name="optional-odata-query-parameters"></a>OData 可选查询参数

此 API 支持以下[ OData 查询参数](/graph/query-parameters)：
- `$top`，表示在调用中获取的最大消息数。上限为 **50** 。
- `$skip`，表示列表开头要跳过的消息数。
- `$filter` 允许返回满足特定条件的消息。支持筛选的唯一属性为 `lastModifiedDateTime`，并且仅支持 **gt** 运算符。例如，`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` 将获取在指定日期/时间后创建或更高的所有消息。

## <a name="request-headers"></a>请求标头
| 标头        | 值                     |
|---------------|---------------------------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json          |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。响应还包括 `nextLink` URL 或 `deltaLink` URL。

## <a name="examples"></a>示例

### <a name="example-1-initial-synchronization"></a>示例 1：初始同步

以下示例显示了用于同步给定频道中消息的三个请求。频道中有 5 个消息。

- 第 1 步：[示例第一个请求](#initial-request)和[响应](#initial-request-response)。
- 第 2 步：[示例第二个请求](#second-request)和[响应](#second-request-response)
- 第 3 步：[示例第三个请求](#third-request)和[最终响应](#third-request-response)。

为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。

另请了解[下一轮](#example-2-retrieving-additional-changes)该执行哪些操作。

#### <a name="initial-request"></a>初始请求

在该示例中，由于频道消息为首次同步，因此第一个同步请求不含任何状态令牌。这一轮将返回该日历视图中的所有事件。

请求指定可选请求标头 odata.top，每次返回 2 个事件。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="initial-request-response"></a>第一个请求响应

该响应包含两个消息和一个具有 `skipToken` 的 `@odata.nextLink` 响应标头。`nextLink` URL 表示该频道中有更多要获取的消息。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T07:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T07:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T08:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T08:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="second-request"></a>第二个请求

第二个请求指定上一个响应中返回的 `nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 top 参数，因为 `nextLink` URL 中的 `skipToken` 已将其编码并包含在内。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="second-request-response"></a>第二个请求响应

第二个响应返回接下来的 2 个消息和一个带有 `skipToken` 的 `@odata.nextLink` 响应标头，指示频道中存在更多可获取的消息。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        },
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T09:50:20.152Z",
            "lastModifiedDateTime": "2019-03-06T09:50:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

#### <a name="third-request"></a>第三个请求

第三个请求继续使用上一个同步请求返回的最新 `nextLink`。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="third-request-response"></a>第三个请求响应

第三个响应仅返回频道中剩下的消息以及带有 `deltaToken` 的 `@odata.deltaLink` 响应标头，指示频道中的所有消息均已阅读。保存并使用 `deltaLink` URL 可在下一轮中查询从此刻开始的任何新消息。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a>示例 2：检索其他更改

使用上一轮中最后一个请求返回的 `deltaLink`，可以只获取从那以后此频道中发生变化（已添加或更新）的消息。假设你愿意在响应中保持页面大小上限不变，你的请求将如下所示：

#### <a name="request"></a>请求



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from": {
                "user": { 
                    "id": "id-value",
                    "displayName": "John Doe"
                }  
            },
            "etag": "id-value",
            "messageType": "message",
            "createdDateTime": "2019-03-06T10:40:20.152Z",
            "lastModifiedDateTime": "2019-03-06T10:40:20.152Z",
            "body": {
                "content": "Hello World",
                "contentType": "Text"
            },
            "attachments": [],
            "mentions": [],
            "importance": "normal",
            "reactions": [],
            "locale": "en-us"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Channel messages: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    ]
}
-->


