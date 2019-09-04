---
title: chatMessages：delta
description: 检索团队频道中的消息列表（无回复）。 通过使用增量查询，可以获取频道中新的或更新的消息。
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: e5f297dc236899f0fbd362c7ef369897b7bc7786
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719868"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="9cc56-104">chatMessages：delta</span><span class="sxs-lookup"><span data-stu-id="9cc56-104">chatMessages: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc56-105">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="9cc56-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="9cc56-106">通过使用增量查询，可以获取频道中新的或更新的消息。</span><span class="sxs-lookup"><span data-stu-id="9cc56-106">By using delta query, you can get new, updated, or deleted events in a calendar view.</span></span>

<span data-ttu-id="9cc56-107">增量查询既支持可检索指定频道中的所有消息的完全同步，也支持可检索自上次同步后频道中添加或发生变化的消息的增量同步。</span><span class="sxs-lookup"><span data-stu-id="9cc56-107">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization.</span></span> <span data-ttu-id="9cc56-108">通常情况下，开始时会执行一次完全同步，随后会定期获取相应日历视图的增量更改。</span><span class="sxs-lookup"><span data-stu-id="9cc56-108">Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="9cc56-109">若要获取消息的回复，请使用[列出消息回复](channel-get-messagereply.md)或[获取消息回复](channel-list-messagereplies.md)操作。</span><span class="sxs-lookup"><span data-stu-id="9cc56-109">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span>

<span data-ttu-id="9cc56-110">使用 delta 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="9cc56-110">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="9cc56-111">`nextLink`（包含具有 **delta** 函数调用和 `skipToken` 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="9cc56-111">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="9cc56-112">`deltaLink`（包含具有 **delta** 函数调用和 `deltaToken` 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="9cc56-112">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="9cc56-113">状态令牌对客户端完全不透明。</span><span class="sxs-lookup"><span data-stu-id="9cc56-113">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="9cc56-114">若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 delta 函数调用即可。</span><span class="sxs-lookup"><span data-stu-id="9cc56-114">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="9cc56-115">响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。</span><span class="sxs-lookup"><span data-stu-id="9cc56-115">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="9cc56-116">可以保存 `deltaLink` URL，并在开始下一轮时使用。</span><span class="sxs-lookup"><span data-stu-id="9cc56-116">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="9cc56-117">有关详细信息，请参阅[增量查询](/graph/delta-query-overview.md)文档。</span><span class="sxs-lookup"><span data-stu-id="9cc56-117">For more information, see the [delta query](/graph/delta-query-overview.md) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc56-118">权限</span><span class="sxs-lookup"><span data-stu-id="9cc56-118">Permissions</span></span>

<span data-ttu-id="9cc56-p105">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9cc56-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="9cc56-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc56-121">Permission Type</span></span>                        |<span data-ttu-id="9cc56-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cc56-122">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="9cc56-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc56-123">Delegated (work or school account)</span></span>     |<span data-ttu-id="9cc56-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc56-124">Group.Read.All, Group.ReadWrite.All</span></span>          |
|<span data-ttu-id="9cc56-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc56-125">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9cc56-126">不支持</span><span class="sxs-lookup"><span data-stu-id="9cc56-126">Not Supported</span></span>                                |
|<span data-ttu-id="9cc56-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cc56-127">Application</span></span>                            |<span data-ttu-id="9cc56-128">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc56-128">Group.Read.All, Group.ReadWrite.All</span></span>          |

## <a name="http-request"></a><span data-ttu-id="9cc56-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc56-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="9cc56-130">查询参数</span><span class="sxs-lookup"><span data-stu-id="9cc56-130">Query parameters</span></span>

<span data-ttu-id="9cc56-131">跟踪频道消息更改会引发一组对 **delta** 函数的一次或多次调用。</span><span class="sxs-lookup"><span data-stu-id="9cc56-131">Tracking changes in users incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="9cc56-132">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="9cc56-132">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="9cc56-133">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="9cc56-133">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="9cc56-134">只需预先指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="9cc56-134">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="9cc56-135">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="9cc56-135">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="9cc56-136">查询参数</span><span class="sxs-lookup"><span data-stu-id="9cc56-136">Query parameter</span></span>      | <span data-ttu-id="9cc56-137">类型</span><span class="sxs-lookup"><span data-stu-id="9cc56-137">Type</span></span>   |<span data-ttu-id="9cc56-138">说明</span><span class="sxs-lookup"><span data-stu-id="9cc56-138">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="9cc56-139">string</span><span class="sxs-lookup"><span data-stu-id="9cc56-139">string</span></span> | <span data-ttu-id="9cc56-140">之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。</span><span class="sxs-lookup"><span data-stu-id="9cc56-140">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire  URL including this token in the first request of the next round of change tracking for that collection.</span></span> <span data-ttu-id="9cc56-141">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="9cc56-141">A state token returned in the  URL of the previous delta function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="9cc56-142">字符串</span><span class="sxs-lookup"><span data-stu-id="9cc56-142">string</span></span> | <span data-ttu-id="9cc56-143">上一个 **delta** 函数调用中的 `nextLink` URL 返回的[状态令牌](/graph/delta-query-overview)，指示需要跟踪进一步的更改。</span><span class="sxs-lookup"><span data-stu-id="9cc56-143">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="9cc56-144">OData 可选查询参数</span><span class="sxs-lookup"><span data-stu-id="9cc56-144">Optional OData query parameters</span></span>

