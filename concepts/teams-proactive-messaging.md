---
title: 使用 Microsoft 团队中的 bot 的主动消息传递
description: 通过先使用 Microsoft Graph 安装机器人，向 Microsoft 团队用户发送具有自定义应用程序的主动消息。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dafd70f1d741f15b2cfe52efe7f0a4942f06f3bd
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288936"
---
# <a name="proactive-messaging-using-a-bot-in-microsoft-teams"></a>使用 Microsoft 团队中的 bot 的主动消息传递

主动消息是在没有用户启动对话的情况下发送给 Microsoft 团队用户的一条消息。 Microsoft 团队中的自定义应用可以使用 bot 向用户发送主动消息。 但是，若要执行此操作，需要将 bot 安装为个人应用程序，也可以安装在用户所属的团队中。 在需要主动向一组用户发出邮件的情况下，如果这些用户可能已安装团队应用程序，则这一要求可能是不可行的。

本文概述了如何将 Microsoft Graph 与 Microsoft 团队应用程序相结合，以安装用户的应用程序，然后使用你的团队应用向其发送一封主动消息，而无需他们手动安装应用程序。

在高级别上，您将需要：

* [创建团队应用和 bot](#create-your-teams-app-and-bot)
* [将应用程序部署到租户应用程序目录](#deploy-your-app-to-your-tenant-app-catalog)
* [为您的用户安装应用程序](#install-the-app-for-your-users)

## <a name="create-your-teams-app-and-bot"></a>创建团队应用和 bot

如果您尚不具有可发送邮件的 bot 的 Microsoft 团队应用程序，则需要创建一个。 请参阅在团队平台文档中 [向团队应用添加 bot](/microsoftteams/platform/concepts/bots/bots-overview) 。 有关创建用于主动消息的 bot 的详细信息，请参阅 [主动型消息 for bot](/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive)。

您还可以使用 [公司 Communicator 应用模板](https://github.com/OfficeDev/microsoft-teams-company-communicator-app) 作为您的应用程序的一个很棒的入门点。 此应用模板是一个生产就绪的 Microsoft 团队应用，可以创建、安排和分发公司范围的邮件。

创建您的应用程序时，请确保记下在 `id` 应用程序清单中使用的，在后续步骤中，你将需要安装应用程序。

如果你对大型组织执行此操作，则来自你的 bot 的欢迎邮件可能会受到限制。 如果可能，请成批执行安装，并在你的 bot 中实施后端功能。 有关详细信息，请参阅 [处理速率限制](/microsoftteams/platform/concepts/bots/rate-limit)。

## <a name="deploy-your-app-to-your-tenant-app-catalog"></a>将应用程序部署到租户应用程序目录

Microsoft Graph 只能安装已添加到租户应用程序目录中的应用程序，也可以在公共 Microsoft 团队应用商店中使用。 如果你正在使用新的应用程序，你需要确保它是 [租户应用程序目录](/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog)。

## <a name="install-the-app-for-your-users"></a>为您的用户安装应用程序

若要为您的用户安装团队应用程序，首先需要确保 Microsoft Graph 应用程序具有正确的权限–你将需要用户的 ReadWrite. All 或所有的 ReadWrite。安装团队应用程序。 你还需要聊天。请参阅。所有后续步骤。 这两项权限都需要管理员同意，而您需要使用应用程序权限而不是用户委派，因为您将向用户以外的用户安装应用程序。

### <a name="check-to-see-if-the-app-is-already-installed"></a>检查是否已安装应用程序

首先，您需要查看您的团队应用是否已为您要安装它的用户安装，如示例中所示。

```http
GET /users/{user-id}/teamwork/installedApps?$expand=teamsAppDefinition&$filter=teamsAppDefinition/teamsAppId eq '{teamsAppid}'
```

其中， `{teamsAppId}` 是 `id` 您之前所做的团队应用程序清单中的。 请注意，这可能与您在 `appid` Microsoft Graph 呼叫和中的不同 `botId` 。 您可能会发现为用户手动安装应用程序并测试该用户的呼叫，以确保获得正确的值，这非常有用 `id` 。

如果未安装应用程序，则该调用将返回一个空数组; 或者，如果已安装了一个 [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) ，则返回一个数组。

### <a name="install-the-app"></a>安装应用程序

如果尚未为该用户安装该应用程序，则可以按照以下示例所示安装它。

```http
POST /users/{user-id}/teamwork/installedApps
{
   "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppid}"
}
```

有关详细信息，请参阅为 [用户安装应用程序](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)。

如果用户运行的是 Microsoft 团队，他们可能会立即或看不到应用程序安装，可能需要重新启动应用才能看到安装。

## <a name="get-the-chat-thread-id"></a>获取聊天线索 ID

为用户安装应用程序时，bot 将获取一个 `conversationUpdate` 事件，该事件将包含用于发送主动消息的必要信息。 有关详细信息，请参阅 [Bot 事件](/microsoftteams/platform/concepts/bots/bots-notifications)。

如果您丢失了 `chatThreadId` ，可以通过调用以下命令再次找到它：

```http
GET /users/{user-id}/chats?$filter=installedApps/any(a:a/teamsApp/id eq '{teamsAppid}')
```

结果的 **id** 属性是 chatThread id。

## <a name="sending-the-message"></a>发送邮件

现在，你的 bot 具有必要的信息，你可以 [发送一封主动消息](/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive)。

## <a name="c-sample"></a>C # 示例

请参阅 https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg (注释分支) 。
GraphService.cs 中有有趣的代码 `InstallAppToAllUsers()` 。 [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs)