---
title: 'chatMessages: delta'
description: 检索团队频道中的消息列表（无回复）。可以通过使用 delta 查询获取频道中的新消息或更新消息。
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 6321c440da24245d1f39c604cb52def894b47a31
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49030121"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="004dc-104">chatMessages: delta</span><span class="sxs-lookup"><span data-stu-id="004dc-104">chatMessages: delta</span></span>

<span data-ttu-id="004dc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="004dc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="004dc-p102">检索[团队](../resources/channel.md)[频道](../resources/team.md)中的[消息](../resources/chatmessage.md)列表（无回复）。可以通过使用 delta 查询获取频道中的新消息或更新消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-p102">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md). By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="004dc-p103">**注意：** Delta 将近返回过去 8 个月内的消息。可以使用 [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) 检索更早的消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-p103">**Note:** Delta will only return messages within the last eight months. You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="004dc-p104">Delta 查询既支持可检索指定频道中所有消息的完全同步，也支持可检索自上次同步后频道中添加或更改的消息的增量同步。通常情况下，开始时会执行一次完全同步，然后会定期获取相应日历视图的增量更改。</span><span class="sxs-lookup"><span data-stu-id="004dc-p104">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization. Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="004dc-112">若要获取消息的回复，请使用[列出消息回复](channel-get-messagereply.md)或[获取消息回复](channel-list-messagereplies.md)操作。</span><span class="sxs-lookup"><span data-stu-id="004dc-112">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="004dc-113">使用 delta 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="004dc-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="004dc-114">`nextLink`（包含具有 **delta** 函数调用和 `skipToken` 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="004dc-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="004dc-115">`deltaLink`（包含具有 **delta** 函数调用和 `deltaToken` 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="004dc-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="004dc-p105">状态令牌对客户端完全不透明。若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 delta 函数调用即可。响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。可以保存 `deltaLink` URL，并在开始下一轮时使用。</span><span class="sxs-lookup"><span data-stu-id="004dc-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="004dc-120">有关详细信息，请参阅 [delta 查询](/graph/delta-query-overview)文档。</span><span class="sxs-lookup"><span data-stu-id="004dc-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="004dc-121">权限</span><span class="sxs-lookup"><span data-stu-id="004dc-121">Permissions</span></span>

