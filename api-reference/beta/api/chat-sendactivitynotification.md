---
title: chat： sendActivityNotification
description: 在聊天范围内发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6335c98549a76fbf0baf13613738251770edeca9
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316915"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="c5f75-103">chat： sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="c5f75-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="c5f75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f75-105">在聊天范围内发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="c5f75-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="c5f75-106">有关发送通知的更多详细信息以及发送通知的要求，请参阅[发送Teams活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5f75-107">权限</span><span class="sxs-lookup"><span data-stu-id="c5f75-107">Permissions</span></span>
<span data-ttu-id="c5f75-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f75-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5f75-110">Permission type</span></span>|<span data-ttu-id="c5f75-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5f75-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f75-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5f75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f75-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c5f75-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="c5f75-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5f75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f75-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5f75-115">Not Supported.</span></span>|
|<span data-ttu-id="c5f75-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5f75-116">Application</span></span>|<span data-ttu-id="c5f75-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c5f75-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f75-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5f75-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="c5f75-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5f75-119">Request headers</span></span>
|<span data-ttu-id="c5f75-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5f75-120">Name</span></span>|<span data-ttu-id="c5f75-121">说明</span><span class="sxs-lookup"><span data-stu-id="c5f75-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5f75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f75-122">Authorization</span></span>|<span data-ttu-id="c5f75-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5f75-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c5f75-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5f75-125">Content-Type</span></span>|<span data-ttu-id="c5f75-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c5f75-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f75-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5f75-128">Request body</span></span>
<span data-ttu-id="c5f75-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5f75-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c5f75-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c5f75-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c5f75-131">参数</span><span class="sxs-lookup"><span data-stu-id="c5f75-131">Parameter</span></span>|<span data-ttu-id="c5f75-132">类型</span><span class="sxs-lookup"><span data-stu-id="c5f75-132">Type</span></span>|<span data-ttu-id="c5f75-133">说明</span><span class="sxs-lookup"><span data-stu-id="c5f75-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f75-134">topic</span><span class="sxs-lookup"><span data-stu-id="c5f75-134">topic</span></span>|[<span data-ttu-id="c5f75-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="c5f75-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="c5f75-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="c5f75-136">Topic of the notification.</span></span> <span data-ttu-id="c5f75-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="c5f75-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="c5f75-138">activityType</span><span class="sxs-lookup"><span data-stu-id="c5f75-138">activityType</span></span>|<span data-ttu-id="c5f75-139">String</span><span class="sxs-lookup"><span data-stu-id="c5f75-139">String</span></span>|<span data-ttu-id="c5f75-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="c5f75-140">Activity type.</span></span> <span data-ttu-id="c5f75-141">这必须在应用清单[Teams声明](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="c5f75-142">chainId</span><span class="sxs-lookup"><span data-stu-id="c5f75-142">chainId</span></span>|<span data-ttu-id="c5f75-143">Int64</span><span class="sxs-lookup"><span data-stu-id="c5f75-143">Int64</span></span>|<span data-ttu-id="c5f75-144">可选。</span><span class="sxs-lookup"><span data-stu-id="c5f75-144">Optional.</span></span> <span data-ttu-id="c5f75-145">用于替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="c5f75-145">Used to override a previous notification.</span></span> <span data-ttu-id="c5f75-146">在后续 `chainId` 请求中使用相同的方法替代上一个通知。</span><span class="sxs-lookup"><span data-stu-id="c5f75-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="c5f75-147">previewText</span><span class="sxs-lookup"><span data-stu-id="c5f75-147">previewText</span></span>|[<span data-ttu-id="c5f75-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="c5f75-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="c5f75-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="c5f75-149">Preview text for the notification.</span></span> <span data-ttu-id="c5f75-150">Microsoft Teams显示前 150 个字符。</span><span class="sxs-lookup"><span data-stu-id="c5f75-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="c5f75-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="c5f75-151">templateParameters</span></span>|<span data-ttu-id="c5f75-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c5f75-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="c5f75-153">活动源条目中定义的模板变量的值与应用程序Teams `activityType` [相对应](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="c5f75-154">recipient</span><span class="sxs-lookup"><span data-stu-id="c5f75-154">recipient</span></span>|[<span data-ttu-id="c5f75-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="c5f75-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="c5f75-156">通知的收件人。</span><span class="sxs-lookup"><span data-stu-id="c5f75-156">Recipient of the notification.</span></span> <span data-ttu-id="c5f75-157">另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) 和 [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) and [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="c5f75-158">将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityURL` ：</span><span class="sxs-lookup"><span data-stu-id="c5f75-158">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="c5f75-159">聊天</span><span class="sxs-lookup"><span data-stu-id="c5f75-159">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="c5f75-160">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c5f75-160">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="c5f75-161">**注意：** 实体 URL 必须与 URL 中的聊天相同或为聊天的子资源。</span><span class="sxs-lookup"><span data-stu-id="c5f75-161">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="c5f75-162">此外[，Teams应用](/microsoftteams/platform/overview)必须安装在聊天中。</span><span class="sxs-lookup"><span data-stu-id="c5f75-162">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="c5f75-163">响应</span><span class="sxs-lookup"><span data-stu-id="c5f75-163">Response</span></span>

<span data-ttu-id="c5f75-164">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c5f75-164">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c5f75-165">示例</span><span class="sxs-lookup"><span data-stu-id="c5f75-165">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="c5f75-166">示例 1：通知用户在聊天中创建的任务</span><span class="sxs-lookup"><span data-stu-id="c5f75-166">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="c5f75-167">此示例演示如何发送在聊天中创建的新任务的活动源通知。</span><span class="sxs-lookup"><span data-stu-id="c5f75-167">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="c5f75-168">有关详细信息，请参阅[发送Teams活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-168">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="c5f75-169">请求</span><span class="sxs-lookup"><span data-stu-id="c5f75-169">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c5f75-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f75-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_1"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
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
# <a name="c"></a>[<span data-ttu-id="c5f75-171">C#</span><span class="sxs-lookup"><span data-stu-id="c5f75-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f75-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f75-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f75-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f75-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5f75-174">Java</span><span class="sxs-lookup"><span data-stu-id="c5f75-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5f75-175">响应</span><span class="sxs-lookup"><span data-stu-id="c5f75-175">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-approval-needed-in-a-chat-message"></a><span data-ttu-id="c5f75-176">示例 2：通知用户聊天消息中所需的审批</span><span class="sxs-lookup"><span data-stu-id="c5f75-176">Example 2: Notify a user about an approval needed in a chat message</span></span>

<span data-ttu-id="c5f75-177">与上一示例类似，此示例对 `entityUrl` 使用 `topic` 。</span><span class="sxs-lookup"><span data-stu-id="c5f75-177">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="c5f75-178">但是，在这种情况下，它会链接到聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="c5f75-178">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="c5f75-179">邮件可包含一个卡片，其中包含审批按钮。</span><span class="sxs-lookup"><span data-stu-id="c5f75-179">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="c5f75-180">请求</span><span class="sxs-lookup"><span data-stu-id="c5f75-180">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c5f75-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f75-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_2"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
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
# <a name="c"></a>[<span data-ttu-id="c5f75-182">C#</span><span class="sxs-lookup"><span data-stu-id="c5f75-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f75-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f75-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f75-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f75-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5f75-185">Java</span><span class="sxs-lookup"><span data-stu-id="c5f75-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5f75-186">响应</span><span class="sxs-lookup"><span data-stu-id="c5f75-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="c5f75-187">示例 3：向用户通知与聊天相关的事件</span><span class="sxs-lookup"><span data-stu-id="c5f75-187">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="c5f75-188">如前面的示例所示，您可以链接到聊天的不同方面。</span><span class="sxs-lookup"><span data-stu-id="c5f75-188">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="c5f75-189">但是，如果要链接到不是聊天的一部分或不是由 Microsoft Graph 表示的方面，可以将 的源设置为 并传递其自定义 `topic` `text` 值。</span><span class="sxs-lookup"><span data-stu-id="c5f75-189">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="c5f75-190">此外， `webUrl` 将 source 设置为 时 `topic` ，也是必需的 `text` 。</span><span class="sxs-lookup"><span data-stu-id="c5f75-190">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="c5f75-191">请求</span><span class="sxs-lookup"><span data-stu-id="c5f75-191">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c5f75-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f75-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_3"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
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
# <a name="c"></a>[<span data-ttu-id="c5f75-193">C#</span><span class="sxs-lookup"><span data-stu-id="c5f75-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f75-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f75-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f75-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f75-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5f75-196">Java</span><span class="sxs-lookup"><span data-stu-id="c5f75-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5f75-197">响应</span><span class="sxs-lookup"><span data-stu-id="c5f75-197">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-chat-members-about-a-task-created-in-a-chat"></a><span data-ttu-id="c5f75-198">示例 4：通知聊天成员有关在聊天中创建的任务</span><span class="sxs-lookup"><span data-stu-id="c5f75-198">Example 4: Notify the chat members about a task created in a chat</span></span>

<span data-ttu-id="c5f75-199">此示例演示如何向所有聊天成员发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="c5f75-199">This example shows how you can send an activity feed notification to all chat members.</span></span> <span data-ttu-id="c5f75-200">此示例与前面的示例类似。</span><span class="sxs-lookup"><span data-stu-id="c5f75-200">This example is similar to previous examples.</span></span> <span data-ttu-id="c5f75-201">但是，在这种情况下， 是 `recipient` [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="c5f75-201">However, in this case, the `recipient` is a [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span></span> <span data-ttu-id="c5f75-202">请注意， `chatId` 中指定的 `recipient` 必须与请求 URL `chatId` 中指定的 匹配。</span><span class="sxs-lookup"><span data-stu-id="c5f75-202">Note that the `chatId` specified in the `recipient` must match the `chatId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="c5f75-203">请求</span><span class="sxs-lookup"><span data-stu-id="c5f75-203">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c5f75-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f75-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="c5f75-205">C#</span><span class="sxs-lookup"><span data-stu-id="c5f75-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f75-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f75-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f75-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f75-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5f75-208">Java</span><span class="sxs-lookup"><span data-stu-id="c5f75-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5f75-209">响应</span><span class="sxs-lookup"><span data-stu-id="c5f75-209">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
