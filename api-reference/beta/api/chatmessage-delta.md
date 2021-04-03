---
title: chatMessage：delta
description: 检索团队频道中的消息列表（无回复）。 通过使用增量查询，可以获取频道中新的或更新的消息。
localization_priority: Priority
doc_type: apiPageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e24106814dac97a8585245a48a3f1641c98188d7
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582681"
---
# <a name="chatmessage-delta"></a><span data-ttu-id="b2059-104">chatMessage：delta</span><span class="sxs-lookup"><span data-stu-id="b2059-104">chatMessage: delta</span></span>

<span data-ttu-id="b2059-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2059-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2059-106">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="b2059-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="b2059-107">通过使用增量查询，可以获取频道中新的或更新的消息。</span><span class="sxs-lookup"><span data-stu-id="b2059-107">By using delta query, you can get new or updated messages in a channel.</span></span>

> <span data-ttu-id="b2059-108">**请注意：** 增量查询将仅返回过去 8 个月内的邮件。</span><span class="sxs-lookup"><span data-stu-id="b2059-108">**Note:** Delta will only return messages within the last eight months.</span></span> <span data-ttu-id="b2059-109">要检索时间更早的邮件，可使用 [GET /teams/{team-id}/channels/{channel-id}/messages](channel-list-messages.md)。</span><span class="sxs-lookup"><span data-stu-id="b2059-109">You can use [GET /teams/{team-id}/channels/{channel-id}/messages](channel-list-messages.md) to retrieve older messages.</span></span>

<span data-ttu-id="b2059-110">增量查询既支持可检索指定频道中的所有消息的完全同步，也支持可检索自上次同步后频道中添加或发生变化的消息的增量同步。</span><span class="sxs-lookup"><span data-stu-id="b2059-110">Delta query supports both full synchronization that retrieves all the messages in the specified channel, and incremental synchronization that retrieves those messages that have been added or changed in the channel since the last synchronization.</span></span> <span data-ttu-id="b2059-111">通常情况下，开始时会执行一次完全同步，随后会定期获取相应消息视图的增量更改。</span><span class="sxs-lookup"><span data-stu-id="b2059-111">Typically, you would do an initial full synchronization, and then get incremental changes to that messages view periodically.</span></span>

