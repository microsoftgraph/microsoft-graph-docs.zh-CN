---
title: chatMessages：delta
description: 检索团队频道中的消息列表（无回复）。 通过使用增量查询，可以获取频道中新的或更新的消息。
localization_priority: Priority
doc_type: apiPageType
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: c1282d71fbd0ae51f4ce1a24549ca2721c77a260
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515658"
---
# <a name="chatmessages-delta"></a><span data-ttu-id="ad2f4-104">chatMessages：delta</span><span class="sxs-lookup"><span data-stu-id="ad2f4-104">chatMessages: delta</span></span>

<span data-ttu-id="ad2f4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad2f4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad2f4-106">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="ad2f4-107">通过使用增量查询，可以获取频道中新的或更新的消息。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="ad2f4-108">**请注意：** 增量查询将仅返回过去 8 个月内的邮件。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="ad2f4-109">要检索时间更早的邮件，可使用 [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md)。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-109">You can use [GET /teams/{id}/channels/{id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="ad2f4-110">增量查询既支持可检索指定频道中的所有消息的完全同步，也支持可检索自上次同步后频道中添加或发生变化的消息的增量同步。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-110">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="ad2f4-111">通常情况下，开始时会执行一次完全同步，随后会定期获取相应日历视图的增量更改。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-111">Typically, you would do an initial full synchronization, and then get incremental changes to that calendar view periodically.</span></span>

<span data-ttu-id="ad2f4-112">若要获取消息的回复，请使用[列出消息回复](channel-get-messagereply.md)或[获取消息回复](channel-list-messagereplies.md)操作。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-112">To get the replies for a message, use the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) operation.</span></span>

<span data-ttu-id="ad2f4-113">使用 delta 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="ad2f4-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="ad2f4-114">`nextLink`（包含具有 **delta** 函数调用和 `skipToken` 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="ad2f4-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="ad2f4-115">`deltaLink`（包含具有 **delta** 函数调用和 `deltaToken` 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="ad2f4-116">状态令牌对客户端完全不透明。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="ad2f4-117">若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 delta 函数调用即可。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="ad2f4-118">响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="ad2f4-119">可以保存 `deltaLink` URL，并在开始下一轮时使用。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-119">You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="ad2f4-120">有关详细信息，请参阅[增量查询](/graph/delta-query-overview)文档。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad2f4-121">权限</span><span class="sxs-lookup"><span data-stu-id="ad2f4-121">Permissions</span></span>

<span data-ttu-id="ad2f4-p106">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="ad2f4-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad2f4-124">Permission Type</span></span>                        |<span data-ttu-id="ad2f4-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad2f4-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="ad2f4-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad2f4-126">Delegated (work or school account)</span></span>| <span data-ttu-id="ad2f4-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad2f4-127">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="ad2f4-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad2f4-128">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad2f4-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-129">Not supported.</span></span>|
|<span data-ttu-id="ad2f4-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad2f4-130">Application</span></span>| <span data-ttu-id="ad2f4-131">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad2f4-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="ad2f4-132">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-132">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="ad2f4-133">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-133">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ad2f4-134">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-134">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ad2f4-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="ad2f4-136">查询参数</span><span class="sxs-lookup"><span data-stu-id="ad2f4-136">Query parameters</span></span>

<span data-ttu-id="ad2f4-137">跟踪频道消息更改会引发一组对 **delta** 函数的一次或多次调用。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-137">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="ad2f4-138">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-138">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="ad2f4-139">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-139">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="ad2f4-140">只需预先指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="ad2f4-141">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="ad2f4-142">查询参数</span><span class="sxs-lookup"><span data-stu-id="ad2f4-142">Query parameter</span></span>      | <span data-ttu-id="ad2f4-143">类型</span><span class="sxs-lookup"><span data-stu-id="ad2f4-143">Type</span></span>   |<span data-ttu-id="ad2f4-144">说明</span><span class="sxs-lookup"><span data-stu-id="ad2f4-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="ad2f4-145">string</span><span class="sxs-lookup"><span data-stu-id="ad2f4-145">string</span></span> | <span data-ttu-id="ad2f4-146">之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-146">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="ad2f4-147">将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-147">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="ad2f4-148">字符串</span><span class="sxs-lookup"><span data-stu-id="ad2f4-148">string</span></span> | <span data-ttu-id="ad2f4-149">上一个 **delta** 函数调用中的 `nextLink` URL 返回的 [状态令牌](/graph/delta-query-overview)，指示需要跟踪进一步的更改。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="ad2f4-150">OData 可选查询参数</span><span class="sxs-lookup"><span data-stu-id="ad2f4-150">Optional OData query parameters</span></span>

