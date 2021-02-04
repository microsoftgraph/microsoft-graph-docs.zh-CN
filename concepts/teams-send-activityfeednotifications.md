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
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a>向 Microsoft Teams 中的用户发送活动源通知

Microsoft Teams 活动源允许用户通过通知用户更改来对需要关注的项目进行分类。 可以使用 Microsoft Graph 中的活动源通知 API 将此功能扩展到你的应用。 这允许应用通过帮助用户了解其使用的工具和工作流中的更改，从而提供更丰富的体验并更好地吸引用户。

## <a name="understanding-the-basics-of-activity-feed-notification"></a>了解活动源通知的基础知识

Microsoft Teams 中的活动源通知由多位信息组成，一起显示，如下图所示。

![显示活动源通知的组件的图像](images/teams-activityfeednotifications/notificationtemplate.png)

这些组件包括：
- 发起活动的人
- 表示活动类型的图标
- 参与者执行活动的原因
- 文本预览
- 时间戳
- 活动的位置

以下示例显示这些组件如何一起提供有关通知的详细信息。 此示例是有关 Yammer 社区中提及的用户的通知。

![Yammer 操作通知示例](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a>使用活动源通知 API 的要求

活动源 API 与 [Teams 应用一起工作](/microsoftteams/platform/overview)。 以下是发送活动源通知的要求：

- Teams 应用清单必须将 Azure AD 应用 ID 添加到 `webApplicationInfo` 该部分。 有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。
- 活动类型必须在节中 `activities` 声明。 有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。
- 必须亲自或在团队或聊天中为收件人安装 Teams 应用。 [](/graph/api/resources/team?preserve-view=true) [](/graph/api/resources/chat?preserve-view=true) 有关详细信息，请参阅 [Teams 应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true)。

### <a name="teams-app-manifest-changes"></a>Teams 应用清单更改

本部分介绍需要添加到 Teams 应用清单的更改。 请注意，你必须使用 Teams [应用](/microsoftteams/platform/resources/schema/manifest-schema) 清单版本 `1.7` 或更高版本。

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a>webApplicationInfo 节更改

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|参数|类型|说明|
|:---|:---|:---|
|id|string|Azure AD 应用 ID (客户端 ID) 。|
|resource|string|与 Azure AD 应用关联的资源。 也称为 Azure 门户中的回复或重定向 URL。|

> **注意：** 如果团队、聊天或用户 (同一 Azure AD 应用，) Teams 应用可能出现错误。 确保你使用的是唯一的 Azure AD 应用。

#### <a name="activities-section-changes"></a>activities 节更改

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

|参数|类型|Description|
|:---|:---|:---|
|类型|string|活动的类型。 这需要在特定的清单中是唯一的。|
|说明|string|可读的简短说明。 这将在 Microsoft Teams 客户端上可见。|
|templateText|string|活动通知的模板文本。 可以通过在 中封装参数来声明参数 `{}` 。|

>**注意：** `actor` 是一个始终采用调用方名称的特殊参数。 在委派呼叫中 `actor` ，是用户名。 在仅应用程序调用中，它采用 Teams 应用的名称。

### <a name="installing-the-teams-app"></a>安装 Teams 应用

Teams 应用可以安装在团队、聊天或用户个人中，并且可以通过多种方式分发。 有关详细信息，请参阅 [Teams 应用分发方法](/microsoftteams/platform/concepts/deploy-and-publish/overview)。 通常， [旁加载](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) 优先用于开发目的。 开发后，您可以基于要分发到一个租户还是所有租户来选择正确的分发方法。

还可使用 [Teams 应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true) API 管理 Teams 应用安装。

## <a name="sending-activity-feed-notifications-to-users"></a>向用户发送活动源通知

由于可以为用户、团队或聊天中安装 Teams 应用，因此也可在以下三种上下文中发送通知：

- [在聊天中向用户发送通知](/graph/api/chat-sendactivitynotification)
- [向团队中的用户发送通知](/graph/api/team-sendactivitynotification)
- [向用户发送通知](/graph/api/userteamwork-sendactivitynotification)

有关每种方案支持的主题的详细信息，请参阅特定 API。 所有方案都支持基于文本的自定义主题。

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>示例 1：通知用户在聊天中创建的任务

此示例演示如何为聊天中创建的新任务发送活动源通知。 在这种情况下，Teams 应用必须安装在具有 ID 的聊天中，用户也必须是聊天的 `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` 一部分。

#### <a name="request"></a>请求
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

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a>示例 2：通知用户有关在团队中创建的任务

此示例演示如何为团队发送活动源通知。 此示例通知工作组所有者需要关注的新任务。

#### <a name="request"></a>请求
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

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a>示例 3：使用自定义主题向用户通知事件

如前面的示例所示，你可以链接到团队或聊天的不同方面。 但是，如果你想要链接到不是团队的一部分或不由 Microsoft Graph 表示的方面，或者如果你想要自定义名称，你可以将源设置为并传递它的自定义 `topic` `text` 值。 此外， `webUrl` 将源用作时 `topic` 是必需的 `text` 。

前面显示的 Yammer 通知示例使用自定义主题，因为 Microsoft Graph 不支持 Yammer 的资源。

> **注意：** `webUrl` 必须以 Microsoft Teams 域域 (teams.microsoft.com例如) 。

#### <a name="request"></a>请求
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

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a>自定义通知通知的提醒

Microsoft Teams 用户可以自定义在源中查看的通知，作为横幅等。 还可自定义通过活动源 API 生成的通知。 用户可以选择如何通过 Microsoft Teams 中的设置通知他们。 Teams 应用将显示在列表中，供用户进行选择，如以下屏幕截图所示。

![Teams 中的通知设置的屏幕截图，其中突出显示了"自定义"选项](images/teams-activityfeednotifications/notificationsettings.png)

用户可以单击 **应用** 旁边的"编辑"并自定义通知，如以下示例所示。 将显示 `description` Teams 应用清单中的字段。

![Screenshot showing notifications customized to Banner and feed for a Teams app](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a>常见问题

### <a name="who-needs-to-install-the-teams-app"></a>谁需要安装 Teams 应用？

目标用户必须已安装正在发送通知的 Teams 应用。

### <a name="can-a-user-send-notifications-to-themselves"></a>用户能否向自己发送通知？

否，用户无法向自己发送通知。 对于此方案，请使用应用程序权限。

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a>Teams 应用能否控制通知如何向用户显示？

否，仅允许用户更改通知设置。

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a>我安装了我的应用，为什么在用户帐户下看不到通知设置？

设置将在 Teams 应用发送第一个通知后显示。 这将减少用户看到的设置数。

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a>我开始使用 409 (冲突) ，如何解决该问题？

`Conflict` 错误主要发生在同一范围内安装的多个 Teams 应用 (团队、聊天、用户等) 清单部分中具有相同的 Azure AD `webApplicationInfo` appId。 发生这种情况时，你将被获取一个错误，例如 `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.` 。 确保将唯一的 Azure AD 应用用于唯一的 Teams 应用。 请注意，可以在多个范围内为团队 + (用户安装同一个 Teams) 。