<span data-ttu-id="9cc56-145">此 API 支持以下[ OData 查询参数](/graph/query-parameters)：</span><span class="sxs-lookup"><span data-stu-id="9cc56-145">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="9cc56-146">`$top`，表示在调用中获取的最大消息数。</span><span class="sxs-lookup"><span data-stu-id="9cc56-146">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="9cc56-147">上限为 **50**。</span><span class="sxs-lookup"><span data-stu-id="9cc56-147">The upper limit is **50**.</span></span>
- <span data-ttu-id="9cc56-148">`$skip`，表示列表开头要跳过的消息数。</span><span class="sxs-lookup"><span data-stu-id="9cc56-148">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="9cc56-149">`$filter`，允许返回满足特定条件的消息。</span><span class="sxs-lookup"><span data-stu-id="9cc56-149">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="9cc56-150">支持筛选的唯一属性是 `lastModifiedDateTime`，且仅支持 **gt** 和 **ge** 运算符。</span><span class="sxs-lookup"><span data-stu-id="9cc56-150">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** and **ge** operators are supported.</span></span> <span data-ttu-id="9cc56-151">例如，`../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` 将提取指定日期时间后创建或更改的任何消息。</span><span class="sxs-lookup"><span data-stu-id="9cc56-151">For example, `../messages/delta?$filter=lastModifiedDateTime ge 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cc56-152">请求头</span><span class="sxs-lookup"><span data-stu-id="9cc56-152">Request headers</span></span>
| <span data-ttu-id="9cc56-153">标头</span><span class="sxs-lookup"><span data-stu-id="9cc56-153">Header</span></span>        | <span data-ttu-id="9cc56-154">值</span><span class="sxs-lookup"><span data-stu-id="9cc56-154">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="9cc56-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc56-155">Authorization</span></span> | <span data-ttu-id="9cc56-p110">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cc56-p110">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cc56-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cc56-158">Content-Type</span></span>  | <span data-ttu-id="9cc56-159">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc56-159">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9cc56-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc56-160">Request Body</span></span>

<span data-ttu-id="9cc56-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cc56-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cc56-162">响应</span><span class="sxs-lookup"><span data-stu-id="9cc56-162">Response</span></span>

<span data-ttu-id="9cc56-163">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](https://docs.microsoft.com/zh-CN/graph/api/resources/chatmessage?view=graph-rest-beta) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9cc56-163">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](https://docs.microsoft.com/en-us/graph/api/resources/chatmessage?view=graph-rest-beta) objects in the response body.</span></span> <span data-ttu-id="9cc56-164">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="9cc56-164">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="9cc56-165">示例</span><span class="sxs-lookup"><span data-stu-id="9cc56-165">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="9cc56-166">示例 1：初始同步</span><span class="sxs-lookup"><span data-stu-id="9cc56-166">Example 1: Initial synchronization</span></span>

<span data-ttu-id="9cc56-167">以下示例显示了用于同步给定频道中消息的三个请求。</span><span class="sxs-lookup"><span data-stu-id="9cc56-167">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="9cc56-168">频道中有五个消息。</span><span class="sxs-lookup"><span data-stu-id="9cc56-168">There are five messages in the channel.</span></span>

- <span data-ttu-id="9cc56-169">第 1 步：[示例第一个请求](#initial-request)和[响应](#initial-request-response)。</span><span class="sxs-lookup"><span data-stu-id="9cc56-169">[Step 1: sample initial request](#initial-request) and [response](#initial-request-response)</span></span>
- <span data-ttu-id="9cc56-170">第 2 步：[示例第二个请求](#second-request)和[响应](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="9cc56-170">[Step 2: sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="9cc56-171">第 3 步：[示例第三个请求](#third-request)和[最终响应](#third-request-response)。</span><span class="sxs-lookup"><span data-stu-id="9cc56-171">[Step 3: sample third request](#third-request) and [final response](#third-request-response)</span></span>

<span data-ttu-id="9cc56-p113">为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。</span><span class="sxs-lookup"><span data-stu-id="9cc56-p113">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="9cc56-174">另请了解[下一轮](#example-2-retrieving-additional-changes)该执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="9cc56-174">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="9cc56-175">初始请求</span><span class="sxs-lookup"><span data-stu-id="9cc56-175">Initial request</span></span>

<span data-ttu-id="9cc56-176">本示例中，频道消息正在进行首次同步，因此初始同步请求未包含任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="9cc56-176">In this example, the specified folder is being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="9cc56-177">这一轮将返回此日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="9cc56-177">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="9cc56-178">请求指定可选请求标头 odata.top，每次返回 2 个事件。</span><span class="sxs-lookup"><span data-stu-id="9cc56-178">The optional request header, odata.maxpagesize, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cc56-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc56-179">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cc56-180">C#</span><span class="sxs-lookup"><span data-stu-id="9cc56-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cc56-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc56-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cc56-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc56-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="9cc56-183">第一个请求响应</span><span class="sxs-lookup"><span data-stu-id="9cc56-183">Initial request and response</span></span>

<span data-ttu-id="9cc56-184">该响应包含两封邮件和一个具有 `skipToken` 的 `@odata.nextLink` 响应标头。</span><span class="sxs-lookup"><span data-stu-id="9cc56-184">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`. The  indicates there are more messages in the folder to get.</span></span> <span data-ttu-id="9cc56-185">`nextLink` URL 表示此频道中还更多邮件可获取。</span><span class="sxs-lookup"><span data-stu-id="9cc56-185">The `nextLink` URL indicates there are more messages in the folder to get.</span></span>

