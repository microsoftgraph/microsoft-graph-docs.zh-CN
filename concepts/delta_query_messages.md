# <a name="get-incremental-changes-to-messages-in-a-folder"></a><span data-ttu-id="7da8c-101">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="7da8c-101">Get incremental changes to messages in a folder</span></span> 

<span data-ttu-id="7da8c-p101">Delta 查询可通过调用一系列的 [delta](../api-reference/v1.0/api/message_delta.md) 函数查询文件夹中邮件的添加、删除或更新。Delta 数据使你可以维护和同步本地存储的用户邮件，而无需每次都从服务器中获取整组邮件。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p101">Delta query lets you query for additions, deletions, or updates to messages in a folder, by way of a series of [delta](../api-reference/v1.0/api/message_delta.md) function calls. Delta data enables you to maintain and synchronize a local store of a user's messages, without having to fetch the entire set of the user's messages from the server every time.</span></span>

<span data-ttu-id="7da8c-p102">Delta 查询支持检索文件夹（例如，用户的收件箱）中所有邮件的完全同步，以及检索自上次同步以来该文件夹中所有已更改邮件的增量同步。通常，需要对文件夹中的所有邮件进行初始完全同步，之后可定期获取该文件夹的增量更改。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p102">Delta query supports both full synchronization that retrieves all of the messages in a folder (for example, the user's Inbox), and incremental synchronization that retrieves all of the messages that have changed in that folder since the last synchronization. Typically, you would do an initial full synchronization of all the messages in a folder, and subsequently, get incremental changes to that folder periodically.</span></span> 

## <a name="track-message-changes-in-a-folder"></a><span data-ttu-id="7da8c-106">跟踪文件夹中的邮件更改</span><span class="sxs-lookup"><span data-stu-id="7da8c-106">Track message changes in a folder</span></span>

<span data-ttu-id="7da8c-p103">Delta 查询对每个文件夹分别执行操作。为跟踪文件夹层次结构中邮件的更改，需要分别跟踪每个文件夹。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p103">Delta query is a per-folder operation. To track the changes of the messages in a folder hierarchy, you need to track each folder individually.</span></span> 

<span data-ttu-id="7da8c-p104">跟踪邮件文件夹中的邮件更改通常需要使用 **delta** 函数按轮发出一个或多个 GET 请求。初始 GET 请求非常类似于[获取邮件](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages)，区别在于要添加 **delta** 函数：</span><span class="sxs-lookup"><span data-stu-id="7da8c-p104">Tracking message changes in a mail folder typically is a round of one or more GET requests with the **delta** function. The initial GET request is very much like the way you [get messages](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_messages), except that you include the **delta** function:</span></span>

```
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

<span data-ttu-id="7da8c-111">使用 **delta** 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="7da8c-111">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="7da8c-112">`nextLink`（包含具有 **delta** 函数调用和 _skipToken_ 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="7da8c-112">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="7da8c-113">`deltaLink`（包含具有 **delta** 函数调用和 _deltaToken_ 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="7da8c-113">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="7da8c-p105">这些令牌是对客户端完全不透明的[状态令牌](delta_query_overview.md#state-tokens)。若要继续一轮邮件更改跟踪，只需将最后一个 GET 请求返回的 URL 复制并应用到同一文件夹的下一个 **delta** 函数调用即可。响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `deltaLink` URL，并在开始下一轮时使用。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p105">These tokens are [state tokens](delta_query_overview.md#state-tokens) that are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the URL returned from the last GET request to the next **delta** function call for the same folder. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="7da8c-118">若要了解如何使用 `nextLink` 和 `deltaLink` URL，请参阅下面的[示例](#example-to-synchronize-messages-in-a-folder)。</span><span class="sxs-lookup"><span data-stu-id="7da8c-118">See the [example](#example-to-synchronize-messages-in-a-folder) below to learn how to use the `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a><span data-ttu-id="7da8c-119">在邮件的增量查询中使用查询参数</span><span class="sxs-lookup"><span data-stu-id="7da8c-119">Use query parameters in a delta query for messages</span></span>

