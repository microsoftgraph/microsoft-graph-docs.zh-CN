---
title: chat： sendActivityNotification
description: 在聊天范围内发送活动源通知。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eabe78843dd9b1e2e71fd433a61e04154e9aafcc
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474126"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="893d4-103">chat： sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="893d4-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="893d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="893d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="893d4-105">在聊天范围内发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="893d4-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="893d4-106">有关发送通知的更多详细信息以及发送通知的要求，请参阅 [发送 Teams 活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="893d4-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="893d4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="893d4-107">Permissions</span></span>
<span data-ttu-id="893d4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="893d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="893d4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="893d4-110">Permission type</span></span>|<span data-ttu-id="893d4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="893d4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="893d4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="893d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="893d4-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="893d4-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="893d4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="893d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="893d4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="893d4-115">Not Supported.</span></span>|
|<span data-ttu-id="893d4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="893d4-116">Application</span></span>|<span data-ttu-id="893d4-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="893d4-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="893d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="893d4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="893d4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="893d4-119">Request headers</span></span>
|<span data-ttu-id="893d4-120">名称</span><span class="sxs-lookup"><span data-stu-id="893d4-120">Name</span></span>|<span data-ttu-id="893d4-121">说明</span><span class="sxs-lookup"><span data-stu-id="893d4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="893d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="893d4-122">Authorization</span></span>|<span data-ttu-id="893d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="893d4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="893d4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="893d4-125">Content-Type</span></span>|<span data-ttu-id="893d4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="893d4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="893d4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="893d4-128">Request body</span></span>
<span data-ttu-id="893d4-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="893d4-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="893d4-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="893d4-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="893d4-131">参数</span><span class="sxs-lookup"><span data-stu-id="893d4-131">Parameter</span></span>|<span data-ttu-id="893d4-132">类型</span><span class="sxs-lookup"><span data-stu-id="893d4-132">Type</span></span>|<span data-ttu-id="893d4-133">说明</span><span class="sxs-lookup"><span data-stu-id="893d4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="893d4-134">topic</span><span class="sxs-lookup"><span data-stu-id="893d4-134">topic</span></span>|[<span data-ttu-id="893d4-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="893d4-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="893d4-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="893d4-136">Topic of the notification.</span></span> <span data-ttu-id="893d4-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="893d4-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="893d4-138">activityType</span><span class="sxs-lookup"><span data-stu-id="893d4-138">activityType</span></span>|<span data-ttu-id="893d4-139">String</span><span class="sxs-lookup"><span data-stu-id="893d4-139">String</span></span>|<span data-ttu-id="893d4-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="893d4-140">Activity type.</span></span> <span data-ttu-id="893d4-141">这必须在 Teams 应用清单 [中声明](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="893d4-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="893d4-142">chainId</span><span class="sxs-lookup"><span data-stu-id="893d4-142">chainId</span></span>|<span data-ttu-id="893d4-143">Int64</span><span class="sxs-lookup"><span data-stu-id="893d4-143">Int64</span></span>|<span data-ttu-id="893d4-144">可选。</span><span class="sxs-lookup"><span data-stu-id="893d4-144">Optional.</span></span> <span data-ttu-id="893d4-145">用于替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="893d4-145">Used to override a previous notification.</span></span> <span data-ttu-id="893d4-146">在后续 `chainId` 请求中使用相同的方法替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="893d4-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="893d4-147">previewText</span><span class="sxs-lookup"><span data-stu-id="893d4-147">previewText</span></span>|[<span data-ttu-id="893d4-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="893d4-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="893d4-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="893d4-149">Preview text for the notification.</span></span> <span data-ttu-id="893d4-150">Microsoft Teams 将只显示前 150 个字符。</span><span class="sxs-lookup"><span data-stu-id="893d4-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="893d4-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="893d4-151">templateParameters</span></span>|<span data-ttu-id="893d4-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="893d4-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="893d4-153">在 Teams 应用清单 中对应的活动源条目中定义的 `activityType` 模板 [变量的值](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="893d4-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="893d4-154">recipient</span><span class="sxs-lookup"><span data-stu-id="893d4-154">recipient</span></span>|[<span data-ttu-id="893d4-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="893d4-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="893d4-156">通知的收件人。</span><span class="sxs-lookup"><span data-stu-id="893d4-156">Recipient of the notification.</span></span> <span data-ttu-id="893d4-157">仅支持 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="893d4-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="893d4-158">另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="893d4-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="893d4-159">将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityURL` ：</span><span class="sxs-lookup"><span data-stu-id="893d4-159">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="893d4-160">聊天</span><span class="sxs-lookup"><span data-stu-id="893d4-160">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="893d4-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="893d4-161">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="893d4-162">**注意：** 实体 URL 必须与 URL 中的聊天相同或为聊天的子资源。</span><span class="sxs-lookup"><span data-stu-id="893d4-162">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="893d4-163">此外， [必须在聊天](/microsoftteams/platform/overview) 中安装 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="893d4-163">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="893d4-164">响应</span><span class="sxs-lookup"><span data-stu-id="893d4-164">Response</span></span>

<span data-ttu-id="893d4-165">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="893d4-165">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="893d4-166">示例</span><span class="sxs-lookup"><span data-stu-id="893d4-166">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="893d4-167">示例 1：通知用户在聊天中创建的任务</span><span class="sxs-lookup"><span data-stu-id="893d4-167">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="893d4-168">此示例演示如何发送在聊天中创建的新任务的活动源通知。</span><span class="sxs-lookup"><span data-stu-id="893d4-168">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="893d4-169">有关详细信息，请参阅发送 [Teams 活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="893d4-169">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="893d4-170">请求</span><span class="sxs-lookup"><span data-stu-id="893d4-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```

#### <a name="response"></a><span data-ttu-id="893d4-171">响应</span><span class="sxs-lookup"><span data-stu-id="893d4-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a><span data-ttu-id="893d4-172">示例 2：通知用户聊天消息中所需的审批</span><span class="sxs-lookup"><span data-stu-id="893d4-172">Example 2: Notify a user about a approval needed in a chat message</span></span>

<span data-ttu-id="893d4-173">与上一示例类似，此示例对 `entityUrl` 使用 `topic` 。</span><span class="sxs-lookup"><span data-stu-id="893d4-173">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="893d4-174">但是，在这种情况下，它会链接到聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="893d4-174">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="893d4-175">邮件可包含一个卡片，其中包含审批按钮。</span><span class="sxs-lookup"><span data-stu-id="893d4-175">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="893d4-176">请求</span><span class="sxs-lookup"><span data-stu-id="893d4-176">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="893d4-177">响应</span><span class="sxs-lookup"><span data-stu-id="893d4-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="893d4-178">示例 3：向用户通知与聊天相关的事件</span><span class="sxs-lookup"><span data-stu-id="893d4-178">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="893d4-179">如前面的示例所示，您可以链接到聊天的不同方面。</span><span class="sxs-lookup"><span data-stu-id="893d4-179">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="893d4-180">但是，如果你想要链接到不是聊天的一部分，或者不是由 Microsoft Graph 表示的方面，你可以将 的源设置为 并传递其自定义 `topic` `text` 值。</span><span class="sxs-lookup"><span data-stu-id="893d4-180">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="893d4-181">此外， `webUrl` 将 source 设置为 时 `topic` ，也是必需的 `text` 。</span><span class="sxs-lookup"><span data-stu-id="893d4-181">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="893d4-182">请求</span><span class="sxs-lookup"><span data-stu-id="893d4-182">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
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

#### <a name="response"></a><span data-ttu-id="893d4-183">响应</span><span class="sxs-lookup"><span data-stu-id="893d4-183">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
