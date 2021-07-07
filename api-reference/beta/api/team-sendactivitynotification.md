---
title: team：sendActivityNotification
description: 在团队范围内发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 81b081ddf045cc1406903bd7d9b88edffc05480d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317123"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="ef0a7-103">team：sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="ef0a7-103">team: sendActivityNotification</span></span>
<span data-ttu-id="ef0a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef0a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef0a7-105">在团队范围内发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="ef0a7-106">有关发送通知的更多详细信息以及发送通知的要求，请参阅[发送Teams活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef0a7-107">权限</span><span class="sxs-lookup"><span data-stu-id="ef0a7-107">Permissions</span></span>
<span data-ttu-id="ef0a7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef0a7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef0a7-110">Permission type</span></span>|<span data-ttu-id="ef0a7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef0a7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef0a7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef0a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef0a7-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="ef0a7-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="ef0a7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef0a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef0a7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-115">Not Supported.</span></span>|
|<span data-ttu-id="ef0a7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef0a7-116">Application</span></span>|<span data-ttu-id="ef0a7-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="ef0a7-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef0a7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="ef0a7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef0a7-119">Request headers</span></span>
|<span data-ttu-id="ef0a7-120">名称</span><span class="sxs-lookup"><span data-stu-id="ef0a7-120">Name</span></span>|<span data-ttu-id="ef0a7-121">说明</span><span class="sxs-lookup"><span data-stu-id="ef0a7-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef0a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef0a7-122">Authorization</span></span>|<span data-ttu-id="ef0a7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ef0a7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef0a7-125">Content-Type</span></span>|<span data-ttu-id="ef0a7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ef0a7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef0a7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef0a7-128">Request body</span></span>
<span data-ttu-id="ef0a7-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ef0a7-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ef0a7-131">参数</span><span class="sxs-lookup"><span data-stu-id="ef0a7-131">Parameter</span></span>|<span data-ttu-id="ef0a7-132">类型</span><span class="sxs-lookup"><span data-stu-id="ef0a7-132">Type</span></span>|<span data-ttu-id="ef0a7-133">说明</span><span class="sxs-lookup"><span data-stu-id="ef0a7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef0a7-134">topic</span><span class="sxs-lookup"><span data-stu-id="ef0a7-134">topic</span></span>|[<span data-ttu-id="ef0a7-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="ef0a7-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="ef0a7-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-136">Topic of the notification.</span></span> <span data-ttu-id="ef0a7-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="ef0a7-138">activityType</span><span class="sxs-lookup"><span data-stu-id="ef0a7-138">activityType</span></span>|<span data-ttu-id="ef0a7-139">String</span><span class="sxs-lookup"><span data-stu-id="ef0a7-139">String</span></span>|<span data-ttu-id="ef0a7-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-140">Activity type.</span></span> <span data-ttu-id="ef0a7-141">这必须在应用清单[Teams声明](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="ef0a7-142">chainId</span><span class="sxs-lookup"><span data-stu-id="ef0a7-142">chainId</span></span>|<span data-ttu-id="ef0a7-143">Int64</span><span class="sxs-lookup"><span data-stu-id="ef0a7-143">Int64</span></span>|<span data-ttu-id="ef0a7-144">可选。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-144">Optional.</span></span> <span data-ttu-id="ef0a7-145">用于替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-145">Used to override a previous notification.</span></span> <span data-ttu-id="ef0a7-146">在后续 `chainId` 请求中使用相同的方法替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="ef0a7-147">previewText</span><span class="sxs-lookup"><span data-stu-id="ef0a7-147">previewText</span></span>|[<span data-ttu-id="ef0a7-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="ef0a7-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="ef0a7-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-149">Preview text for the notification.</span></span> <span data-ttu-id="ef0a7-150">Microsoft Teams显示前 150 个字符。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="ef0a7-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="ef0a7-151">templateParameters</span></span>|<span data-ttu-id="ef0a7-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef0a7-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="ef0a7-153">活动源条目中定义的模板变量的值与应用程序Teams `activityType` [相对应](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="ef0a7-154">recipient</span><span class="sxs-lookup"><span data-stu-id="ef0a7-154">recipient</span></span>|[<span data-ttu-id="ef0a7-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="ef0a7-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="ef0a7-156">通知的收件人。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-156">Recipient of the notification.</span></span> <span data-ttu-id="ef0a7-157">另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) [、teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md)和 [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md), [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md), and [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="ef0a7-158">将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityUrl` ：</span><span class="sxs-lookup"><span data-stu-id="ef0a7-158">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="ef0a7-159">团队</span><span class="sxs-lookup"><span data-stu-id="ef0a7-159">team</span></span>](../resources/team.md)
- [<span data-ttu-id="ef0a7-160">频道</span><span class="sxs-lookup"><span data-stu-id="ef0a7-160">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="ef0a7-161">chatMesage</span><span class="sxs-lookup"><span data-stu-id="ef0a7-161">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="ef0a7-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ef0a7-162">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="ef0a7-163">**注意：** 实体 URL 必须相同或 URL 中团队的子资源。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-163">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="ef0a7-164">此外[，Teams](/microsoftteams/platform/overview)应用必须安装在团队中。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-164">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="ef0a7-165">响应</span><span class="sxs-lookup"><span data-stu-id="ef0a7-165">Response</span></span>

<span data-ttu-id="ef0a7-166">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-166">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ef0a7-167">示例</span><span class="sxs-lookup"><span data-stu-id="ef0a7-167">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="ef0a7-168">示例 1：通知用户有关待处理的财务审批请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-168">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="ef0a7-169">此示例演示如何发送团队的活动源通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-169">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="ef0a7-170">此示例通知团队所有者有关待处理的财务审批请求。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-170">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="ef0a7-171">请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef0a7-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0a7-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_1"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="javascript"></a>[<span data-ttu-id="ef0a7-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef0a7-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ef0a7-174">C#</span><span class="sxs-lookup"><span data-stu-id="ef0a7-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef0a7-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef0a7-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef0a7-176">Java</span><span class="sxs-lookup"><span data-stu-id="ef0a7-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef0a7-177">响应</span><span class="sxs-lookup"><span data-stu-id="ef0a7-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="ef0a7-178">示例 2：通知用户有关频道选项卡的信息</span><span class="sxs-lookup"><span data-stu-id="ef0a7-178">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="ef0a7-179">与上一示例类似，此示例对 `entityUrl` 使用 `topic` 。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-179">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="ef0a7-180">但是，此示例[链接到频道中的](../resources/teamstab.md)[选项卡](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-180">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="ef0a7-181">选项卡承载一个页面，向用户显示其酒店预订的状态。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-181">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="ef0a7-182">选择通知后，用户即可访问选项卡，可在其中查看预订。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-182">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="ef0a7-183">请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-183">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef0a7-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0a7-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "reservationId",
            "value": "TREEE433"
        },
        {
            "name": "currentSlot",
            "value": "23"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="ef0a7-185">C#</span><span class="sxs-lookup"><span data-stu-id="ef0a7-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef0a7-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef0a7-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef0a7-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef0a7-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef0a7-188">Java</span><span class="sxs-lookup"><span data-stu-id="ef0a7-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef0a7-189">响应</span><span class="sxs-lookup"><span data-stu-id="ef0a7-189">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="ef0a7-190">示例 3：使用自定义主题通知用户事件</span><span class="sxs-lookup"><span data-stu-id="ef0a7-190">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="ef0a7-191">如前面的示例中所示，你可以链接到团队的不同方面。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-191">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="ef0a7-192">但是，如果要链接到不是团队的一部分或不是由 Microsoft Graph 表示的方面，或者希望自定义名称，可以将 的源设置为 并传递其自定义 `topic` `text` 值。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-192">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="ef0a7-193">`webUrl` 将 source 设置为 时 `topic` 是必需的 `text` 。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-193">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="ef0a7-194">请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef0a7-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0a7-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_3"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="ef0a7-196">C#</span><span class="sxs-lookup"><span data-stu-id="ef0a7-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef0a7-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef0a7-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef0a7-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef0a7-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef0a7-199">Java</span><span class="sxs-lookup"><span data-stu-id="ef0a7-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef0a7-200">响应</span><span class="sxs-lookup"><span data-stu-id="ef0a7-200">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-pending-finance-approval-requests"></a><span data-ttu-id="ef0a7-201">示例 4：通知团队成员有关待处理的财务审批请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-201">Example 4: Notify the team members about pending finance approval requests</span></span>

<span data-ttu-id="ef0a7-202">此示例演示如何向所有团队成员发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-202">This example shows how you can send an activity feed notification to all team members.</span></span> <span data-ttu-id="ef0a7-203">此示例与前面的示例类似。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-203">This example is similar to previous examples.</span></span> <span data-ttu-id="ef0a7-204">但是，在这种情况下， 是 `recipient` [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-204">However, in this case, the `recipient` is a [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span></span> <span data-ttu-id="ef0a7-205">请注意， `teamId` 中指定的 `recipient` 必须与请求 URL `teamId` 中指定的 匹配。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-205">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

> <span data-ttu-id="ef0a7-206">**注意：** 向所有团队成员发送通知的能力仅限于拥有 10，000 个成员或更少成员的团队。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-206">**Note:** The ability to send notifications to all team members is limited to teams with 10,000 members or less.</span></span> <span data-ttu-id="ef0a7-207">如果团队超过 10，000 个成员，则任何团队成员均不会收到通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-207">If the team exceeds 10,000 members, none of the team members will receive a notification.</span></span>

#### <a name="request"></a><span data-ttu-id="ef0a7-208">请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-208">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef0a7-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0a7-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.teamMembersNotificationRecipient",
        "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="ef0a7-210">C#</span><span class="sxs-lookup"><span data-stu-id="ef0a7-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef0a7-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef0a7-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef0a7-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef0a7-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef0a7-213">Java</span><span class="sxs-lookup"><span data-stu-id="ef0a7-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef0a7-214">响应</span><span class="sxs-lookup"><span data-stu-id="ef0a7-214">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-pending-finance-approval-requests"></a><span data-ttu-id="ef0a7-215">示例 5：通知频道成员有关待处理的财务审批请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-215">Example 5: Notify the channel members about pending finance approval requests</span></span>

<span data-ttu-id="ef0a7-216">此示例演示如何向所有频道成员发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-216">This example shows how you can send an activity feed notification to all channel members.</span></span> <span data-ttu-id="ef0a7-217">此示例与上一个示例类似。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-217">This example is similar to the previous example.</span></span> <span data-ttu-id="ef0a7-218">但是，在这种情况下， 是 `recipient` [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-218">However, in this case, the `recipient` is a [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> <span data-ttu-id="ef0a7-219">请注意， `teamId` 中指定的 `recipient` 必须与请求 URL `teamId` 中指定的 匹配。</span><span class="sxs-lookup"><span data-stu-id="ef0a7-219">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="ef0a7-220">请求</span><span class="sxs-lookup"><span data-stu-id="ef0a7-220">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef0a7-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0a7-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_5"
}
-->

``` http
POST https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
        "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
        "channelId": "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="ef0a7-222">C#</span><span class="sxs-lookup"><span data-stu-id="ef0a7-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef0a7-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef0a7-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef0a7-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef0a7-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef0a7-225">Java</span><span class="sxs-lookup"><span data-stu-id="ef0a7-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef0a7-226">响应</span><span class="sxs-lookup"><span data-stu-id="ef0a7-226">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