<span data-ttu-id="b2059-112">若要获取消息的回复，请使用[列出消息回复](chatmessage-list-replies.md)或[获取消息回复](chatmessage-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="b2059-112">To get the replies for a message, use the [list message replies](chatmessage-list-replies.md) or the [get message reply](chatmessage-get.md) operation.</span></span>

<span data-ttu-id="b2059-113">使用 delta 函数的 GET 请求返回以下任一内容：</span><span class="sxs-lookup"><span data-stu-id="b2059-113">A GET request with the delta function returns either:</span></span>

- <span data-ttu-id="b2059-114">`nextLink`（包含具有 **delta** 函数调用和 `skipToken` 的 URL），或</span><span class="sxs-lookup"><span data-stu-id="b2059-114">A `nextLink` (that contains a URL with a **delta** function call and a `skipToken`), or</span></span>
- <span data-ttu-id="b2059-115">`deltaLink`（包含具有 **delta** 函数调用和 `deltaToken` 的 URL）。</span><span class="sxs-lookup"><span data-stu-id="b2059-115">A `deltaLink` (that contains a URL with a **delta** function call and `deltaToken`).</span></span>

<span data-ttu-id="b2059-116">状态令牌对客户端完全不透明。</span><span class="sxs-lookup"><span data-stu-id="b2059-116">State tokens are completely opaque to the client.</span></span> <span data-ttu-id="b2059-117">若要继续一轮事件更改跟踪，只需将最后一个 GET 请求返回的 `nextLink` 或 `deltaLink` URL 复制并应用到同一日历视图的下一个 delta 函数调用即可。</span><span class="sxs-lookup"><span data-stu-id="b2059-117">To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next delta function call for that same calendar view.</span></span> <span data-ttu-id="b2059-118">响应中返回的 `deltaLink` 表示当前一轮更改跟踪已完成。</span><span class="sxs-lookup"><span data-stu-id="b2059-118">A `deltaLink` returned in a response signifies that the current round of change tracking is complete.</span></span> <span data-ttu-id="b2059-119">开始检索其他更改（获取`deltaLink` 后更改或发布的消息）时，可以保存并使用 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="b2059-119">You can save and use the `deltaLink` URL when you begin the to retrieve additional changes (messages changed or posted after acquiring `deltaLink`).</span></span>

<span data-ttu-id="b2059-120">有关详细信息，请参阅[增量查询](/graph/delta-query-overview)文档。</span><span class="sxs-lookup"><span data-stu-id="b2059-120">For more information, see the [delta query](/graph/delta-query-overview) documentation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2059-121">权限</span><span class="sxs-lookup"><span data-stu-id="b2059-121">Permissions</span></span>

<span data-ttu-id="b2059-p106">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b2059-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="b2059-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2059-124">Permission Type</span></span>                        |<span data-ttu-id="b2059-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2059-125">Permissions (from least to most privileged)</span></span>  |
|---------------------------------------|---------------------------------------------|
|<span data-ttu-id="b2059-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2059-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2059-127">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2059-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="b2059-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2059-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2059-129">不支持</span><span class="sxs-lookup"><span data-stu-id="b2059-129">Not Supported</span></span>                                |
|<span data-ttu-id="b2059-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2059-130">Application</span></span>                            | <span data-ttu-id="b2059-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2059-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="b2059-132">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="b2059-132">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="b2059-133">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="b2059-133">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="b2059-134">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="b2059-134">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="b2059-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2059-135">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="b2059-136">查询参数</span><span class="sxs-lookup"><span data-stu-id="b2059-136">Query parameters</span></span>

<span data-ttu-id="b2059-137">跟踪频道消息更改会引发一组对 **delta** 函数的一次或多次调用。</span><span class="sxs-lookup"><span data-stu-id="b2059-137">Tracking changes in channel messages incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="b2059-138">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="b2059-138">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="b2059-139">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="b2059-139">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="b2059-140">只需预先指定任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="b2059-140">You only need to specify any query parameters once upfront.</span></span>

<span data-ttu-id="b2059-141">在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含编码参数。</span><span class="sxs-lookup"><span data-stu-id="b2059-141">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="b2059-142">查询参数</span><span class="sxs-lookup"><span data-stu-id="b2059-142">Query parameter</span></span>      | <span data-ttu-id="b2059-143">类型</span><span class="sxs-lookup"><span data-stu-id="b2059-143">Type</span></span>   |<span data-ttu-id="b2059-144">说明</span><span class="sxs-lookup"><span data-stu-id="b2059-144">Description</span></span>|
|:---------------|:--------|:----------|
| `$deltatoken` | <span data-ttu-id="b2059-145">string</span><span class="sxs-lookup"><span data-stu-id="b2059-145">string</span></span> | <span data-ttu-id="b2059-146">之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。</span><span class="sxs-lookup"><span data-stu-id="b2059-146">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="b2059-147">将此令牌包含在对该集合的下一个更改追踪迭代的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="b2059-147">Save and apply the entire `deltaLink` URL including this token in the first request of the next iteration of change tracking for that collection.</span></span>|
| `$skiptoken` | <span data-ttu-id="b2059-148">字符串</span><span class="sxs-lookup"><span data-stu-id="b2059-148">string</span></span> | <span data-ttu-id="b2059-149">上一个 **delta** 函数调用中的 `nextLink` URL 返回的 [状态令牌](/graph/delta-query-overview)，指示需要跟踪进一步的更改。</span><span class="sxs-lookup"><span data-stu-id="b2059-149">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating that there are further changes to be tracked.</span></span> |

### <a name="optional-odata-query-parameters"></a><span data-ttu-id="b2059-150">OData 可选查询参数</span><span class="sxs-lookup"><span data-stu-id="b2059-150">Optional OData query parameters</span></span>

<span data-ttu-id="b2059-151">此 API 支持以下[ OData 查询参数](/graph/query-parameters)：</span><span class="sxs-lookup"><span data-stu-id="b2059-151">The following [OData query parameters](/graph/query-parameters) are supported by this API:</span></span>
- <span data-ttu-id="b2059-152">`$top`，表示在调用中获取的最大消息数。</span><span class="sxs-lookup"><span data-stu-id="b2059-152">`$top`, represents maximum number of messages to fetch in a call.</span></span> <span data-ttu-id="b2059-153">上限为 **50**。</span><span class="sxs-lookup"><span data-stu-id="b2059-153">The upper limit is **50**.</span></span>
- <span data-ttu-id="b2059-154">`$skip`，表示列表开头要跳过的消息数。</span><span class="sxs-lookup"><span data-stu-id="b2059-154">`$skip`, represents how many messages to skip at the beginning of the list.</span></span>
- <span data-ttu-id="b2059-155">`$filter`，允许返回满足特定条件的消息。</span><span class="sxs-lookup"><span data-stu-id="b2059-155">`$filter` allows returning messages that meet a certain criteria.</span></span> <span data-ttu-id="b2059-156">支持筛选的唯一属性是 `lastModifiedDateTime`，且仅支持 **gt** 运算符。</span><span class="sxs-lookup"><span data-stu-id="b2059-156">The only property that supports filtering is `lastModifiedDateTime`, and only the **gt** operator is supported.</span></span> <span data-ttu-id="b2059-157">例如，`../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` 将提取指定日期时间后创建或更改的任何消息。</span><span class="sxs-lookup"><span data-stu-id="b2059-157">For example, `../messages/delta?$filter=lastModifiedDateTime gt 2019-02-27T07:13:28.000z` will fetch any messages created or changed after the specified date time.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2059-158">请求头</span><span class="sxs-lookup"><span data-stu-id="b2059-158">Request headers</span></span>
| <span data-ttu-id="b2059-159">标头</span><span class="sxs-lookup"><span data-stu-id="b2059-159">Header</span></span>        | <span data-ttu-id="b2059-160">值</span><span class="sxs-lookup"><span data-stu-id="b2059-160">Value</span></span>                     |
|---------------|---------------------------|
| <span data-ttu-id="b2059-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2059-161">Authorization</span></span> | <span data-ttu-id="b2059-p112">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2059-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2059-164">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2059-164">Request Body</span></span>

<span data-ttu-id="b2059-165">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2059-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2059-166">响应</span><span class="sxs-lookup"><span data-stu-id="b2059-166">Response</span></span>

<span data-ttu-id="b2059-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b2059-167">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span> <span data-ttu-id="b2059-168">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="b2059-168">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

## <a name="examples"></a><span data-ttu-id="b2059-169">示例</span><span class="sxs-lookup"><span data-stu-id="b2059-169">Examples</span></span>

### <a name="example-1-initial-synchronization"></a><span data-ttu-id="b2059-170">示例 1：初始同步</span><span class="sxs-lookup"><span data-stu-id="b2059-170">Example 1: Initial synchronization</span></span>

<span data-ttu-id="b2059-171">以下示例显示了用于同步给定频道中消息的三个请求。</span><span class="sxs-lookup"><span data-stu-id="b2059-171">The following example shows a series of three requests to synchronize the messages in the given channel.</span></span> <span data-ttu-id="b2059-172">频道中有五个消息。</span><span class="sxs-lookup"><span data-stu-id="b2059-172">There are five messages in the channel.</span></span>

- <span data-ttu-id="b2059-173">步骤 1：[初始请求](#initial-request)和[响应](#initial-request-response)。</span><span class="sxs-lookup"><span data-stu-id="b2059-173">Step 1: [initial request](#initial-request) and [response](#initial-request-response).</span></span>
- <span data-ttu-id="b2059-174">步骤 2：[第二个请求](#second-request)和[响应](#second-request-response)</span><span class="sxs-lookup"><span data-stu-id="b2059-174">Step 2: [second request](#second-request) and [response](#second-request-response)</span></span>
- <span data-ttu-id="b2059-175">步骤 3：[第三个请求](#third-request)和[最终响应](#third-request-response)。</span><span class="sxs-lookup"><span data-stu-id="b2059-175">Step 3: [third request](#third-request) and [final response](#third-request-response).</span></span>

<span data-ttu-id="b2059-p115">为简洁起见，示例响应仅显示一部分事件属性。在实际调用中，大多数事件属性都会返回。</span><span class="sxs-lookup"><span data-stu-id="b2059-p115">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span>

<span data-ttu-id="b2059-178">另请参见如何[检索其他更改](#example-2-retrieving-additional-changes)。</span><span class="sxs-lookup"><span data-stu-id="b2059-178">See also what you'll do [to retrieve additional changes](#example-2-retrieving-additional-changes).</span></span>

#### <a name="initial-request"></a><span data-ttu-id="b2059-179">初始请求</span><span class="sxs-lookup"><span data-stu-id="b2059-179">Initial request</span></span>

<span data-ttu-id="b2059-180">本示例中，频道消息正在进行首次同步，因此初始同步请求未包含任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="b2059-180">In this example, the channel messages are being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="b2059-181">这一轮将返回此日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="b2059-181">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="b2059-182">请求指定可选请求标头 odata.top，每次返回 2 个事件。</span><span class="sxs-lookup"><span data-stu-id="b2059-182">The request specifies the optional request header, odata.top, returning 2 events at a time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_1"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$top=2
```

#### <a name="initial-request-response"></a><span data-ttu-id="b2059-183">第一个请求响应</span><span class="sxs-lookup"><span data-stu-id="b2059-183">Initial request response</span></span>

<span data-ttu-id="b2059-184">该响应包含两封邮件和一个具有 `skipToken` 的 `@odata.nextLink` 响应标头。</span><span class="sxs-lookup"><span data-stu-id="b2059-184">The response includes two messages and a `@odata.nextLink` response header with a `skipToken`.</span></span> <span data-ttu-id="b2059-185">`nextLink` URL 表示此频道中还更多邮件可获取。</span><span class="sxs-lookup"><span data-stu-id="b2059-185">The `nextLink` URL indicates there are more messages in the channel to get.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606515483514",
            "messageType": "message",
            "createdDateTime": "2020-11-27T22:18:03.514Z",
            "lastModifiedDateTime": "2020-11-27T22:18:03.514Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606515483514?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606515483514&parentMessageId=1606515483514",
            "policyViolation": null,
            "id": "1606515483514",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691795113",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:16:35.113Z",
            "lastModifiedDateTime": "2020-11-29T23:16:35.113Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691795113?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691795113&parentMessageId=1606691795113",
            "policyViolation": null,
            "id": "1606691795113",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 11/29/2020 3:16:31 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

#### <a name="second-request"></a><span data-ttu-id="b2059-186">第二个请求</span><span class="sxs-lookup"><span data-stu-id="b2059-186">Second request</span></span>

<span data-ttu-id="b2059-187">第二个请求指定上一个响应中返回的 `nextLink` URL。</span><span class="sxs-lookup"><span data-stu-id="b2059-187">The second request specifies the `nextLink` URL returned from the previous response.</span></span> <span data-ttu-id="b2059-188">请注意，无需再像在第一个请求中一样指定相同的顶级参数，因为 `nextLink` URL 中的 `skipToken` 会将其编码并包含在内。</span><span class="sxs-lookup"><span data-stu-id="b2059-188">Notice that it no longer has to specify the same top parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_2"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58
```

#### <a name="second-request-response"></a><span data-ttu-id="b2059-189">第二个请求响应</span><span class="sxs-lookup"><span data-stu-id="b2059-189">Second request response</span></span>

<span data-ttu-id="b2059-190">第二个响应返回接下来的 2 个消息和一个带有 `skipToken` 的 `@odata.nextLink` 响应标头，指示频道中存在可获取的更多消息。</span><span class="sxs-lookup"><span data-stu-id="b2059-190">The second response returns the next 2 messages and a `@odata.nextLink` response header with a `skipToken`, indicates there are more messages in the channel to get.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691812117",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:16:52.117Z",
            "lastModifiedDateTime": "2020-11-29T23:16:52.117Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691812117?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691812117&parentMessageId=1606691812117",
            "policyViolation": null,
            "id": "1606691812117",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 11/29/2020 3:16:51 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1606691846203",
            "messageType": "message",
            "createdDateTime": "2020-11-29T23:17:26.203Z",
            "lastModifiedDateTime": "2020-11-29T23:17:26.203Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1606691846203?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1606691846203&parentMessageId=1606691846203",
            "policyViolation": null,
            "id": "1606691846203",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 11/29/2020 3:17:25 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

#### <a name="third-request"></a><span data-ttu-id="b2059-191">第三个请求</span><span class="sxs-lookup"><span data-stu-id="b2059-191">Third request</span></span>

<span data-ttu-id="b2059-192">第三个请求继续使用上一个同步请求返回的最新 `nextLink`。</span><span class="sxs-lookup"><span data-stu-id="b2059-192">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_3"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$skiptoken=8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4
```

#### <a name="third-request-response"></a><span data-ttu-id="b2059-193">第三个请求响应</span><span class="sxs-lookup"><span data-stu-id="b2059-193">Third request response</span></span>

<span data-ttu-id="b2059-194">第三个响应仅返回频道中剩下的消息以及带有 `deltaToken` 的 `@odata.deltaLink` 响应标头，指示频道中的所有消息已被阅读。</span><span class="sxs-lookup"><span data-stu-id="b2059-194">The third response returns the only remaining messages in the channel and a `@odata.deltaLink` response header with a `deltaToken` which indicates that all messages in the channel have been read.</span></span> <span data-ttu-id="b2059-195">保存并使用 `deltaLink` URL，查询从此点开始的任何新消息。</span><span class="sxs-lookup"><span data-stu-id="b2059-195">Save and use the `deltaLink` URL to query for any new messages starting from this point onwards.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1611351582080",
            "messageType": "message",
            "createdDateTime": "2021-01-22T21:39:42.08Z",
            "lastModifiedDateTime": "2021-01-22T21:39:42.08Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1611351582080?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1611351582080&parentMessageId=1611351582080",
            "policyViolation": null,
            "id": "1611351582080",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 1/22/2021 1:39:39 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1611351603178",
            "messageType": "message",
            "createdDateTime": "2021-01-22T21:40:03.178Z",
            "lastModifiedDateTime": "2021-01-22T21:40:03.178Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1611351603178?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1611351603178&parentMessageId=1611351603178",
            "policyViolation": null,
            "id": "1611351603178",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "HelloWorld 1/22/2021 1:40:00 PM -08:00"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

### <a name="example-2-retrieving-additional-changes"></a><span data-ttu-id="b2059-196">示例 2：检索其他更改</span><span class="sxs-lookup"><span data-stu-id="b2059-196">Example 2: Retrieving additional changes</span></span>

<span data-ttu-id="b2059-197">使用上一轮中最后一个请求返回的 `deltaLink`，可以只获取从那以后此频道中发生变化（已添加或更新）的邮件。</span><span class="sxs-lookup"><span data-stu-id="b2059-197">Using the `deltaLink` from the last request in the last round, you will be able to get only those messages that have changed (by being added, or updated) in that channel since then.</span></span> <span data-ttu-id="b2059-198">假如你更喜欢在响应中保持最大页面的同一大小，则请求将如下所示：</span><span class="sxs-lookup"><span data-stu-id="b2059-198">Your request will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>

#### <a name="request"></a><span data-ttu-id="b2059-199">请求</span><span class="sxs-lookup"><span data-stu-id="b2059-199">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagedeltachannel_4"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4
```

#### <a name="response"></a><span data-ttu-id="b2059-200">响应</span><span class="sxs-lookup"><span data-stu-id="b2059-200">Response</span></span>

><span data-ttu-id="b2059-p121">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b2059-p121">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta?$deltatoken=aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_yjz2nsMoh1gXNtXii7s78HapCi5woifXqwXlVNxICh8wUUnvE2gExsa8eZ2Vy_ch5rVIhm067_1mUPML3iYUVyg.3o0rhgaBUduuxOr98An5pjBDP5JjKUiVWku3flSiOsk",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "replyToId": null,
            "etag": "1616989510408",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:45:10.408Z",
            "lastModifiedDateTime": "2021-03-29T03:45:10.408Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989510408?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989510408&parentMessageId=1616989510408",
            "policyViolation": null,
            "id": "1616989510408",
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Hello World 28th March 2021"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
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