<span data-ttu-id="ad2f4-151">此 API 支持以下[ OData 查询参数](/graph/query-parameters)：</span><span class="sxs-lookup"><span data-stu-id="ad2f4-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="ad2f4-152">`$top`，表示在调用中获取的最大消息数。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-152">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="ad2f4-153">上限为 **50**。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-153">The upper limit is **50**.</span></span>
- <span data-ttu-id="ad2f4-154">`$skip`，表示列表开头要跳过的消息数。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="ad2f4-155">`$filter`，允许返回满足特定条件的消息。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-155">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="ad2f4-156">支持筛选的唯一属性是 `lastModifiedDateTime`，且仅支持 **gt** 运算符。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-156">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="ad2f4-157">例如，`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` 将提取指定日期时间后创建或更改的任何消息。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-157">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad2f4-158">请求头</span><span class="sxs-lookup"><span data-stu-id="ad2f4-158">Request headers</span></span>
| <span data-ttu-id="ad2f4-159">标头</span><span class="sxs-lookup"><span data-stu-id="ad2f4-159">Header</span></span>        | <span data-ttu-id="ad2f4-160">值</span><span class="sxs-lookup"><span data-stu-id="ad2f4-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="ad2f4-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad2f4-161">Authorization</span></span> | <span data-ttu-id="ad2f4-p112">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-p112">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad2f4-164">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad2f4-164">Content-Type</span></span>  | <span data-ttu-id="ad2f4-165">application/json</span><span class="sxs-lookup"><span data-stu-id="ad2f4-165">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ad2f4-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad2f4-166">Request Body</span></span>

<span data-ttu-id="ad2f4-167">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad2f4-168">响应</span><span class="sxs-lookup"><span data-stu-id="ad2f4-168">Response</span></span>

<span data-ttu-id="ad2f4-169">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-169">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="ad2f4-170">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-170">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="ad2f4-171">示例</span><span class="sxs-lookup"><span data-stu-id="ad2f4-171">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="ad2f4-172">示例 1：初始同步</span><span class="sxs-lookup"><span data-stu-id="ad2f4-172">Example 1: Initial synchronization</span></span>

<span data-ttu-id="ad2f4-173">以下示例显示了用于同步给定频道中消息的三个请求。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-173">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="ad2f4-174">频道中有五个消息。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-174">There are five messages in the channel.</span></span>