- <span data-ttu-id="7da8c-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="7da8c-122">对于邮件，Delta 查询支持 `$select`、`$top` 和 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="7da8c-122">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="7da8c-123">提供对 `$filter` 和 `$orderby` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="7da8c-123">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="7da8c-124">唯一支持的 `$filter` 表达式是 `$filter=receivedDateTime+ge+{value}` 或 `$filter=receivedDateTime+gt+{value}`。</span><span class="sxs-lookup"><span data-stu-id="7da8c-124">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="7da8c-p107">唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p107">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="7da8c-127">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="7da8c-127">There is no support for `$search`.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="7da8c-128">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="7da8c-128">Optional request header</span></span>

<span data-ttu-id="7da8c-p108">每个 delta 查询 GET 请求在响应中返回一个或多个邮件的集合。可以选择性地指定请求标头 _Prefer: odata.maxpagesize={x}_，以设置响应的最大邮件数。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p108">Each delta query GET request returns a collection of one or more messages in the response. You can optionally specify the request header, _Prefer: odata.maxpagesize={x}_, to set the maximum number of messages in a response.</span></span>

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

## <a name="example-to-synchronize-messages-in-a-folder"></a><span data-ttu-id="7da8c-131">同步文件夹中邮件的示例</span><span class="sxs-lookup"><span data-stu-id="7da8c-131">Example to synchronize messages in a folder</span></span>

<span data-ttu-id="7da8c-132">以下示例显示对包含 5 封邮件的特定文件夹进行同步的 3 个请求：</span><span class="sxs-lookup"><span data-stu-id="7da8c-132">The following example shows a series of 3 requests to synchronize a specific folder which contains 5 messages:</span></span>

