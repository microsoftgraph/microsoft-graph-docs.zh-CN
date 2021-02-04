---
title: 向 Microsoft Teams 中的用户发送活动源通知
description: 使用 Teams 应用和 Microsoft graph 向 Microsoft Teams 中的用户发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 940ffba39293a3b01df67c47b6ff6b5e09821767
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101893"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a><span data-ttu-id="72f9b-103">向 Microsoft Teams 中的用户发送活动源通知</span><span class="sxs-lookup"><span data-stu-id="72f9b-103">Send activity feed notifications to users in Microsoft Teams</span></span>

<span data-ttu-id="72f9b-104">Microsoft Teams 活动源允许用户通过通知用户更改来对需要关注的项目进行分类。</span><span class="sxs-lookup"><span data-stu-id="72f9b-104">The Microsoft Teams activity feed enables users to triage items that require attention by notifying them of changes.</span></span> <span data-ttu-id="72f9b-105">可以使用 Microsoft Graph 中的活动源通知 API 将此功能扩展到你的应用。</span><span class="sxs-lookup"><span data-stu-id="72f9b-105">You can use the activity feed notification APIs in Microsoft Graph to extend this functionality to your apps.</span></span> <span data-ttu-id="72f9b-106">这允许应用通过帮助用户了解其使用的工具和工作流中的更改，从而提供更丰富的体验并更好地吸引用户。</span><span class="sxs-lookup"><span data-stu-id="72f9b-106">This allows your apps to provide richer experiences and better engage users by helping to keep them up to date with changes in the tools and workflows they use.</span></span>

## <a name="understanding-the-basics-of-activity-feed-notification"></a><span data-ttu-id="72f9b-107">了解活动源通知的基础知识</span><span class="sxs-lookup"><span data-stu-id="72f9b-107">Understanding the basics of activity feed notification</span></span>

<span data-ttu-id="72f9b-108">Microsoft Teams 中的活动源通知由多位信息组成，一起显示，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="72f9b-108">Activity feed notifications in Microsoft Teams are comprised of multiple bits of information, displayed together, as shown in the following image.</span></span>

![显示活动源通知的组件的图像](images/teams-activityfeednotifications/notificationtemplate.png)

<span data-ttu-id="72f9b-110">这些组件包括：</span><span class="sxs-lookup"><span data-stu-id="72f9b-110">The components include:</span></span>
- <span data-ttu-id="72f9b-111">发起活动的人</span><span class="sxs-lookup"><span data-stu-id="72f9b-111">The actor who initiated the activity</span></span>
- <span data-ttu-id="72f9b-112">表示活动类型的图标</span><span class="sxs-lookup"><span data-stu-id="72f9b-112">An icon that represents the activity type</span></span>
- <span data-ttu-id="72f9b-113">参与者执行活动的原因</span><span class="sxs-lookup"><span data-stu-id="72f9b-113">The reason the actor did the activity</span></span>
- <span data-ttu-id="72f9b-114">文本预览</span><span class="sxs-lookup"><span data-stu-id="72f9b-114">A text preview</span></span>
- <span data-ttu-id="72f9b-115">时间戳</span><span class="sxs-lookup"><span data-stu-id="72f9b-115">A time stamp</span></span>
- <span data-ttu-id="72f9b-116">活动的位置</span><span class="sxs-lookup"><span data-stu-id="72f9b-116">The location of the activity</span></span>

<span data-ttu-id="72f9b-117">以下示例显示这些组件如何一起提供有关通知的详细信息。</span><span class="sxs-lookup"><span data-stu-id="72f9b-117">The following example shows how these components together provide the details about a notification.</span></span> <span data-ttu-id="72f9b-118">此示例是有关 Yammer 社区中提及的用户的通知。</span><span class="sxs-lookup"><span data-stu-id="72f9b-118">This example is a notification about a user mentioned in a Yammer community.</span></span>

