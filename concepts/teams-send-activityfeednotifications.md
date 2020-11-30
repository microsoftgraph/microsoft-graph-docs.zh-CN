---
title: 向 Microsoft 团队中的用户发送活动源通知
description: 使用团队应用和 microsoft graph 将活动源通知发送给 Microsoft 团队中的用户。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 33a44ef158a1336e198e7382e144efed11ff35e7
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377431"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a><span data-ttu-id="a6f44-103">向 Microsoft 团队中的用户发送活动源通知</span><span class="sxs-lookup"><span data-stu-id="a6f44-103">Send activity feed notifications to users in Microsoft Teams</span></span>

<span data-ttu-id="a6f44-104">Microsoft 团队活动源使用户能够通过通知所做的更改来会审需要注意的项目。</span><span class="sxs-lookup"><span data-stu-id="a6f44-104">The Microsoft Teams activity feed enables users to triage items that require attention by notifying them of changes.</span></span> <span data-ttu-id="a6f44-105">您可以使用 Microsoft Graph 中的活动源通知 Api 将此功能扩展到您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a6f44-105">You can use the activity feed notification APIs in Microsoft Graph to extend this functionality to your apps.</span></span> <span data-ttu-id="a6f44-106">这样一来，你的应用程序可以提供更丰富的体验，并通过帮助保持他们所使用的工具和工作流中的更改来保持最新。</span><span class="sxs-lookup"><span data-stu-id="a6f44-106">This allows your apps to provide richer experiences and better engage users by helping to keep them up to date with changes in the tools and workflows they use.</span></span>

## <a name="understanding-the-basics-of-activity-feed-notification"></a><span data-ttu-id="a6f44-107">了解活动源通知的基础知识</span><span class="sxs-lookup"><span data-stu-id="a6f44-107">Understanding the basics of activity feed notification</span></span>

<span data-ttu-id="a6f44-108">Microsoft 团队中的活动源通知由多个位的信息组成，显示在一起，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="a6f44-108">Activity feed notifications in Microsoft Teams are comprised of multiple bits of information, displayed together, as shown in the following image.</span></span>

![显示活动源通知组件的图像](images/teams-activityfeednotifications/notificationtemplate.png)

<span data-ttu-id="a6f44-110">这些组件包括：</span><span class="sxs-lookup"><span data-stu-id="a6f44-110">The components include:</span></span>
- <span data-ttu-id="a6f44-111">启动活动的参与者</span><span class="sxs-lookup"><span data-stu-id="a6f44-111">The actor who initiated the activity</span></span>
- <span data-ttu-id="a6f44-112">一个代表活动类型的图标</span><span class="sxs-lookup"><span data-stu-id="a6f44-112">An icon that represents the activity type</span></span>
- <span data-ttu-id="a6f44-113">主角执行活动的原因</span><span class="sxs-lookup"><span data-stu-id="a6f44-113">The reason the actor did the activity</span></span>
- <span data-ttu-id="a6f44-114">文本预览</span><span class="sxs-lookup"><span data-stu-id="a6f44-114">A text preview</span></span>
- <span data-ttu-id="a6f44-115">一个时间戳</span><span class="sxs-lookup"><span data-stu-id="a6f44-115">A time stamp</span></span>
- <span data-ttu-id="a6f44-116">活动的位置</span><span class="sxs-lookup"><span data-stu-id="a6f44-116">The location of the activity</span></span>

<span data-ttu-id="a6f44-117">下面的示例演示这些组件如何共同提供有关通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a6f44-117">The following example shows how these components together provide the details about a notification.</span></span> <span data-ttu-id="a6f44-118">本示例是关于 Yammer 社区中提到的用户的通知。</span><span class="sxs-lookup"><span data-stu-id="a6f44-118">This example is a notification about a user mentioned in a Yammer community.</span></span>