<span data-ttu-id="004dc-p106">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="004dc-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="004dc-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="004dc-124">Permission Type</span></span>                        |<span data-ttu-id="004dc-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="004dc-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="004dc-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="004dc-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="004dc-127">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004dc-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="004dc-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="004dc-128">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="004dc-129">不支持</span><span class="sxs-lookup"><span data-stu-id="004dc-129">Not Supported</span></span>                                |
|<span data-ttu-id="004dc-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="004dc-130">Application</span></span>                            | <span data-ttu-id="004dc-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004dc-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="004dc-132">**注意** ：标有 \* 的权限使用 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="004dc-132">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="004dc-p107">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。有关详细信息，请参阅 [Microsoft Teams 中受保护的 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="004dc-p107">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="004dc-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="004dc-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="004dc-136">查询参数</span><span class="sxs-lookup"><span data-stu-id="004dc-136">Query parameters</span></span>

<span data-ttu-id="004dc-p108">跟踪频道消息中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="004dc-p108">Tracking changes in channel messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="004dc-140">只需预先指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="004dc-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="004dc-141">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="004dc-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="004dc-142">查询参数</span><span class="sxs-lookup"><span data-stu-id="004dc-142">Query parameter</span></span>      | <span data-ttu-id="004dc-143">类型</span><span class="sxs-lookup"><span data-stu-id="004dc-143">Type</span></span>   |<span data-ttu-id="004dc-144">说明</span><span class="sxs-lookup"><span data-stu-id="004dc-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="004dc-145">字符串</span><span class="sxs-lookup"><span data-stu-id="004dc-145">string</span></span> | <span data-ttu-id="004dc-p109">之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="004dc-p109">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="004dc-148">字符串</span><span class="sxs-lookup"><span data-stu-id="004dc-148">string</span></span> | <span data-ttu-id="004dc-149">上一个 **delta** 函数调用中的 `nextLink` URL 返回的 [状态令牌](/graph/delta-query-overview)，指示需要跟踪进一步的更改。</span><span class="sxs-lookup"><span data-stu-id="004dc-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="004dc-150">OData 可选查询参数</span><span class="sxs-lookup"><span data-stu-id="004dc-150">Optional OData query parameters</span></span>

<span data-ttu-id="004dc-151">此 API 支持以下[ OData 查询参数](/graph/query-parameters)：</span><span class="sxs-lookup"><span data-stu-id="004dc-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="004dc-p110">`$top`，表示在调用中获取的最大消息数。上限为 **50** 。</span><span class="sxs-lookup"><span data-stu-id="004dc-p110">`$top`, represents maximum number of messages to fetch in a call. The upper limit is **50**.</span></span>
- <span data-ttu-id="004dc-154">`$skip`，表示列表开头要跳过的消息数。</span><span class="sxs-lookup"><span data-stu-id="004dc-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="004dc-p111">`$filter` 允许返回满足特定条件的消息。支持筛选的唯一属性为 `lastModifiedDateTime`，并且仅支持 **gt** 运算符。例如，`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` 将获取在指定日期/时间后创建或更高的所有消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-p111">`$filter` allows returning messages that meet a certain criteria. The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported. For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="004dc-158">请求标头</span><span class="sxs-lookup"><span data-stu-id="004dc-158">Request headers</span></span>
| <span data-ttu-id="004dc-159">标头</span><span class="sxs-lookup"><span data-stu-id="004dc-159">Header</span></span>        | <span data-ttu-id="004dc-160">值</span><span class="sxs-lookup"><span data-stu-id="004dc-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="004dc-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="004dc-161">Authorization</span></span> | <span data-ttu-id="004dc-p112">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="004dc-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="004dc-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="004dc-164">Content-Type</span></span>  | <span data-ttu-id="004dc-165">application/json</span><span class="sxs-lookup"><span data-stu-id="004dc-165">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="004dc-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="004dc-166">Request Body</span></span>

<span data-ttu-id="004dc-167">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="004dc-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="004dc-168">响应</span><span class="sxs-lookup"><span data-stu-id="004dc-168">Response</span></span>

<span data-ttu-id="004dc-p113">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。响应还包括 `nextLink` URL 或 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="004dc-p113">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body. The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="004dc-171">示例</span><span class="sxs-lookup"><span data-stu-id="004dc-171">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="004dc-172">示例 1：初始同步</span><span class="sxs-lookup"><span data-stu-id="004dc-172">Example 1: Initial synchronization</span></span>

<span data-ttu-id="004dc-p114">以下示例显示了用于同步给定频道中消息的三个请求。频道中有 5 个消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-p114">The following example shows a series of three requests to synchronize the messages in the given channel. There are five messages in the channel.</span></span>

- <span data-ttu-id="004dc-175">第 1 步：[示例第一个请求](#initial-request)和[响应](#initial-request-response)。</span><span class="sxs-lookup"><span data-stu-id="004dc-175">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="004dc-176">第 2 步：[示例第二个请求](#second-request)和[响应](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="004dc-176">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="004dc-177">第 3 步：[示例第三个请求](#third-request)和[最终响应](#third-request-response)。</span><span class="sxs-lookup"><span data-stu-id="004dc-177">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="004dc-p115">为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。</span><span class="sxs-lookup"><span data-stu-id="004dc-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="004dc-180">另请了解[下一轮](#example-2-retrieving-additional-changes)该执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="004dc-180">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="004dc-181">初始请求</span><span class="sxs-lookup"><span data-stu-id="004dc-181">Initial request</span></span>

<span data-ttu-id="004dc-p116">在该示例中，由于频道消息为首次同步，因此第一个同步请求不含任何状态令牌。这一轮将返回该日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="004dc-p116">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="004dc-184">请求指定可选请求标头 odata.top，每次返回 2 个事件。</span><span class="sxs-lookup"><span data-stu-id="004dc-184">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>


# <a name="http"></a>[<span data-ttu-id="004dc-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="004dc-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="004dc-186">C#</span><span class="sxs-lookup"><span data-stu-id="004dc-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="004dc-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="004dc-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="004dc-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="004dc-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="004dc-189">Java</span><span class="sxs-lookup"><span data-stu-id="004dc-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="initial-request-response"></a><span data-ttu-id="004dc-190">第一个请求响应</span><span class="sxs-lookup"><span data-stu-id="004dc-190">Initial request response</span></span>

<span data-ttu-id="004dc-p117">该响应包含两个消息和一个具有 `skipToken` 的 `@odata.nextLink` 响应标头。`nextLink` URL 表示该频道中有更多要获取的消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-p117">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="004dc-p118">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="004dc-p118">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="004dc-195">第二个请求</span><span class="sxs-lookup"><span data-stu-id="004dc-195">Second request</span></span>

<span data-ttu-id="004dc-p119">第二个请求指定上一个响应中返回的 `nextLink` URL。请注意，不再需要像第一个请求一样指定相同的 top 参数，因为 `nextLink` URL 中的 `skipToken` 已将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="004dc-p119">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="004dc-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="004dc-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="004dc-199">C#</span><span class="sxs-lookup"><span data-stu-id="004dc-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="004dc-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="004dc-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="004dc-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="004dc-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="004dc-202">Java</span><span class="sxs-lookup"><span data-stu-id="004dc-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="second-request-response"></a><span data-ttu-id="004dc-203">第二个请求响应</span><span class="sxs-lookup"><span data-stu-id="004dc-203">Second request response</span></span>

<span data-ttu-id="004dc-204">第二个响应返回接下来的 2 个消息和一个带有 `skipToken` 的 `@odata.nextLink` 响应标头，指示频道中存在更多可获取的消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-204">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="004dc-p120">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="004dc-p120">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="004dc-207">第三个请求</span><span class="sxs-lookup"><span data-stu-id="004dc-207">Third request</span></span>

<span data-ttu-id="004dc-208">第三个请求继续使用上一个同步请求返回的最新 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="004dc-208">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>


# <a name="http"></a>[<span data-ttu-id="004dc-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="004dc-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="004dc-210">C#</span><span class="sxs-lookup"><span data-stu-id="004dc-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="004dc-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="004dc-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="004dc-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="004dc-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="004dc-213">Java</span><span class="sxs-lookup"><span data-stu-id="004dc-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="third-request-response"></a><span data-ttu-id="004dc-214">第三个请求响应</span><span class="sxs-lookup"><span data-stu-id="004dc-214">Third request response</span></span>

<span data-ttu-id="004dc-p121">第三个响应仅返回频道中剩下的消息以及带有 `deltaToken` 的 `@odata.deltaLink` 响应标头，指示频道中的所有消息均已阅读。保存并使用 `deltaLink` URL 可在下一轮中查询从此刻开始的任何新消息。</span><span class="sxs-lookup"><span data-stu-id="004dc-p121">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read. Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="004dc-p122">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="004dc-p122">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="004dc-219">示例 2：检索其他更改</span><span class="sxs-lookup"><span data-stu-id="004dc-219">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="004dc-p123">使用上一轮中最后一个请求返回的 `deltaLink`，可以只获取从那以后此频道中发生变化（已添加或更新）的消息。假设你愿意在响应中保持页面大小上限不变，你的请求将如下所示：</span><span class="sxs-lookup"><span data-stu-id="004dc-p123">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then. Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="004dc-222">请求</span><span class="sxs-lookup"><span data-stu-id="004dc-222">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="004dc-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="004dc-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```http
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="004dc-224">C#</span><span class="sxs-lookup"><span data-stu-id="004dc-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="004dc-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="004dc-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="004dc-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="004dc-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="004dc-227">Java</span><span class="sxs-lookup"><span data-stu-id="004dc-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="004dc-228">响应</span><span class="sxs-lookup"><span data-stu-id="004dc-228">Response</span></span>

><span data-ttu-id="004dc-p124">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="004dc-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