![Yammer 操作通知示例](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a><span data-ttu-id="72f9b-120">使用活动源通知 API 的要求</span><span class="sxs-lookup"><span data-stu-id="72f9b-120">Requirements for using the activity feed notification APIs</span></span>

<span data-ttu-id="72f9b-121">活动源 API 与 [Teams 应用一起工作](/microsoftteams/platform/overview)。</span><span class="sxs-lookup"><span data-stu-id="72f9b-121">Activity feed APIs work with a [Teams app](/microsoftteams/platform/overview).</span></span> <span data-ttu-id="72f9b-122">以下是发送活动源通知的要求：</span><span class="sxs-lookup"><span data-stu-id="72f9b-122">The following are the requirements for sending activity feed notifications:</span></span>

- <span data-ttu-id="72f9b-123">Teams 应用清单必须将 Azure AD 应用 ID 添加到 `webApplicationInfo` 该部分。</span><span class="sxs-lookup"><span data-stu-id="72f9b-123">The Teams app manifest must have the Azure AD app ID added to the `webApplicationInfo` section.</span></span> <span data-ttu-id="72f9b-124">有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。</span><span class="sxs-lookup"><span data-stu-id="72f9b-124">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="72f9b-125">活动类型必须在节中 `activities` 声明。</span><span class="sxs-lookup"><span data-stu-id="72f9b-125">Activity types must be declared in the `activities` section.</span></span> <span data-ttu-id="72f9b-126">有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。</span><span class="sxs-lookup"><span data-stu-id="72f9b-126">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="72f9b-127">必须亲自或在团队或聊天中为收件人安装 Teams 应用。 [](/graph/api/resources/team?preserve-view=true) [](/graph/api/resources/chat?preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="72f9b-127">The Teams app must be installed for the recipient, either personally, or in a [team](/graph/api/resources/team?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true) they are part of.</span></span> <span data-ttu-id="72f9b-128">有关详细信息，请参阅 [Teams 应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="72f9b-128">For more information, see [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true).</span></span>

### <a name="teams-app-manifest-changes"></a><span data-ttu-id="72f9b-129">Teams 应用清单更改</span><span class="sxs-lookup"><span data-stu-id="72f9b-129">Teams app manifest changes</span></span>

<span data-ttu-id="72f9b-130">本部分介绍需要添加到 Teams 应用清单的更改。</span><span class="sxs-lookup"><span data-stu-id="72f9b-130">This section describes the changes that need to be added to Teams app manifest.</span></span> <span data-ttu-id="72f9b-131">请注意，你必须使用 Teams [应用](/microsoftteams/platform/resources/schema/manifest-schema) 清单版本 `1.7` 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="72f9b-131">Note that you must be using the [Teams app manifest](/microsoftteams/platform/resources/schema/manifest-schema) version `1.7` or greater.</span></span>

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a><span data-ttu-id="72f9b-132">webApplicationInfo 节更改</span><span class="sxs-lookup"><span data-stu-id="72f9b-132">webApplicationInfo section changes</span></span>

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|<span data-ttu-id="72f9b-133">参数</span><span class="sxs-lookup"><span data-stu-id="72f9b-133">Parameter</span></span>|<span data-ttu-id="72f9b-134">类型</span><span class="sxs-lookup"><span data-stu-id="72f9b-134">Type</span></span>|<span data-ttu-id="72f9b-135">说明</span><span class="sxs-lookup"><span data-stu-id="72f9b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72f9b-136">id</span><span class="sxs-lookup"><span data-stu-id="72f9b-136">id</span></span>|<span data-ttu-id="72f9b-137">string</span><span class="sxs-lookup"><span data-stu-id="72f9b-137">string</span></span>|<span data-ttu-id="72f9b-138">Azure AD 应用 ID (客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="72f9b-138">Azure AD app ID (client ID).</span></span>|
|<span data-ttu-id="72f9b-139">resource</span><span class="sxs-lookup"><span data-stu-id="72f9b-139">resource</span></span>|<span data-ttu-id="72f9b-140">string</span><span class="sxs-lookup"><span data-stu-id="72f9b-140">string</span></span>|<span data-ttu-id="72f9b-141">与 Azure AD 应用关联的资源。</span><span class="sxs-lookup"><span data-stu-id="72f9b-141">Resource associated with the Azure AD app.</span></span> <span data-ttu-id="72f9b-142">也称为 Azure 门户中的回复或重定向 URL。</span><span class="sxs-lookup"><span data-stu-id="72f9b-142">Also known as reply or redirect URL in the Azure Portal.</span></span>|

> <span data-ttu-id="72f9b-143">**注意：** 如果团队、聊天或用户 (同一 Azure AD 应用，) Teams 应用可能出现错误。</span><span class="sxs-lookup"><span data-stu-id="72f9b-143">**Note:** You might get an error if multiple Teams apps in the same scope (team, chat or user) are using the same Azure AD app.</span></span> <span data-ttu-id="72f9b-144">确保你使用的是唯一的 Azure AD 应用。</span><span class="sxs-lookup"><span data-stu-id="72f9b-144">Make sure that you're using unique Azure AD apps.</span></span>

#### <a name="activities-section-changes"></a><span data-ttu-id="72f9b-145">activities 节更改</span><span class="sxs-lookup"><span data-stu-id="72f9b-145">activities section changes</span></span>

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

|<span data-ttu-id="72f9b-146">参数</span><span class="sxs-lookup"><span data-stu-id="72f9b-146">Parameter</span></span>|<span data-ttu-id="72f9b-147">类型</span><span class="sxs-lookup"><span data-stu-id="72f9b-147">Type</span></span>|<span data-ttu-id="72f9b-148">Description</span><span class="sxs-lookup"><span data-stu-id="72f9b-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72f9b-149">类型</span><span class="sxs-lookup"><span data-stu-id="72f9b-149">type</span></span>|<span data-ttu-id="72f9b-150">string</span><span class="sxs-lookup"><span data-stu-id="72f9b-150">string</span></span>|<span data-ttu-id="72f9b-151">活动的类型。</span><span class="sxs-lookup"><span data-stu-id="72f9b-151">Type of activity.</span></span> <span data-ttu-id="72f9b-152">这需要在特定的清单中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="72f9b-152">This needs to be unique in a specific manifest.</span></span>|
|<span data-ttu-id="72f9b-153">说明</span><span class="sxs-lookup"><span data-stu-id="72f9b-153">description</span></span>|<span data-ttu-id="72f9b-154">string</span><span class="sxs-lookup"><span data-stu-id="72f9b-154">string</span></span>|<span data-ttu-id="72f9b-155">可读的简短说明。</span><span class="sxs-lookup"><span data-stu-id="72f9b-155">Human-readable short description.</span></span> <span data-ttu-id="72f9b-156">这将在 Microsoft Teams 客户端上可见。</span><span class="sxs-lookup"><span data-stu-id="72f9b-156">This will be visible on the Microsoft Teams client.</span></span>|
|<span data-ttu-id="72f9b-157">templateText</span><span class="sxs-lookup"><span data-stu-id="72f9b-157">templateText</span></span>|<span data-ttu-id="72f9b-158">string</span><span class="sxs-lookup"><span data-stu-id="72f9b-158">string</span></span>|<span data-ttu-id="72f9b-159">活动通知的模板文本。</span><span class="sxs-lookup"><span data-stu-id="72f9b-159">Template text for the activity notification.</span></span> <span data-ttu-id="72f9b-160">可以通过在 中封装参数来声明参数 `{}` 。</span><span class="sxs-lookup"><span data-stu-id="72f9b-160">You can declare your parameters by encapsulating parameters in `{}`.</span></span>|

><span data-ttu-id="72f9b-161">**注意：** `actor` 是一个始终采用调用方名称的特殊参数。</span><span class="sxs-lookup"><span data-stu-id="72f9b-161">**Note:** `actor` is a special parameter that always takes the name of the caller.</span></span> <span data-ttu-id="72f9b-162">在委派呼叫中 `actor` ，是用户名。</span><span class="sxs-lookup"><span data-stu-id="72f9b-162">In delegated calls, `actor` is the user's name.</span></span> <span data-ttu-id="72f9b-163">在仅应用程序调用中，它采用 Teams 应用的名称。</span><span class="sxs-lookup"><span data-stu-id="72f9b-163">In application-only calls, it takes the name of the Teams app.</span></span>

### <a name="installing-the-teams-app"></a><span data-ttu-id="72f9b-164">安装 Teams 应用</span><span class="sxs-lookup"><span data-stu-id="72f9b-164">Installing the Teams app</span></span>

<span data-ttu-id="72f9b-165">Teams 应用可以安装在团队、聊天或用户个人中，并且可以通过多种方式分发。</span><span class="sxs-lookup"><span data-stu-id="72f9b-165">Teams apps can be installed in a team, a chat, or for a user personally, and can be distributed in multiple ways.</span></span> <span data-ttu-id="72f9b-166">有关详细信息，请参阅 [Teams 应用分发方法](/microsoftteams/platform/concepts/deploy-and-publish/overview)。</span><span class="sxs-lookup"><span data-stu-id="72f9b-166">For details, see [Teams app distribution methods](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span></span> <span data-ttu-id="72f9b-167">通常， [旁加载](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) 优先用于开发目的。</span><span class="sxs-lookup"><span data-stu-id="72f9b-167">Typically, [sideloading](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) is preferred for development purposes.</span></span> <span data-ttu-id="72f9b-168">开发后，您可以基于要分发到一个租户还是所有租户来选择正确的分发方法。</span><span class="sxs-lookup"><span data-stu-id="72f9b-168">After development, you can choose the right distribution method based on whether you want to distribute to one tenant or to all tenants.</span></span>

<span data-ttu-id="72f9b-169">还可使用 [Teams 应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true) API 管理 Teams 应用安装。</span><span class="sxs-lookup"><span data-stu-id="72f9b-169">You can also use [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true) APIs to manage Teams app installations.</span></span>

## <a name="sending-activity-feed-notifications-to-users"></a><span data-ttu-id="72f9b-170">向用户发送活动源通知</span><span class="sxs-lookup"><span data-stu-id="72f9b-170">Sending activity feed notifications to users</span></span>

<span data-ttu-id="72f9b-171">由于可以为用户、团队或聊天中安装 Teams 应用，因此也可在以下三种上下文中发送通知：</span><span class="sxs-lookup"><span data-stu-id="72f9b-171">Because a Teams app can be installed for a user, in a team, or in a chat, the notifications can be sent in these three contexts as well:</span></span>

- [<span data-ttu-id="72f9b-172">在聊天中向用户发送通知</span><span class="sxs-lookup"><span data-stu-id="72f9b-172">Send notification to user in a chat</span></span>](/graph/api/chat-sendactivitynotification)
- [<span data-ttu-id="72f9b-173">向团队中的用户发送通知</span><span class="sxs-lookup"><span data-stu-id="72f9b-173">Send notification to user in a team</span></span>](/graph/api/team-sendactivitynotification)
- [<span data-ttu-id="72f9b-174">向用户发送通知</span><span class="sxs-lookup"><span data-stu-id="72f9b-174">Send notification to user</span></span>](/graph/api/userteamwork-sendactivitynotification)

<span data-ttu-id="72f9b-175">有关每种方案支持的主题的详细信息，请参阅特定 API。</span><span class="sxs-lookup"><span data-stu-id="72f9b-175">For details about what topics are supported for each scenario, see the specific APIs.</span></span> <span data-ttu-id="72f9b-176">所有方案都支持基于文本的自定义主题。</span><span class="sxs-lookup"><span data-stu-id="72f9b-176">Custom text-based topics are supported for all scenarios.</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="72f9b-177">示例 1：通知用户在聊天中创建的任务</span><span class="sxs-lookup"><span data-stu-id="72f9b-177">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="72f9b-178">此示例演示如何为聊天中创建的新任务发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="72f9b-178">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="72f9b-179">在这种情况下，Teams 应用必须安装在具有 ID 的聊天中，用户也必须是聊天的 `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` 一部分。</span><span class="sxs-lookup"><span data-stu-id="72f9b-179">In this case, the Teams app must be installed in a chat with Id `chatId` and user `569363e2-4e49-4661-87f2-16f245c5d66a` must be part of the chat as well.</span></span>

#### <a name="request"></a><span data-ttu-id="72f9b-180">请求</span><span class="sxs-lookup"><span data-stu-id="72f9b-180">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="72f9b-181">响应</span><span class="sxs-lookup"><span data-stu-id="72f9b-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a><span data-ttu-id="72f9b-182">示例 2：通知用户有关在团队中创建的任务</span><span class="sxs-lookup"><span data-stu-id="72f9b-182">Example 2: Notify a user about a task created in a team</span></span>

<span data-ttu-id="72f9b-183">此示例演示如何为团队发送活动源通知。</span><span class="sxs-lookup"><span data-stu-id="72f9b-183">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="72f9b-184">此示例通知工作组所有者需要关注的新任务。</span><span class="sxs-lookup"><span data-stu-id="72f9b-184">This example notifies the team owner about a new task created that requires their attention.</span></span>

#### <a name="request"></a><span data-ttu-id="72f9b-185">请求</span><span class="sxs-lookup"><span data-stu-id="72f9b-185">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="72f9b-186">响应</span><span class="sxs-lookup"><span data-stu-id="72f9b-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a><span data-ttu-id="72f9b-187">示例 3：使用自定义主题向用户通知事件</span><span class="sxs-lookup"><span data-stu-id="72f9b-187">Example 3: Notify a user about an event using a custom topic</span></span>

<span data-ttu-id="72f9b-188">如前面的示例所示，你可以链接到团队或聊天的不同方面。</span><span class="sxs-lookup"><span data-stu-id="72f9b-188">As seen in the previous examples, you can link to different aspects of a team or a chat.</span></span> <span data-ttu-id="72f9b-189">但是，如果你想要链接到不是团队的一部分或不由 Microsoft Graph 表示的方面，或者如果你想要自定义名称，你可以将源设置为并传递它的自定义 `topic` `text` 值。</span><span class="sxs-lookup"><span data-stu-id="72f9b-189">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or if you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="72f9b-190">此外， `webUrl` 将源用作时 `topic` 是必需的 `text` 。</span><span class="sxs-lookup"><span data-stu-id="72f9b-190">Additionally, `webUrl` is required when you use `topic` source as `text`.</span></span>

<span data-ttu-id="72f9b-191">前面显示的 Yammer 通知示例使用自定义主题，因为 Microsoft Graph 不支持 Yammer 的资源。</span><span class="sxs-lookup"><span data-stu-id="72f9b-191">The Yammer notification example shown earlier uses a custom topic because Yammer's resources are not supported by Microsoft Graph.</span></span>

> <span data-ttu-id="72f9b-192">**注意：** `webUrl` 必须以 Microsoft Teams 域域 (teams.microsoft.com例如) 。</span><span class="sxs-lookup"><span data-stu-id="72f9b-192">**Note:** `webUrl` must start with the Microsoft Teams domain (teams.microsoft.com for example).</span></span>

#### <a name="request"></a><span data-ttu-id="72f9b-193">请求</span><span class="sxs-lookup"><span data-stu-id="72f9b-193">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="72f9b-194">响应</span><span class="sxs-lookup"><span data-stu-id="72f9b-194">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a><span data-ttu-id="72f9b-195">自定义通知通知的提醒</span><span class="sxs-lookup"><span data-stu-id="72f9b-195">Customizing how the notifications alert you</span></span>

<span data-ttu-id="72f9b-196">Microsoft Teams 用户可以自定义在源中查看的通知，作为横幅等。</span><span class="sxs-lookup"><span data-stu-id="72f9b-196">Microsoft Teams users can customize the notifications they see in their feed, as a banner, and so on.</span></span> <span data-ttu-id="72f9b-197">还可自定义通过活动源 API 生成的通知。</span><span class="sxs-lookup"><span data-stu-id="72f9b-197">Notifications generated through activity feed APIs can also be customized.</span></span> <span data-ttu-id="72f9b-198">用户可以选择如何通过 Microsoft Teams 中的设置通知他们。</span><span class="sxs-lookup"><span data-stu-id="72f9b-198">Users can choose how they are notified via settings in Microsoft Teams.</span></span> <span data-ttu-id="72f9b-199">Teams 应用将显示在列表中，供用户进行选择，如以下屏幕截图所示。</span><span class="sxs-lookup"><span data-stu-id="72f9b-199">Teams apps will appear in the list for the user to choose from, as shown in the following screenshot.</span></span>

![Teams 中的通知设置的屏幕截图，其中突出显示了"自定义"选项](images/teams-activityfeednotifications/notificationsettings.png)

<span data-ttu-id="72f9b-201">用户可以单击 **应用** 旁边的"编辑"并自定义通知，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="72f9b-201">Users can click **Edit** next to an app and customize the notifications, as shown in the following example.</span></span> <span data-ttu-id="72f9b-202">将显示 `description` Teams 应用清单中的字段。</span><span class="sxs-lookup"><span data-stu-id="72f9b-202">The `description` field in the Teams app manifest is displayed.</span></span>

![Screenshot showing notifications customized to Banner and feed for a Teams app](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a><span data-ttu-id="72f9b-204">常见问题</span><span class="sxs-lookup"><span data-stu-id="72f9b-204">FAQs</span></span>

### <a name="who-needs-to-install-the-teams-app"></a><span data-ttu-id="72f9b-205">谁需要安装 Teams 应用？</span><span class="sxs-lookup"><span data-stu-id="72f9b-205">Who needs to install the Teams app?</span></span>

<span data-ttu-id="72f9b-206">目标用户必须已安装正在发送通知的 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="72f9b-206">The target user must have the Teams app that is sending notifications installed.</span></span>

### <a name="can-a-user-send-notifications-to-themselves"></a><span data-ttu-id="72f9b-207">用户能否向自己发送通知？</span><span class="sxs-lookup"><span data-stu-id="72f9b-207">Can a user send notifications to themselves?</span></span>

<span data-ttu-id="72f9b-208">否，用户无法向自己发送通知。</span><span class="sxs-lookup"><span data-stu-id="72f9b-208">No, a user cannot send notifications to themselves.</span></span> <span data-ttu-id="72f9b-209">对于此方案，请使用应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="72f9b-209">For this scenario, use application permissions.</span></span>

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a><span data-ttu-id="72f9b-210">Teams 应用能否控制通知如何向用户显示？</span><span class="sxs-lookup"><span data-stu-id="72f9b-210">Can a Teams app control how the notifications are shown to the user?</span></span>

<span data-ttu-id="72f9b-211">否，仅允许用户更改通知设置。</span><span class="sxs-lookup"><span data-stu-id="72f9b-211">No, only users are allowed to change notification settings.</span></span>

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a><span data-ttu-id="72f9b-212">我安装了我的应用，为什么在用户帐户下看不到通知设置？</span><span class="sxs-lookup"><span data-stu-id="72f9b-212">I installed my app, why don't I see notification settings under the user account?</span></span>

<span data-ttu-id="72f9b-213">设置将在 Teams 应用发送第一个通知后显示。</span><span class="sxs-lookup"><span data-stu-id="72f9b-213">The settings will appear after the first notification is sent by the Teams app.</span></span> <span data-ttu-id="72f9b-214">这将减少用户看到的设置数。</span><span class="sxs-lookup"><span data-stu-id="72f9b-214">This reduces the number of settings that users see.</span></span>

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a><span data-ttu-id="72f9b-215">我开始使用 409 (冲突) ，如何解决该问题？</span><span class="sxs-lookup"><span data-stu-id="72f9b-215">I started getting a 409 (conflict) error, how do I resolve it?</span></span>

<span data-ttu-id="72f9b-216">`Conflict` 错误主要发生在同一范围内安装的多个 Teams 应用 (团队、聊天、用户等) 清单部分中具有相同的 Azure AD `webApplicationInfo` appId。</span><span class="sxs-lookup"><span data-stu-id="72f9b-216">`Conflict` errors primarily occur when multiple Teams apps installed in the same scope (team, chat, user, and so on) have the same Azure AD appId in the `webApplicationInfo` section of the manifest.</span></span> <span data-ttu-id="72f9b-217">发生这种情况时，你将被获取一个错误，例如 `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.` 。</span><span class="sxs-lookup"><span data-stu-id="72f9b-217">When this happens, you will get an error such as `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.`.</span></span> <span data-ttu-id="72f9b-218">确保将唯一的 Azure AD 应用用于唯一的 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="72f9b-218">Make sure that you use unique Azure AD apps for unique Teams apps.</span></span> <span data-ttu-id="72f9b-219">请注意，可以在多个范围内为团队 + (用户安装同一个 Teams) 。</span><span class="sxs-lookup"><span data-stu-id="72f9b-219">Note that you can have the same Teams app installed in multiple scopes (team + user for example).</span></span>


