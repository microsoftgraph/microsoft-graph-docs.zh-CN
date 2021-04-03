---
title: team：sendActivityNotification
description: 在团队范围内发送活动源通知。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: add05d086580d5ed76b4195de98d28187e3ad30d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507562"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="d585b-103">team：sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="d585b-103">team: sendActivityNotification</span></span>
<span data-ttu-id="d585b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d585b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d585b-105">在团队范围内发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="d585b-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="d585b-106">有关发送通知的更多详细信息以及发送通知的要求，请参阅 [发送 Teams 活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="d585b-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="d585b-107">权限</span><span class="sxs-lookup"><span data-stu-id="d585b-107">Permissions</span></span>
<span data-ttu-id="d585b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d585b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d585b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d585b-110">Permission type</span></span>|<span data-ttu-id="d585b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d585b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d585b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d585b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d585b-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="d585b-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="d585b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d585b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d585b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d585b-115">Not Supported.</span></span>|
|<span data-ttu-id="d585b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d585b-116">Application</span></span>|<span data-ttu-id="d585b-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="d585b-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="d585b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d585b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="d585b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d585b-119">Request headers</span></span>
|<span data-ttu-id="d585b-120">名称</span><span class="sxs-lookup"><span data-stu-id="d585b-120">Name</span></span>|<span data-ttu-id="d585b-121">说明</span><span class="sxs-lookup"><span data-stu-id="d585b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d585b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d585b-122">Authorization</span></span>|<span data-ttu-id="d585b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d585b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d585b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d585b-125">Content-Type</span></span>|<span data-ttu-id="d585b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d585b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d585b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d585b-128">Request body</span></span>
<span data-ttu-id="d585b-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d585b-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d585b-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d585b-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d585b-131">参数</span><span class="sxs-lookup"><span data-stu-id="d585b-131">Parameter</span></span>|<span data-ttu-id="d585b-132">类型</span><span class="sxs-lookup"><span data-stu-id="d585b-132">Type</span></span>|<span data-ttu-id="d585b-133">说明</span><span class="sxs-lookup"><span data-stu-id="d585b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d585b-134">topic</span><span class="sxs-lookup"><span data-stu-id="d585b-134">topic</span></span>|[<span data-ttu-id="d585b-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="d585b-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="d585b-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="d585b-136">Topic of the notification.</span></span> <span data-ttu-id="d585b-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="d585b-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="d585b-138">activityType</span><span class="sxs-lookup"><span data-stu-id="d585b-138">activityType</span></span>|<span data-ttu-id="d585b-139">String</span><span class="sxs-lookup"><span data-stu-id="d585b-139">String</span></span>|<span data-ttu-id="d585b-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="d585b-140">Activity type.</span></span> <span data-ttu-id="d585b-141">这必须在 Teams 应用清单 [中声明](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="d585b-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="d585b-142">chainId</span><span class="sxs-lookup"><span data-stu-id="d585b-142">chainId</span></span>|<span data-ttu-id="d585b-143">Int64</span><span class="sxs-lookup"><span data-stu-id="d585b-143">Int64</span></span>|<span data-ttu-id="d585b-144">可选。</span><span class="sxs-lookup"><span data-stu-id="d585b-144">Optional.</span></span> <span data-ttu-id="d585b-145">用于替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="d585b-145">Used to override a previous notification.</span></span> <span data-ttu-id="d585b-146">在后续 `chainId` 请求中使用相同的方法替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="d585b-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="d585b-147">previewText</span><span class="sxs-lookup"><span data-stu-id="d585b-147">previewText</span></span>|[<span data-ttu-id="d585b-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="d585b-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="d585b-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="d585b-149">Preview text for the notification.</span></span> <span data-ttu-id="d585b-150">Microsoft Teams 将只显示前 150 个字符。</span><span class="sxs-lookup"><span data-stu-id="d585b-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="d585b-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="d585b-151">templateParameters</span></span>|<span data-ttu-id="d585b-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d585b-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="d585b-153">在 Teams 应用清单 中对应的活动源条目中定义的 `activityType` 模板 [变量的值](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="d585b-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="d585b-154">recipient</span><span class="sxs-lookup"><span data-stu-id="d585b-154">recipient</span></span>|[<span data-ttu-id="d585b-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="d585b-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="d585b-156">通知的收件人。</span><span class="sxs-lookup"><span data-stu-id="d585b-156">Recipient of the notification.</span></span> <span data-ttu-id="d585b-157">仅支持 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="d585b-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="d585b-158">另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="d585b-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="d585b-159">将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityUrl` ：</span><span class="sxs-lookup"><span data-stu-id="d585b-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="d585b-160">团队</span><span class="sxs-lookup"><span data-stu-id="d585b-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="d585b-161">频道</span><span class="sxs-lookup"><span data-stu-id="d585b-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="d585b-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="d585b-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="d585b-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d585b-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="d585b-164">**注意：** 实体 URL 必须相同或 URL 中团队的子资源。</span><span class="sxs-lookup"><span data-stu-id="d585b-164">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="d585b-165">此外 [，Teams 应用](/microsoftteams/platform/overview) 必须安装在团队中。</span><span class="sxs-lookup"><span data-stu-id="d585b-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="d585b-166">响应</span><span class="sxs-lookup"><span data-stu-id="d585b-166">Response</span></span>

<span data-ttu-id="d585b-167">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d585b-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d585b-168">示例</span><span class="sxs-lookup"><span data-stu-id="d585b-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="d585b-169">示例 1：通知用户有关待处理的财务审批请求</span><span class="sxs-lookup"><span data-stu-id="d585b-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="d585b-170">此示例演示如何发送团队的活动源通知。</span><span class="sxs-lookup"><span data-stu-id="d585b-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="d585b-171">此示例通知团队所有者有关待处理的财务审批请求。</span><span class="sxs-lookup"><span data-stu-id="d585b-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="d585b-172">请求</span><span class="sxs-lookup"><span data-stu-id="d585b-172">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d585b-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="d585b-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}"
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
# <a name="c"></a>[<span data-ttu-id="d585b-174">C#</span><span class="sxs-lookup"><span data-stu-id="d585b-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d585b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d585b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d585b-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d585b-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d585b-177">Java</span><span class="sxs-lookup"><span data-stu-id="d585b-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


#### <a name="response"></a><span data-ttu-id="d585b-178">响应</span><span class="sxs-lookup"><span data-stu-id="d585b-178">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="d585b-179">示例 2：通知用户有关频道选项卡的信息</span><span class="sxs-lookup"><span data-stu-id="d585b-179">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="d585b-180">与上一示例类似，此示例对 `entityUrl` 使用 `topic` 。</span><span class="sxs-lookup"><span data-stu-id="d585b-180">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="d585b-181">但是，此示例[链接到频道中的](../resources/teamstab.md)[选项卡](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="d585b-181">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="d585b-182">选项卡承载一个页面，向用户显示其酒店预订的状态。</span><span class="sxs-lookup"><span data-stu-id="d585b-182">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="d585b-183">选择通知后，用户即可访问选项卡，可在其中查看预订。</span><span class="sxs-lookup"><span data-stu-id="d585b-183">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="d585b-184">请求</span><span class="sxs-lookup"><span data-stu-id="d585b-184">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
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

#### <a name="response"></a><span data-ttu-id="d585b-185">响应</span><span class="sxs-lookup"><span data-stu-id="d585b-185">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="d585b-186">示例 3：使用自定义主题通知用户事件</span><span class="sxs-lookup"><span data-stu-id="d585b-186">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="d585b-187">如前面的示例中所示，你可以链接到团队的不同方面。</span><span class="sxs-lookup"><span data-stu-id="d585b-187">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="d585b-188">但是，如果你希望链接到不是团队的一部分或不是由 Microsoft Graph 表示的方面，或者想要自定义名称，你可以将 的源设置为 并传递其自定义 `topic` `text` 值。</span><span class="sxs-lookup"><span data-stu-id="d585b-188">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="d585b-189">`webUrl` 将 source 设置为 时 `topic` 是必需的 `text` 。</span><span class="sxs-lookup"><span data-stu-id="d585b-189">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="d585b-190">请求</span><span class="sxs-lookup"><span data-stu-id="d585b-190">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
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

#### <a name="response"></a><span data-ttu-id="d585b-191">响应</span><span class="sxs-lookup"><span data-stu-id="d585b-191">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