- <span data-ttu-id="ad2f4-175">第 1 步：[示例第一个请求](#initial-request)和[响应](#initial-request-response)。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-175">Step 1: [sample initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="ad2f4-176">第 2 步：[示例第二个请求](#second-request)和[响应](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="ad2f4-176">Step 2: [sample second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="ad2f4-177">第 3 步：[示例第三个请求](#third-request)和[最终响应](#third-request-response)。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-177">Step 3: [sample third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="ad2f4-p115">为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="ad2f4-180">另请了解[下一轮](#example-2-retrieving-additional-changes)该执行哪些操作。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-180">See also what you'll do in the [next round](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="ad2f4-181">初始请求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-181">Initial request</span></span>

<span data-ttu-id="ad2f4-182">本示例中，频道消息正在进行首次同步，因此初始同步请求未包含任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-182">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="ad2f4-183">这一轮将返回此日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-183">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="ad2f4-184">请求指定可选请求标头 odata.top，每次返回 2 个事件。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-184">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>



# <a name="http"></a>[<span data-ttu-id="ad2f4-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad2f4-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_1"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$top=2
```
# <a name="c"></a>[<span data-ttu-id="ad2f4-186">C#</span><span class="sxs-lookup"><span data-stu-id="ad2f4-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad2f4-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad2f4-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad2f4-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad2f4-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad2f4-189">Java</span><span class="sxs-lookup"><span data-stu-id="ad2f4-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="initial-request-response"></a><span data-ttu-id="ad2f4-190">第一个请求响应</span><span class="sxs-lookup"><span data-stu-id="ad2f4-190">Initial request response</span></span>

<span data-ttu-id="ad2f4-191">该响应包含两封邮件和一个具有 `skipToken` 的 `@odata.nextLink` 响应标头。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-191">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="ad2f4-192">`nextLink` URL 表示此频道中还更多邮件可获取。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-192">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="ad2f4-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad2f4-194">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-194">All the properties will be returned from an actual call.</span></span>
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

#### <a name="second-request"></a><span data-ttu-id="ad2f4-195">第二个请求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-195">Second request</span></span>

<span data-ttu-id="ad2f4-196">第二个请求指定上一个响应中返回的 `nextLink` URL。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-196">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="ad2f4-197">请注意，无需再像在第一个请求中一样指定相同的顶级参数，因为 `nextLink` URL 中的 `skipToken` 会将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-197">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad2f4-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad2f4-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_2"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="ad2f4-199">C#</span><span class="sxs-lookup"><span data-stu-id="ad2f4-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad2f4-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad2f4-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad2f4-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad2f4-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad2f4-202">Java</span><span class="sxs-lookup"><span data-stu-id="ad2f4-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="second-request-response"></a><span data-ttu-id="ad2f4-203">第二个请求响应</span><span class="sxs-lookup"><span data-stu-id="ad2f4-203">Second request response</span></span>

<span data-ttu-id="ad2f4-204">第二个响应返回接下来的 2 个消息和一个带有 `skipToken` 的 `@odata.nextLink` 响应标头，指示频道中存在可获取的更多消息。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-204">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

><span data-ttu-id="ad2f4-205">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-205">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad2f4-206">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-206">All the properties will be returned from an actual call.</span></span>
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

#### <a name="third-request"></a><span data-ttu-id="ad2f4-207">第三个请求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-207">Third request</span></span>

<span data-ttu-id="ad2f4-208">第三个请求继续使用上一个同步请求返回的最新 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-208">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>



# <a name="http"></a>[<span data-ttu-id="ad2f4-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad2f4-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_3"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$skiptoken=c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="ad2f4-210">C#</span><span class="sxs-lookup"><span data-stu-id="ad2f4-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad2f4-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad2f4-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad2f4-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad2f4-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad2f4-213">Java</span><span class="sxs-lookup"><span data-stu-id="ad2f4-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="third-request-response"></a><span data-ttu-id="ad2f4-214">第三个请求响应</span><span class="sxs-lookup"><span data-stu-id="ad2f4-214">Third request response</span></span>

<span data-ttu-id="ad2f4-215">第三个响应仅返回频道中剩下的消息以及带有 `deltaToken` 的 `@odata.deltaLink` 响应标头，指示频道中的所有消息已被阅读。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-215">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="ad2f4-216">保存并使用 `deltaLink` URL，以便查询下一轮中从此点开始的任何新消息。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-216">Save and use the `deltaLink` URL to query for any new messages starting from this point in the next round.</span></span>

><span data-ttu-id="ad2f4-217">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-217">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad2f4-218">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-218">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="ad2f4-219">示例 2：检索其他更改</span><span class="sxs-lookup"><span data-stu-id="ad2f4-219">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="ad2f4-220">使用上一轮中最后一个请求返回的 `deltaLink`，可以只获取从那以后此频道中发生变化（已添加或更新）的邮件。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-220">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="ad2f4-221">假如你更喜欢在响应中保持最大页面的同一大小，则请求将如下所示：</span><span class="sxs-lookup"><span data-stu-id="ad2f4-221">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="ad2f4-222">请求</span><span class="sxs-lookup"><span data-stu-id="ad2f4-222">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="ad2f4-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad2f4-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel_messages_delta_4"
}-->
```msgraph-interactive
GET /teams/{id}/channels/{id}/messages/delta?$deltatoken=c3RhcnRUaW1lPTE1NTEyODc1ODA0OTAmcGFnZVNpemU9MjA%3d
```
# <a name="c"></a>[<span data-ttu-id="ad2f4-224">C#</span><span class="sxs-lookup"><span data-stu-id="ad2f4-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-delta-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad2f4-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad2f4-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-delta-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad2f4-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad2f4-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-delta-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad2f4-227">Java</span><span class="sxs-lookup"><span data-stu-id="ad2f4-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-delta-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="ad2f4-228">响应</span><span class="sxs-lookup"><span data-stu-id="ad2f4-228">Response</span></span>

><span data-ttu-id="ad2f4-p124">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad2f4-p124">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


