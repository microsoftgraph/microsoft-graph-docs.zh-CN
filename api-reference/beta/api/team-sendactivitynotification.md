---
title: 团队： sendActivityNotification
description: 在团队范围内发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed7177f4a91fae4fb5e87f496489cdc0c9569607
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377523"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="96174-103">团队： sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="96174-103">team: sendActivityNotification</span></span>
<span data-ttu-id="96174-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96174-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96174-105">在团队范围内发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="96174-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="96174-106">有关发送通知和执行此操作的要求的详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="96174-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="96174-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="96174-107">Permissions</span></span>
<span data-ttu-id="96174-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96174-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96174-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96174-110">Permission type</span></span>|<span data-ttu-id="96174-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96174-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96174-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96174-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96174-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="96174-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="96174-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96174-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96174-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96174-115">Not Supported.</span></span>|
|<span data-ttu-id="96174-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96174-116">Application</span></span>|<span data-ttu-id="96174-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="96174-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="96174-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96174-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="96174-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96174-119">Request headers</span></span>
|<span data-ttu-id="96174-120">名称</span><span class="sxs-lookup"><span data-stu-id="96174-120">Name</span></span>|<span data-ttu-id="96174-121">说明</span><span class="sxs-lookup"><span data-stu-id="96174-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96174-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96174-122">Authorization</span></span>|<span data-ttu-id="96174-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96174-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="96174-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96174-125">Content-Type</span></span>|<span data-ttu-id="96174-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="96174-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96174-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="96174-128">Request body</span></span>
<span data-ttu-id="96174-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96174-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="96174-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="96174-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="96174-131">参数</span><span class="sxs-lookup"><span data-stu-id="96174-131">Parameter</span></span>|<span data-ttu-id="96174-132">类型</span><span class="sxs-lookup"><span data-stu-id="96174-132">Type</span></span>|<span data-ttu-id="96174-133">说明</span><span class="sxs-lookup"><span data-stu-id="96174-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96174-134">topic</span><span class="sxs-lookup"><span data-stu-id="96174-134">topic</span></span>|[<span data-ttu-id="96174-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="96174-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="96174-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="96174-136">Topic of the notification.</span></span> <span data-ttu-id="96174-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="96174-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="96174-138">activityType</span><span class="sxs-lookup"><span data-stu-id="96174-138">activityType</span></span>|<span data-ttu-id="96174-139">String</span><span class="sxs-lookup"><span data-stu-id="96174-139">String</span></span>|<span data-ttu-id="96174-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="96174-140">Activity type.</span></span> <span data-ttu-id="96174-141">必须在 [团队应用程序清单](/microsoftteams/platform/overview)中声明。</span><span class="sxs-lookup"><span data-stu-id="96174-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="96174-142">chainId</span><span class="sxs-lookup"><span data-stu-id="96174-142">chainId</span></span>|<span data-ttu-id="96174-143">Int64</span><span class="sxs-lookup"><span data-stu-id="96174-143">Int64</span></span>|<span data-ttu-id="96174-144">可选。</span><span class="sxs-lookup"><span data-stu-id="96174-144">Optional.</span></span> <span data-ttu-id="96174-145">用于替代以前的通知。</span><span class="sxs-lookup"><span data-stu-id="96174-145">Used to override a previous notification.</span></span> <span data-ttu-id="96174-146">`chainId`在后续请求中使用相同的重写以前的通知。</span><span class="sxs-lookup"><span data-stu-id="96174-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="96174-147">previewText</span><span class="sxs-lookup"><span data-stu-id="96174-147">previewText</span></span>|[<span data-ttu-id="96174-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="96174-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="96174-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="96174-149">Preview text for the notification.</span></span> <span data-ttu-id="96174-150">Microsoft 团队将仅显示前150个字符。</span><span class="sxs-lookup"><span data-stu-id="96174-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="96174-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="96174-151">templateParameters</span></span>|<span data-ttu-id="96174-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96174-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="96174-153">在与 `activityType` [团队应用程序清单](/microsoftteams/platform/overview)对应的活动源条目中定义的模板变量的值。</span><span class="sxs-lookup"><span data-stu-id="96174-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="96174-154">recipient</span><span class="sxs-lookup"><span data-stu-id="96174-154">recipient</span></span>|[<span data-ttu-id="96174-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="96174-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="96174-156">通知的收件人。</span><span class="sxs-lookup"><span data-stu-id="96174-156">Recipient of the notification.</span></span> <span data-ttu-id="96174-157">仅支持 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="96174-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="96174-158">另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="96174-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="96174-159">将主题属性的值设置为以下资源时，支持以下资源 `source` **topic** `entityUrl` ：</span><span class="sxs-lookup"><span data-stu-id="96174-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="96174-160">团队</span><span class="sxs-lookup"><span data-stu-id="96174-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="96174-161">频道</span><span class="sxs-lookup"><span data-stu-id="96174-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="96174-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="96174-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="96174-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="96174-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="96174-164">**注意：** 实体 url 必须是 url 中的团队的相同或子资源。</span><span class="sxs-lookup"><span data-stu-id="96174-164">**Note:** The entity url must be same or child resource of the team in the url.</span></span> <span data-ttu-id="96174-165">此外，团队 [应用程序](/microsoftteams/platform/overview) 必须安装在团队中。</span><span class="sxs-lookup"><span data-stu-id="96174-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="96174-166">响应</span><span class="sxs-lookup"><span data-stu-id="96174-166">Response</span></span>

<span data-ttu-id="96174-167">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="96174-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="96174-168">示例</span><span class="sxs-lookup"><span data-stu-id="96174-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="96174-169">示例1：通知用户有关待定的财务审批请求</span><span class="sxs-lookup"><span data-stu-id="96174-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="96174-170">本示例演示如何向团队发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="96174-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="96174-171">本示例将关于待处理的财务审批请求通知工作组所有者。</span><span class="sxs-lookup"><span data-stu-id="96174-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="96174-172">请求</span><span class="sxs-lookup"><span data-stu-id="96174-172">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
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

#### <a name="response"></a><span data-ttu-id="96174-173">响应</span><span class="sxs-lookup"><span data-stu-id="96174-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="96174-174">示例2：通知用户有关频道选项卡的信息</span><span class="sxs-lookup"><span data-stu-id="96174-174">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="96174-175">与上一个示例类似，此示例使用 `entityUrl` `topic` 。</span><span class="sxs-lookup"><span data-stu-id="96174-175">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="96174-176">但是，此示例链接到[频道](../resources/channel.md)中的一个[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="96174-176">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="96174-177">该选项卡承载一个页面，向用户显示其酒店预订的状态。</span><span class="sxs-lookup"><span data-stu-id="96174-177">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="96174-178">选择通知将使用户进入该选项卡，在其中可以检查其保留。</span><span class="sxs-lookup"><span data-stu-id="96174-178">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="96174-179">请求</span><span class="sxs-lookup"><span data-stu-id="96174-179">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
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

#### <a name="response"></a><span data-ttu-id="96174-180">响应</span><span class="sxs-lookup"><span data-stu-id="96174-180">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="96174-181">示例3：使用自定义主题通知用户有关事件</span><span class="sxs-lookup"><span data-stu-id="96174-181">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="96174-182">如前面的示例中所示，您可以链接到团队的不同方面。</span><span class="sxs-lookup"><span data-stu-id="96174-182">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="96174-183">但是，如果要链接到不属于团队的方位或者不是由 Microsoft Graph 表示的方位，或者您想要自定义该名称，则可以设置 to 的来源 `topic` `text` 并为其传入自定义值。</span><span class="sxs-lookup"><span data-stu-id="96174-183">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="96174-184">`webUrl` 将 "源" 设置为时是必需的 `topic` `text` 。</span><span class="sxs-lookup"><span data-stu-id="96174-184">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="96174-185">请求</span><span class="sxs-lookup"><span data-stu-id="96174-185">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
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

#### <a name="response"></a><span data-ttu-id="96174-186">响应</span><span class="sxs-lookup"><span data-stu-id="96174-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
