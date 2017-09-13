# <a name="get-incremental-changes-to-messages-in-a-folder"></a>获取文件夹中邮件的增量更改 

Delta 查询可通过调用一系列的 [delta](../api-reference/v1.0/api/message_delta.md) 函数查询文件夹中邮件的添加、删除或更新。Delta 数据使你可以维护和同步本地存储的用户邮件，而无需每次都从服务器中获取整组邮件。

Delta 查询支持检索文件夹（例如，用户的收件箱）中所有邮件的完全同步，以及检索自上次同步以来该文件夹中所有已更改邮件的增量同步。通常，需要对文件夹中的所有邮件进行初始完全同步，之后可定期获取该文件夹的增量更改。 

## <a name="track-message-changes-in-a-folder"></a>跟踪文件夹中的邮件更改

Delta 查询对每个文件夹分别执行操作。为跟踪文件夹层次结构中邮件的更改，需要分别跟踪每个文件夹。 

跟踪邮件文件夹中的邮件更改通常需要使用 **delta** 函数按轮发出一个或多个 GET 请求。初始 GET 请求非常类似于[获取邮件](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages)，区别在于要添加 **delta** 函数：

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

使用 **delta** 函数的 GET 请求返回以下任一内容：

- `nextLink`（包含具有 **delta** 函数调用和 _skipToken_ 的 URL），或 
- `deltaLink`（包含具有 **delta** 函数调用和 _deltaToken_ 的 URL）。

这些令牌是对客户端完全不透明的[状态令牌](delta_query_overview.md#state-tokens)。若要继续一轮邮件更改跟踪，只需将最后一个 GET 请求返回的 URL 复制并应用到同一文件夹的下一个 **delta** 函数调用即可。响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `deltaLink` URL，并在开始下一轮时使用。

若要了解如何使用 `nextLink` 和 `deltaLink` URL，请参阅下面的[示例](#example-to-synchronize-messages-in-a-folder)。

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a>在邮件的增量查询中使用查询参数

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 
- 对于邮件，Delta 查询支持 `$select`、`$top` 和 `$expand`。 
- 提供对 `$filter` 和 `$orderby` 的有限支持：
  * 唯一支持的 `$filter` 表达式是 `$filter=receivedDateTime+ge+{value}` 或 `$filter=receivedDateTime+gt+{value}`。
  * 唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。 
- 不支持 `$search`。


### <a name="optional-request-header"></a>可选的请求标头

每个 delta 查询 GET 请求在响应中返回一个或多个邮件的集合。可以选择性地指定请求标头 _Prefer: odata.maxpagesize={x}_，以设置响应的最大邮件数。

<!--
### Iterative process 

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query 
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative 
process (steps 2-6) described below will return the entire set of messages in that folder. 

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header, 
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned 
   in _@odata.nextLink_, which includes a _skipToken_. 

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages, 
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3. 

6. When you eventually receive a _detlaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This 
round of change tracking is complete. 

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request 
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated) 
since the completion of the very first round.

-->

## <a name="example-to-synchronize-messages-in-a-folder"></a>同步文件夹中邮件的示例

以下示例显示对包含 5 封邮件的特定文件夹进行同步的 3 个请求：

- [示例：初始请求](#sample-initial-request)和[响应](#sample-initial-response)
- [示例：第二个请求](#sample-second-request)和[响应](#sample-second-response)
- [示例：第三个请求](#sample-third-request)和[最终响应](#sample-third-and-final-response)

另请参阅[下一轮](#the-next-round)以了解如何做。


### <a name="sample-initial-request"></a>示例：初始请求

本示例中，指定文件夹正在进行首次同步，因此初始同步请求未包含任何状态令牌。此轮将返回该文件夹中的所有邮件。

第一个请求指定以下内容：

- `$select` 参数用于在响应中返回每个邮件的**主题**和**发件人**属性。
- [可选的请求标头](#optional-request-header) _odata.maxpagesize_，一次返回两封邮件。

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a>示例第一个响应

响应中返回两封邮件和一个 `@odata.nextLink` 响应头。`nextLink` URL 表示此文件夹中还更多邮件可获取。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
            "subject":"Holiday hours update",
            "sender":{
                "emailAddress":{
                    "name":"Dana Swope",
                    "address":"danas@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADNkNAAASq35xAAA="
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
            "subject":"Holiday promotion sale",
            "sender":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAVRMKAAAAA=="
        }
    ]
}
```

### <a name="sample-second-request"></a>示例第二个请求

第二个请求指定上一个响应中返回的 `nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 `$select` 参数，因为 `nextLink` URL 中的 `skipToken` 已将其编码并包含在内。

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>示例第二个响应 

第二个响应中返回此文件夹中接下来的 2 封邮件和另一个 `nextLink`（表示此文件夹中还有更多邮件可获取）。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWJAAAA"
        },
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB9\"",
            "subject":"New or modified user account information",
            "sender":{
                "emailAddress":{
                    "name":"Randi Welch",
                    "address":"randiw@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWHAAAA"
        }
    ]
}
```


### <a name="sample-third-request"></a>示例第三个请求

第三个请求继续使用上一个同步请求返回的最新 `nextLink` URL。 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>示例第三个响应（即最终响应）

第三个响应中返回此文件夹中仅剩的邮件，以及表示目前已完成同步此文件夹的 `deltaLink` URL。保存并使用 `deltaLink` URL [在下一轮中同步同一文件夹](#the-next-round)。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
    "value":[
        {
            "@odata.type":"#microsoft.graph.message",
            "@odata.etag":"W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB8\"",
            "subject":"You've joined the Customer Manager group",
            "sender":{
                "emailAddress":{
                    "name":"Customer Managers team",
                    "address":"customer_managers@contoso.onmicrosoft.com"
                }
            },
            "id":"AQMkADNkNAAAgWFAAAA"
        }
    ]
}
```


### <a name="the-next-round"></a>下一轮

使用上一轮中[最后一个请求](#sample-third-request)返回的 `deltaLink`，可以只获取从那以后此文件夹中发生变化（已添加、删除或更新）的邮件。假设你愿意在响应中保持页面大小上限不变，下一轮的第一个请求如下所示：

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](../Concepts/delta_query_overview.md)
- [获取日历视图中事件的增量更改](../Concepts/delta_query_events.md)
- [获取组的增量更改](../Concepts/delta_query_groups.md)
- [获取用户的增量更改](../Concepts/delta_query_users.md)