- <span data-ttu-id="7da8c-133">[示例：初始请求](#sample-initial-request)和[响应](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="7da8c-133">[Sample initial request](#sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="7da8c-134">[示例：第二个请求](#sample-second-request)和[响应](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="7da8c-134">[Sample second request](#sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="7da8c-135">[示例：第三个请求](#sample-third-request)和[最终响应](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="7da8c-135">[Sample third request](#sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="7da8c-136">另请参阅[下一轮](#the-next-round)以了解如何做。</span><span class="sxs-lookup"><span data-stu-id="7da8c-136">See also what you'll do in the [next round](#the-next-round).</span></span>


### <a name="sample-initial-request"></a><span data-ttu-id="7da8c-137">示例：初始请求</span><span class="sxs-lookup"><span data-stu-id="7da8c-137">Sample initial request</span></span>

<span data-ttu-id="7da8c-p109">本示例中，指定文件夹正在进行首次同步，因此初始同步请求未包含任何状态令牌。此轮将返回该文件夹中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p109">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the messages in that folder.</span></span>

<span data-ttu-id="7da8c-140">第一个请求指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="7da8c-140">The first request specifies the following:</span></span>

- <span data-ttu-id="7da8c-141">`$select` 参数用于在响应中返回每个邮件的**主题**和**发件人**属性。</span><span class="sxs-lookup"><span data-stu-id="7da8c-141">A `$select` parameter to return the **Subject** and **Sender** properties for each message in the response.</span></span>
- <span data-ttu-id="7da8c-142">[可选的请求标头](#optional-request-header) _odata.maxpagesize_，一次返回两封邮件。</span><span class="sxs-lookup"><span data-stu-id="7da8c-142">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 messages at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_1"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$select=Subject,Sender HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a><span data-ttu-id="7da8c-143">示例第一个响应</span><span class="sxs-lookup"><span data-stu-id="7da8c-143">Sample initial response</span></span>

<span data-ttu-id="7da8c-p110">响应中返回两封邮件和一个 `@odata.nextLink` 响应头。`nextLink` URL 表示此文件夹中还更多邮件可获取。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p110">The response includes two messages and an `@odata.nextLink` response header. The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

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

### <a name="sample-second-request"></a><span data-ttu-id="7da8c-146">示例第二个请求</span><span class="sxs-lookup"><span data-stu-id="7da8c-146">Sample second request</span></span>

<span data-ttu-id="7da8c-p111">第二个请求指定上一个响应中返回的 `nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 `$select` 参数，因为 `nextLink` URL 中的 `skipToken` 已将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same `$select` parameter as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_2"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a><span data-ttu-id="7da8c-149">示例第二个响应</span><span class="sxs-lookup"><span data-stu-id="7da8c-149">Sample second response</span></span> 

<span data-ttu-id="7da8c-150">第二个响应中返回此文件夹中接下来的 2 封邮件和另一个 `nextLink`（表示此文件夹中还有更多邮件可获取）。</span><span class="sxs-lookup"><span data-stu-id="7da8c-150">The second response returns the next 2 messages in the folder and another `nextLink`, indicating there are more messages to get from the folder.</span></span>

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


### <a name="sample-third-request"></a><span data-ttu-id="7da8c-151">示例第三个请求</span><span class="sxs-lookup"><span data-stu-id="7da8c-151">Sample third request</span></span>

<span data-ttu-id="7da8c-152">第三个请求继续使用上一个同步请求返回的最新 `nextLink` URL。</span><span class="sxs-lookup"><span data-stu-id="7da8c-152">The third request continues to use the latest `nextLink` URL returned from the last sync request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a><span data-ttu-id="7da8c-153">示例第三个响应（即最终响应）</span><span class="sxs-lookup"><span data-stu-id="7da8c-153">Sample third and final response</span></span>

<span data-ttu-id="7da8c-p112">第三个响应中返回此文件夹中仅剩的邮件，以及表示目前已完成同步此文件夹的 `deltaLink` URL。保存并使用 `deltaLink` URL [在下一轮中同步同一文件夹](#the-next-round)。</span><span class="sxs-lookup"><span data-stu-id="7da8c-p112">The third response returns the only remaining message in the folder, and a `deltaLink` URL which indicates synchronization is complete for the time being for this folder. Save and use the `deltaLink` URL to [synchronize the same folder in the next round](#the-next-round).</span></span>

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


### <a name="the-next-round"></a><span data-ttu-id="7da8c-156">下一轮</span><span class="sxs-lookup"><span data-stu-id="7da8c-156">The next round</span></span>

<span data-ttu-id="7da8c-p113">使用上一轮中[最后一个请求](#sample-third-request)返回的 `deltaLink`，可以只获取从那以后此文件夹中发生变化（已添加、删除或更新）的邮件。假设你愿意在响应中保持页面大小上限不变，下一轮的第一个请求如下所示：</span><span class="sxs-lookup"><span data-stu-id="7da8c-p113">Using the `deltaLink` from the [last request](#sample-third-request) in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_messages_delta_next"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```



## <a name="see-also"></a><span data-ttu-id="7da8c-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7da8c-159">See also</span></span>

- [<span data-ttu-id="7da8c-160">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="7da8c-160">Microsoft Graph delta query</span></span>](../Concepts/delta_query_overview.md)
- [<span data-ttu-id="7da8c-161">获取日历视图中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="7da8c-161">Get incremental changes to events in a calendar view</span></span>](../Concepts/delta_query_events.md)
- [<span data-ttu-id="7da8c-162">获取组的增量更改</span><span class="sxs-lookup"><span data-stu-id="7da8c-162">Get incremental changes to groups</span></span>](../Concepts/delta_query_groups.md)
- [<span data-ttu-id="7da8c-163">获取用户的增量更改</span><span class="sxs-lookup"><span data-stu-id="7da8c-163">Get incremental changes to users</span></span>](../Concepts/delta_query_users.md)