![Yammer actifity 通知示例](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a><span data-ttu-id="a6f44-120">使用活动源通知 Api 的要求</span><span class="sxs-lookup"><span data-stu-id="a6f44-120">Requirements for using the activity feed notification APIs</span></span>

<span data-ttu-id="a6f44-121">活动源 Api 与 [团队应用](/microsoftteams/platform/overview)一起使用。</span><span class="sxs-lookup"><span data-stu-id="a6f44-121">Activity feed APIs work with a [Teams app](/microsoftteams/platform/overview).</span></span> <span data-ttu-id="a6f44-122">以下是发送活动源通知的要求：</span><span class="sxs-lookup"><span data-stu-id="a6f44-122">The following are the requirements for sending activity feed notifications:</span></span>

- <span data-ttu-id="a6f44-123">团队应用程序清单必须向分区添加了 Azure AD 应用 ID `webApplicationInfo` 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-123">The Teams app manifest must have the Azure AD app ID added to the `webApplicationInfo` section.</span></span> <span data-ttu-id="a6f44-124">有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。</span><span class="sxs-lookup"><span data-stu-id="a6f44-124">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="a6f44-125">必须在 "" 部分声明活动类型 `activities` 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-125">Activity types must be declared in the `activities` section.</span></span> <span data-ttu-id="a6f44-126">有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。</span><span class="sxs-lookup"><span data-stu-id="a6f44-126">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="a6f44-127">必须为收件人（个人身份）或 [团队或团队](/graph/api/resources/team?preserve-view=true) 中的团队用户安装团队应用程序或 [聊天](/graph/api/resources/chat?preserve-view=true) 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-127">The Teams app must be installed for the recipient, either personally, or in a [team](/graph/api/resources/team?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true) they are part of.</span></span> <span data-ttu-id="a6f44-128">有关详细信息，请参阅 [团队应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="a6f44-128">For more information, see [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true).</span></span>

### <a name="teams-app-manifest-changes"></a><span data-ttu-id="a6f44-129">团队应用程序清单更改</span><span class="sxs-lookup"><span data-stu-id="a6f44-129">Teams app manifest changes</span></span>

<span data-ttu-id="a6f44-130">本节介绍了需要添加到团队应用程序清单中的更改。</span><span class="sxs-lookup"><span data-stu-id="a6f44-130">This section describes the changes that need to be added to Teams app manifest.</span></span> <span data-ttu-id="a6f44-131">请注意，您必须使用 [团队应用程序清单](/microsoftteams/platform/resources/schema/manifest-schema) 版本 `1.7` 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="a6f44-131">Note that you must be using the [Teams app manifest](/microsoftteams/platform/resources/schema/manifest-schema) version `1.7` or greater.</span></span>

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a><span data-ttu-id="a6f44-132">webApplicationInfo 节更改</span><span class="sxs-lookup"><span data-stu-id="a6f44-132">webApplicationInfo section changes</span></span>

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|<span data-ttu-id="a6f44-133">参数</span><span class="sxs-lookup"><span data-stu-id="a6f44-133">Parameter</span></span>|<span data-ttu-id="a6f44-134">类型</span><span class="sxs-lookup"><span data-stu-id="a6f44-134">Type</span></span>|<span data-ttu-id="a6f44-135">说明</span><span class="sxs-lookup"><span data-stu-id="a6f44-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f44-136">id</span><span class="sxs-lookup"><span data-stu-id="a6f44-136">id</span></span>|<span data-ttu-id="a6f44-137">string</span><span class="sxs-lookup"><span data-stu-id="a6f44-137">string</span></span>|<span data-ttu-id="a6f44-138">Azure AD 应用 ID (客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-138">Azure AD app ID (client ID).</span></span>|
|<span data-ttu-id="a6f44-139">resource</span><span class="sxs-lookup"><span data-stu-id="a6f44-139">resource</span></span>|<span data-ttu-id="a6f44-140">string</span><span class="sxs-lookup"><span data-stu-id="a6f44-140">string</span></span>|<span data-ttu-id="a6f44-141">与 Azure AD 应用关联的资源。</span><span class="sxs-lookup"><span data-stu-id="a6f44-141">Resource associated with the Azure AD app.</span></span> <span data-ttu-id="a6f44-142">在 Azure 门户中也称为 "答复" 或 "重定向 URL"。</span><span class="sxs-lookup"><span data-stu-id="a6f44-142">Also known as reply or redirect URL in the Azure Portal.</span></span>|

> <span data-ttu-id="a6f44-143">**注意：** 如果同一作用域中的多个团队应用 (团队、聊天或用户) 使用相同的 Azure AD 应用程序，则可能会出现错误。</span><span class="sxs-lookup"><span data-stu-id="a6f44-143">**Note:** You might get an error if multiple Teams apps in the same scope (team, chat or user) are using the same Azure AD app.</span></span> <span data-ttu-id="a6f44-144">请确保您使用的是唯一的 Azure AD 应用。</span><span class="sxs-lookup"><span data-stu-id="a6f44-144">Make sure that you're using unique Azure AD apps.</span></span>

#### <a name="activities-section-changes"></a><span data-ttu-id="a6f44-145">"活动" 部分更改</span><span class="sxs-lookup"><span data-stu-id="a6f44-145">activities section changes</span></span>

```json
"activities":
{
  "activityTypes": [
    {
      "type": "taskCreated",
      "description": "Task Created Activity",
      "templateText": "{actor} created task {taskId} for you"
    },
    {
      "type": "approvalRequired",
      "description": "Deployment requires your approval",
      "templateText": "{actor} created a new deployment {deploymentId}"
    }
  ]
}
```

|<span data-ttu-id="a6f44-146">参数</span><span class="sxs-lookup"><span data-stu-id="a6f44-146">Parameter</span></span>|<span data-ttu-id="a6f44-147">类型</span><span class="sxs-lookup"><span data-stu-id="a6f44-147">Type</span></span>|<span data-ttu-id="a6f44-148">说明</span><span class="sxs-lookup"><span data-stu-id="a6f44-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f44-149">类型</span><span class="sxs-lookup"><span data-stu-id="a6f44-149">type</span></span>|<span data-ttu-id="a6f44-150">string</span><span class="sxs-lookup"><span data-stu-id="a6f44-150">string</span></span>|<span data-ttu-id="a6f44-151">活动的类型。</span><span class="sxs-lookup"><span data-stu-id="a6f44-151">Type of activity.</span></span> <span data-ttu-id="a6f44-152">这在特定清单中需要是唯一的。</span><span class="sxs-lookup"><span data-stu-id="a6f44-152">This needs to be unique in a specific manifest.</span></span>|
|<span data-ttu-id="a6f44-153">说明</span><span class="sxs-lookup"><span data-stu-id="a6f44-153">description</span></span>|<span data-ttu-id="a6f44-154">string</span><span class="sxs-lookup"><span data-stu-id="a6f44-154">string</span></span>|<span data-ttu-id="a6f44-155">可读的简短说明。</span><span class="sxs-lookup"><span data-stu-id="a6f44-155">Human-readable short description.</span></span> <span data-ttu-id="a6f44-156">这将显示在 Microsoft 团队客户端上。</span><span class="sxs-lookup"><span data-stu-id="a6f44-156">This will be visible on the Microsoft Teams client.</span></span>|
|<span data-ttu-id="a6f44-157">templateText</span><span class="sxs-lookup"><span data-stu-id="a6f44-157">templateText</span></span>|<span data-ttu-id="a6f44-158">string</span><span class="sxs-lookup"><span data-stu-id="a6f44-158">string</span></span>|<span data-ttu-id="a6f44-159">活动通知的模板文本。</span><span class="sxs-lookup"><span data-stu-id="a6f44-159">Template text for the activity notification.</span></span> <span data-ttu-id="a6f44-160">您可以通过在中封装参数来声明参数 `{}` 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-160">You can declare your parameters by encapsulating parameters in `{}`.</span></span>|

><span data-ttu-id="a6f44-161">**注意：** `actor` 是一个特殊参数，始终采用调用方的名称。</span><span class="sxs-lookup"><span data-stu-id="a6f44-161">**Note:** `actor` is a special parameter that always takes the name of the caller.</span></span> <span data-ttu-id="a6f44-162">在委托呼叫中， `actor` 是用户的名称。</span><span class="sxs-lookup"><span data-stu-id="a6f44-162">In delegated calls, `actor` is the user's name.</span></span> <span data-ttu-id="a6f44-163">在仅限应用程序的调用中，它采用团队应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="a6f44-163">In application-only calls, it takes the name of the Teams app.</span></span>

### <a name="installing-the-teams-app"></a><span data-ttu-id="a6f44-164">安装团队应用程序</span><span class="sxs-lookup"><span data-stu-id="a6f44-164">Installing the Teams app</span></span>

<span data-ttu-id="a6f44-165">团队应用可以安装在团队、聊天或用户个人中，并且可以通过多种方式分发。</span><span class="sxs-lookup"><span data-stu-id="a6f44-165">Teams apps can be installed in a team, a chat, or for a user personally, and can be distributed in multiple ways.</span></span> <span data-ttu-id="a6f44-166">有关详细信息，请参阅 [团队应用程序分发方法](/microsoftteams/platform/concepts/deploy-and-publish/overview)。</span><span class="sxs-lookup"><span data-stu-id="a6f44-166">For details, see [Teams app distribution methods](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span></span> <span data-ttu-id="a6f44-167">通常情况下，推荐的是用于开发目的的 [旁加载](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-167">Typically, [sideloading](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) is preferred for development purposes.</span></span> <span data-ttu-id="a6f44-168">开发完成后，可以根据您是要分发到一个租户还是所有租户选择适当的分发方法。</span><span class="sxs-lookup"><span data-stu-id="a6f44-168">After development, you can choose the right distribution method based on whether you want to distribute to one tenant or to all tenants.</span></span>

<span data-ttu-id="a6f44-169">您还可以使用 [团队应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true) api 来管理团队应用程序安装。</span><span class="sxs-lookup"><span data-stu-id="a6f44-169">You can also use [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true) APIs to manage Teams app installations.</span></span>

## <a name="sending-activity-feed-notifications-to-users"></a><span data-ttu-id="a6f44-170">向用户发送活动源通知</span><span class="sxs-lookup"><span data-stu-id="a6f44-170">Sending activity feed notifications to users</span></span>

<span data-ttu-id="a6f44-171">由于可以为用户、团队中或聊天中的用户安装团队应用程序，因此也可以在以下三种上下文中发送通知：</span><span class="sxs-lookup"><span data-stu-id="a6f44-171">Because a Teams app can be installed for a user, in a team, or in a chat, the notifications can be sent in these three contexts as well:</span></span>

- [<span data-ttu-id="a6f44-172">在聊天中向用户发送通知</span><span class="sxs-lookup"><span data-stu-id="a6f44-172">Send notification to user in a chat</span></span>](/graph/api/chat-sendactivitynotification)
- [<span data-ttu-id="a6f44-173">向团队中的用户发送通知</span><span class="sxs-lookup"><span data-stu-id="a6f44-173">Send notification to user in a team</span></span>](/graph/api/team-sendactivitynotification)
- [<span data-ttu-id="a6f44-174">向用户发送通知</span><span class="sxs-lookup"><span data-stu-id="a6f44-174">Send notification to user</span></span>](/graph/api/userteamwork-sendactivitynotification)

<span data-ttu-id="a6f44-175">有关每个方案支持的主题的详细信息，请参阅特定的 Api。</span><span class="sxs-lookup"><span data-stu-id="a6f44-175">For details about what topics are supported for each scenario, see the specific APIs.</span></span> <span data-ttu-id="a6f44-176">所有方案都支持自定义基于文本的主题。</span><span class="sxs-lookup"><span data-stu-id="a6f44-176">Custom text-based topics are supported for all scenarios.</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="a6f44-177">示例1：通知用户在聊天中创建的任务</span><span class="sxs-lookup"><span data-stu-id="a6f44-177">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="a6f44-178">本示例演示如何为在聊天中创建的新任务发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="a6f44-178">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="a6f44-179">在这种情况下，团队应用必须安装在 Id 为的聊天中 `chatId` ，并且用户 `569363e2-4e49-4661-87f2-16f245c5d66a` 也必须是聊天的一部分。</span><span class="sxs-lookup"><span data-stu-id="a6f44-179">In this case, the Teams app must be installed in a chat with Id `chatId` and user `569363e2-4e49-4661-87f2-16f245c5d66a` must be part of the chat as well.</span></span>

#### <a name="request"></a><span data-ttu-id="a6f44-180">请求</span><span class="sxs-lookup"><span data-stu-id="a6f44-180">Request</span></span>
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
            "value": "12322"
        }
    ]
}

```

#### <a name="response"></a><span data-ttu-id="a6f44-181">响应</span><span class="sxs-lookup"><span data-stu-id="a6f44-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2--notify-a-user-about-a-task-created-in-a-team"></a><span data-ttu-id="a6f44-182">示例2：通知用户在团队中创建的任务</span><span class="sxs-lookup"><span data-stu-id="a6f44-182">Example 2 : Notify a user about a task created in a team</span></span>

<span data-ttu-id="a6f44-183">本示例演示如何向团队发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="a6f44-183">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="a6f44-184">本示例通知工作组所有者所创建的新任务需要关注。</span><span class="sxs-lookup"><span data-stu-id="a6f44-184">This example notifies the team owner about a new task created that requires their attention.</span></span>

#### <a name="request"></a><span data-ttu-id="a6f44-185">请求</span><span class="sxs-lookup"><span data-stu-id="a6f44-185">Request</span></span>
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
            "value": "12322"
        }
    ]
}

```

#### <a name="response"></a><span data-ttu-id="a6f44-186">响应</span><span class="sxs-lookup"><span data-stu-id="a6f44-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a><span data-ttu-id="a6f44-187">示例3：使用自定义主题通知用户事件</span><span class="sxs-lookup"><span data-stu-id="a6f44-187">Example 3: Notify a user about an event using a custom topic</span></span>

<span data-ttu-id="a6f44-188">如前面的示例中所示，您可以链接到团队的不同方面或聊天。</span><span class="sxs-lookup"><span data-stu-id="a6f44-188">As seen in the previous examples, you can link to different aspects of a team or a chat.</span></span> <span data-ttu-id="a6f44-189">但是，如果要链接到不属于团队的方位或者不是由 Microsoft Graph 表示的方位，或者如果您想要自定义该名称，则可以为其设置 "to" 的来源 `topic` `text` 并为其传入自定义值。</span><span class="sxs-lookup"><span data-stu-id="a6f44-189">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or if you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="a6f44-190">此外， `webUrl` 当您使用源作为时，也是必需的 `topic` `text` 。</span><span class="sxs-lookup"><span data-stu-id="a6f44-190">Additionally, `webUrl` is required when you use `topic` source as `text`.</span></span>

<span data-ttu-id="a6f44-191">以下所示的 Yammer 通知示例使用自定义主题，因为 Microsoft Graph 不支持 Yammer 的资源。</span><span class="sxs-lookup"><span data-stu-id="a6f44-191">The Yammer notification example shown earlier uses a custom topic because Yammer's resources are not supported by Microsoft Graph.</span></span>

> <span data-ttu-id="a6f44-192">**注意：** `webUrl` 必须从 Microsoft 团队域 (teams.microsoft.com （例如) ）开始。</span><span class="sxs-lookup"><span data-stu-id="a6f44-192">**Note:** `webUrl` must start with the Microsoft Teams domain (teams.microsoft.com for example).</span></span>

#### <a name="request"></a><span data-ttu-id="a6f44-193">请求</span><span class="sxs-lookup"><span data-stu-id="a6f44-193">Request</span></span>
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
    "activityType": "approvalRequired",
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

#### <a name="response"></a><span data-ttu-id="a6f44-194">响应</span><span class="sxs-lookup"><span data-stu-id="a6f44-194">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a><span data-ttu-id="a6f44-195">自定义通知通知方式</span><span class="sxs-lookup"><span data-stu-id="a6f44-195">Customizing how the notifications alert you</span></span>

<span data-ttu-id="a6f44-196">Microsoft 团队用户可以自定义他们在其订阅源中看到的通知，作为横幅，等等。</span><span class="sxs-lookup"><span data-stu-id="a6f44-196">Microsoft Teams users can customize the notifications they see in their feed, as a banner, and so on.</span></span> <span data-ttu-id="a6f44-197">通过活动源 Api 生成的通知也可以自定义。</span><span class="sxs-lookup"><span data-stu-id="a6f44-197">Notifications generated through activity feed APIs can also be customized.</span></span> <span data-ttu-id="a6f44-198">用户可以通过 Microsoft 团队中的设置来选择如何通知他们。</span><span class="sxs-lookup"><span data-stu-id="a6f44-198">Users can choose how they are notified via settings in Microsoft Teams.</span></span> <span data-ttu-id="a6f44-199">团队应用程序将显示在列表中供用户选择，如下面的屏幕截图中所示。</span><span class="sxs-lookup"><span data-stu-id="a6f44-199">Teams apps will appear in the list for the user to choose from, as shown in the following screenshot.</span></span>

![团队中通知设置的屏幕截图，其中突出显示了 "自定义" 选项](images/teams-activityfeednotifications/notificationsettings.png)

<span data-ttu-id="a6f44-201">用户可以单击应用程序旁边的 " **编辑** "，然后自定义通知，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="a6f44-201">Users can click **Edit** next to an app and customize the notifications, as shown in the following example.</span></span> <span data-ttu-id="a6f44-202">将 `description` 显示 "团队" 应用程序清单中的字段。</span><span class="sxs-lookup"><span data-stu-id="a6f44-202">The `description` field in the Teams app manifest is displayed.</span></span>

![显示针对团队应用程序的横幅和订阅源自定义通知的屏幕截图](images/teams-activityfeednotifications/applevelnotificationsettings.png)