><span data-ttu-id="9cc56-186">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cc56-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9cc56-187">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cc56-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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
            "from" : {
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

#### <a name="second-request"></a><span data-ttu-id="9cc56-188">第二个请求</span><span class="sxs-lookup"><span data-stu-id="9cc56-188">Second request</span></span>

<span data-ttu-id="9cc56-189">第二个请求指定上一个响应中返回的 `nextLink` URL。</span><span class="sxs-lookup"><span data-stu-id="9cc56-189">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="9cc56-190">请注意，无需再像在第一个请求中一样指定相同的顶级参数，因为 `nextLink` URL 中的 `skipToken` 会将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="9cc56-190">Notice that it no longer has to specify the same startDateTime and endDateTime parameters as in the initial request, as the  in the  URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cc56-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc56-191">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cc56-192">C#</span><span class="sxs-lookup"><span data-stu-id="9cc56-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cc56-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc56-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cc56-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc56-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="9cc56-195">第二个请求响应</span><span class="sxs-lookup"><span data-stu-id="9cc56-195">Second request response</span></span>

<span data-ttu-id="9cc56-196">第二个响应返回接下来的 2 个消息和一个带有 `skipToken` 的 `@odata.nextLink` 响应标头，指示频道中存在可获取的更多消息。</span><span class="sxs-lookup"><span data-stu-id="9cc56-196">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`. The  indicates there are more messages in the folder to get.</span></span>

><span data-ttu-id="9cc56-197">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cc56-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9cc56-198">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cc56-198">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.nextLink": "/teams('id')/channels('id')/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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
            "from" : {
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

#### <a name="third-request"></a><span data-ttu-id="9cc56-199">第三个请求</span><span class="sxs-lookup"><span data-stu-id="9cc56-199">Third sync request</span></span>

<span data-ttu-id="9cc56-200">第三个请求继续使用上一个同步请求返回的最新 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="9cc56-200">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cc56-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc56-201">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cc56-202">C#</span><span class="sxs-lookup"><span data-stu-id="9cc56-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cc56-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc56-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cc56-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc56-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="9cc56-205">第三个请求响应</span><span class="sxs-lookup"><span data-stu-id="9cc56-205">Third request response</span></span>

<span data-ttu-id="9cc56-206">第三个响应仅返回频道中剩下的消息以及带有 `deltaToken` 的 `@odata.deltaLink` 响应标头，指示频道中的所有消息已被阅读。</span><span class="sxs-lookup"><span data-stu-id="9cc56-206">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="9cc56-207">保存并使用 `deltaLink` URL，以便查询下一轮中从此点开始的任何新消息。</span><span class="sxs-lookup"><span data-stu-id="9cc56-207">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="9cc56-208">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cc56-208">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9cc56-209">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cc56-209">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="9cc56-210">示例 2：检索其他更改</span><span class="sxs-lookup"><span data-stu-id="9cc56-210">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="9cc56-211">使用上一轮中最后一个请求返回的 `deltaLink`，可以只获取从那以后此频道中发生变化（已添加或更新）的邮件。</span><span class="sxs-lookup"><span data-stu-id="9cc56-211">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, deleted, or updated) in that folder since then.</span></span> <span data-ttu-id="9cc56-212">假如你更喜欢在响应中保持最大页面的同一大小，则请求将如下所示：</span><span class="sxs-lookup"><span data-stu-id="9cc56-212">Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="9cc56-213">请求</span><span class="sxs-lookup"><span data-stu-id="9cc56-213">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cc56-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc56-214">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cc56-215">C#</span><span class="sxs-lookup"><span data-stu-id="9cc56-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cc56-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc56-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cc56-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc56-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cc56-218">响应</span><span class="sxs-lookup"><span data-stu-id="9cc56-218">Response</span></span>

><span data-ttu-id="9cc56-p122">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cc56-p122">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "/$metadata#Collection(Microsoft.Teams.GraphSvc.chatMessage)",
    "@odata.deltaLink": "/teams('id')/channels('id')/messages/delta?$deltatoken=c3RhcnRUaW1l5Ti1NTEyODc1ODB0OTAyXGFdZVNpemU9MjA%3d",
    "value": [
        {
            "id": "id-value",
            "replyToId": "id-value",
            "from" : {
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
