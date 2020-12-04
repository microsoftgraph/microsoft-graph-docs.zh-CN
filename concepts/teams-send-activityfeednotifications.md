---
title: 向 Microsoft 团队中的用户发送活动源通知
description: 使用团队应用和 microsoft graph 将活动源通知发送给 Microsoft 团队中的用户。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 698a5ed338906f8eed2d2611c8aba3b4f0b6f624
ms.sourcegitcommit: c419bb8901b7766af193196f80bc1d497643fcb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49572119"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a>向 Microsoft 团队中的用户发送活动源通知

Microsoft 团队活动源使用户能够通过通知所做的更改来会审需要注意的项目。 您可以使用 Microsoft Graph 中的活动源通知 Api 将此功能扩展到您的应用程序。 这样一来，你的应用程序可以提供更丰富的体验，并通过帮助保持他们所使用的工具和工作流中的更改来保持最新。

## <a name="understanding-the-basics-of-activity-feed-notification"></a>了解活动源通知的基础知识

Microsoft 团队中的活动源通知由多个位的信息组成，显示在一起，如下图所示。

![显示活动源通知组件的图像](images/teams-activityfeednotifications/notificationtemplate.png)

这些组件包括：
- 启动活动的参与者
- 一个代表活动类型的图标
- 主角执行活动的原因
- 文本预览
- 一个时间戳
- 活动的位置

下面的示例演示这些组件如何共同提供有关通知的详细信息。 本示例是关于 Yammer 社区中提到的用户的通知。

![Yammer actifity 通知示例](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a>使用活动源通知 Api 的要求

活动源 Api 与 [团队应用](/microsoftteams/platform/overview)一起使用。 以下是发送活动源通知的要求：

- 团队应用程序清单必须向分区添加了 Azure AD 应用 ID `webApplicationInfo` 。 有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。
- 必须在 "" 部分声明活动类型 `activities` 。 有关详细信息，请参阅 [清单架构](/microsoftteams/platform/resources/schema/manifest-schema)。
- 必须为收件人（个人身份）或 [团队或团队](/graph/api/resources/team?preserve-view=true) 中的团队用户安装团队应用程序或 [聊天](/graph/api/resources/chat?preserve-view=true) 。 有关详细信息，请参阅 [团队应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true)。

### <a name="teams-app-manifest-changes"></a>团队应用程序清单更改

本节介绍了需要添加到团队应用程序清单中的更改。 请注意，您必须使用 [团队应用程序清单](/microsoftteams/platform/resources/schema/manifest-schema) 版本 `1.7` 或更高版本。

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
|resource|string|与 Azure AD 应用关联的资源。 在 Azure 门户中也称为 "答复" 或 "重定向 URL"。|

> **注意：** 如果同一作用域中的多个团队应用 (团队、聊天或用户) 使用相同的 Azure AD 应用程序，则可能会出现错误。 请确保您使用的是唯一的 Azure AD 应用。

#### <a name="activities-section-changes"></a>"活动" 部分更改

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

|参数|类型|说明|
|:---|:---|:---|
|类型|string|活动的类型。 这在特定清单中需要是唯一的。|
|说明|string|可读的简短说明。 这将显示在 Microsoft 团队客户端上。|
|templateText|string|活动通知的模板文本。 您可以通过在中封装参数来声明参数 `{}` 。|

>**注意：** `actor` 是一个特殊参数，始终采用调用方的名称。 在委托呼叫中， `actor` 是用户的名称。 在仅限应用程序的调用中，它采用团队应用程序的名称。

### <a name="installing-the-teams-app"></a>安装团队应用程序

团队应用可以安装在团队、聊天或用户个人中，并且可以通过多种方式分发。 有关详细信息，请参阅 [团队应用程序分发方法](/microsoftteams/platform/concepts/deploy-and-publish/overview)。 通常情况下，推荐的是用于开发目的的 [旁加载](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) 。 开发完成后，可以根据您是要分发到一个租户还是所有租户选择适当的分发方法。

您还可以使用 [团队应用安装](/graph/api/resources/teamsappinstallation?preserve-view=true) api 来管理团队应用程序安装。

## <a name="sending-activity-feed-notifications-to-users"></a>向用户发送活动源通知

由于可以为用户、团队中或聊天中的用户安装团队应用程序，因此也可以在以下三种上下文中发送通知：

- [在聊天中向用户发送通知](/graph/api/chat-sendactivitynotification)
- [向团队中的用户发送通知](/graph/api/team-sendactivitynotification)
- [向用户发送通知](/graph/api/userteamwork-sendactivitynotification)

有关每个方案支持的主题的详细信息，请参阅特定的 Api。 所有方案都支持自定义基于文本的主题。

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>示例1：通知用户在聊天中创建的任务

本示例演示如何为在聊天中创建的新任务发送活动源通知。 在这种情况下，团队应用必须安装在 Id 为的聊天中 `chatId` ，并且用户 `569363e2-4e49-4661-87f2-16f245c5d66a` 也必须是聊天的一部分。

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

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a>示例2：通知用户在团队中创建的任务

本示例演示如何向团队发送活动源通知。 本示例通知工作组所有者所创建的新任务需要关注。

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

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a>示例3：使用自定义主题通知用户事件

如前面的示例中所示，您可以链接到团队的不同方面或聊天。 但是，如果要链接到不属于团队的方位或者不是由 Microsoft Graph 表示的方位，或者如果您想要自定义该名称，则可以为其设置 "to" 的来源 `topic` `text` 并为其传入自定义值。 此外， `webUrl` 当您使用源作为时，也是必需的 `topic` `text` 。

以下所示的 Yammer 通知示例使用自定义主题，因为 Microsoft Graph 不支持 Yammer 的资源。

> **注意：** `webUrl` 必须从 Microsoft 团队域 (teams.microsoft.com （例如) ）开始。

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

## <a name="customizing-how-the-notifications-alert-you"></a>自定义通知通知方式

Microsoft 团队用户可以自定义他们在其订阅源中看到的通知，作为横幅，等等。 通过活动源 Api 生成的通知也可以自定义。 用户可以通过 Microsoft 团队中的设置来选择如何通知他们。 团队应用程序将显示在列表中供用户选择，如下面的屏幕截图中所示。

![团队中通知设置的屏幕截图，其中突出显示了 "自定义" 选项](images/teams-activityfeednotifications/notificationsettings.png)

用户可以单击应用程序旁边的 " **编辑** "，然后自定义通知，如下面的示例所示。 将 `description` 显示 "团队" 应用程序清单中的字段。

![显示针对团队应用程序的横幅和订阅源自定义通知的屏幕截图](images/teams-activityfeednotifications/applevelnotificationsettings.png)
