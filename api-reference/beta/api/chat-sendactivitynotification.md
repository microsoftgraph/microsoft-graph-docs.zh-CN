---
title: 聊天： sendActivityNotification
description: 在聊天范围内发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76598572ebca1421770de5a298f46fdedc30a0c9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521997"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="de0a9-103">聊天： sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="de0a9-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="de0a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de0a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de0a9-105">在聊天范围内发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="de0a9-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="de0a9-106">有关发送通知和执行此操作的要求的详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="de0a9-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="de0a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="de0a9-107">Permissions</span></span>
<span data-ttu-id="de0a9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de0a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de0a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de0a9-110">Permission type</span></span>|<span data-ttu-id="de0a9-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de0a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de0a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de0a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de0a9-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="de0a9-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="de0a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de0a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de0a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de0a9-115">Not Supported.</span></span>|
|<span data-ttu-id="de0a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de0a9-116">Application</span></span>|<span data-ttu-id="de0a9-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="de0a9-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="de0a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de0a9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="de0a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="de0a9-119">Request headers</span></span>
|<span data-ttu-id="de0a9-120">名称</span><span class="sxs-lookup"><span data-stu-id="de0a9-120">Name</span></span>|<span data-ttu-id="de0a9-121">说明</span><span class="sxs-lookup"><span data-stu-id="de0a9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de0a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de0a9-122">Authorization</span></span>|<span data-ttu-id="de0a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de0a9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="de0a9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de0a9-125">Content-Type</span></span>|<span data-ttu-id="de0a9-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="de0a9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de0a9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="de0a9-128">Request body</span></span>
<span data-ttu-id="de0a9-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de0a9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="de0a9-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="de0a9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="de0a9-131">参数</span><span class="sxs-lookup"><span data-stu-id="de0a9-131">Parameter</span></span>|<span data-ttu-id="de0a9-132">类型</span><span class="sxs-lookup"><span data-stu-id="de0a9-132">Type</span></span>|<span data-ttu-id="de0a9-133">说明</span><span class="sxs-lookup"><span data-stu-id="de0a9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de0a9-134">topic</span><span class="sxs-lookup"><span data-stu-id="de0a9-134">topic</span></span>|[<span data-ttu-id="de0a9-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="de0a9-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="de0a9-136">通知的主题。</span><span class="sxs-lookup"><span data-stu-id="de0a9-136">Topic of the notification.</span></span> <span data-ttu-id="de0a9-137">指定要讨论的资源。</span><span class="sxs-lookup"><span data-stu-id="de0a9-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="de0a9-138">activityType</span><span class="sxs-lookup"><span data-stu-id="de0a9-138">activityType</span></span>|<span data-ttu-id="de0a9-139">String</span><span class="sxs-lookup"><span data-stu-id="de0a9-139">String</span></span>|<span data-ttu-id="de0a9-140">活动类型。</span><span class="sxs-lookup"><span data-stu-id="de0a9-140">Activity type.</span></span> <span data-ttu-id="de0a9-141">必须在 [团队应用程序清单](/microsoftteams/platform/overview)中声明。</span><span class="sxs-lookup"><span data-stu-id="de0a9-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="de0a9-142">chainId</span><span class="sxs-lookup"><span data-stu-id="de0a9-142">chainId</span></span>|<span data-ttu-id="de0a9-143">Int64</span><span class="sxs-lookup"><span data-stu-id="de0a9-143">Int64</span></span>|<span data-ttu-id="de0a9-144">可选。</span><span class="sxs-lookup"><span data-stu-id="de0a9-144">Optional.</span></span> <span data-ttu-id="de0a9-145">用于替代以前的通知。</span><span class="sxs-lookup"><span data-stu-id="de0a9-145">Used to override a previous notification.</span></span> <span data-ttu-id="de0a9-146">`chainId`在后续请求中使用相同的重写以前的通知。</span><span class="sxs-lookup"><span data-stu-id="de0a9-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="de0a9-147">previewText</span><span class="sxs-lookup"><span data-stu-id="de0a9-147">previewText</span></span>|[<span data-ttu-id="de0a9-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="de0a9-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="de0a9-149">预览通知文本。</span><span class="sxs-lookup"><span data-stu-id="de0a9-149">Preview text for the notification.</span></span> <span data-ttu-id="de0a9-150">Microsoft 团队将仅显示前150个字符。</span><span class="sxs-lookup"><span data-stu-id="de0a9-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="de0a9-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="de0a9-151">templateParameters</span></span>|<span data-ttu-id="de0a9-152">[keyValuePair](../resources/keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de0a9-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="de0a9-153">在与 `activityType` [团队应用程序清单](/microsoftteams/platform/overview)对应的活动源条目中定义的模板变量的值。</span><span class="sxs-lookup"><span data-stu-id="de0a9-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="de0a9-154">recipient</span><span class="sxs-lookup"><span data-stu-id="de0a9-154">recipient</span></span>|[<span data-ttu-id="de0a9-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="de0a9-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="de0a9-156">通知的收件人。</span><span class="sxs-lookup"><span data-stu-id="de0a9-156">Recipient of the notification.</span></span> <span data-ttu-id="de0a9-157">仅支持 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="de0a9-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="de0a9-158">另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="de0a9-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="de0a9-159">将主题属性的值设置为以下资源时，支持以下资源 `source` **topic** `entityURL` ：</span><span class="sxs-lookup"><span data-stu-id="de0a9-159">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="de0a9-160">聊天</span><span class="sxs-lookup"><span data-stu-id="de0a9-160">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="de0a9-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="de0a9-161">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="de0a9-162">**注意：** 实体 URL 必须与 URL 中的聊天或子资源相同。</span><span class="sxs-lookup"><span data-stu-id="de0a9-162">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="de0a9-163">此外，还必须在聊天中安装 [团队应用程序](/microsoftteams/platform/overview) 。</span><span class="sxs-lookup"><span data-stu-id="de0a9-163">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="de0a9-164">响应</span><span class="sxs-lookup"><span data-stu-id="de0a9-164">Response</span></span>

<span data-ttu-id="de0a9-165">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="de0a9-165">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="de0a9-166">示例</span><span class="sxs-lookup"><span data-stu-id="de0a9-166">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="de0a9-167">示例1：通知用户在聊天中创建的任务</span><span class="sxs-lookup"><span data-stu-id="de0a9-167">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="de0a9-168">本示例演示如何为在聊天中创建的新任务发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="de0a9-168">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="de0a9-169">有关更多详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。</span><span class="sxs-lookup"><span data-stu-id="de0a9-169">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="de0a9-170">请求</span><span class="sxs-lookup"><span data-stu-id="de0a9-170">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="de0a9-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="de0a9-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
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
# <a name="c"></a>[<span data-ttu-id="de0a9-172">C#</span><span class="sxs-lookup"><span data-stu-id="de0a9-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de0a9-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de0a9-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de0a9-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de0a9-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de0a9-175">Java</span><span class="sxs-lookup"><span data-stu-id="de0a9-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="de0a9-176">响应</span><span class="sxs-lookup"><span data-stu-id="de0a9-176">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a><span data-ttu-id="de0a9-177">示例2：在聊天消息中通知用户所需的审批</span><span class="sxs-lookup"><span data-stu-id="de0a9-177">Example 2: Notify a user about a approval needed in a chat message</span></span>

<span data-ttu-id="de0a9-178">与上一个示例类似，此示例使用 `entityUrl` `topic` 。</span><span class="sxs-lookup"><span data-stu-id="de0a9-178">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="de0a9-179">但是，在这种情况下，它链接到聊天中的邮件。</span><span class="sxs-lookup"><span data-stu-id="de0a9-179">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="de0a9-180">邮件可以包含卡片上有审批按钮的卡片。</span><span class="sxs-lookup"><span data-stu-id="de0a9-180">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="de0a9-181">请求</span><span class="sxs-lookup"><span data-stu-id="de0a9-181">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
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

#### <a name="response"></a><span data-ttu-id="de0a9-182">响应</span><span class="sxs-lookup"><span data-stu-id="de0a9-182">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="de0a9-183">示例3：通知用户与聊天相关的事件</span><span class="sxs-lookup"><span data-stu-id="de0a9-183">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="de0a9-184">如前面的示例中所示，您可以链接到聊天的不同方面。</span><span class="sxs-lookup"><span data-stu-id="de0a9-184">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="de0a9-185">但是，如果您想要链接到不属于聊天的方位，或者不是由 Microsoft Graph 表示的，则可以将的来源设置 `topic` 为， `text` 并为其传入自定义值。</span><span class="sxs-lookup"><span data-stu-id="de0a9-185">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="de0a9-186">此外，将 " `webUrl` 源" 设置为时也是必需的 `topic` `text` 。</span><span class="sxs-lookup"><span data-stu-id="de0a9-186">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="de0a9-187">请求</span><span class="sxs-lookup"><span data-stu-id="de0a9-187">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
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

#### <a name="response"></a><span data-ttu-id="de0a9-188">响应</span><span class="sxs-lookup"><span data-stu-id="de0a9-188">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
