---
title: 使用 Microsoft 团队中的 bot 的主动消息传递
description: 通过先使用 Microsoft Graph 安装机器人，向 Microsoft 团队用户发送具有自定义应用程序的主动消息。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 76b7527a961cc3aa5e78b30ff740cbda90d1c63c
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435052"
---
# <a name="proactive-messaging-using-a-bot-in-microsoft-teams"></a><span data-ttu-id="715ae-103">使用 Microsoft 团队中的 bot 的主动消息传递</span><span class="sxs-lookup"><span data-stu-id="715ae-103">Proactive messaging using a bot in Microsoft Teams</span></span>

<span data-ttu-id="715ae-104">主动消息是在没有用户启动对话的情况下发送给 Microsoft 团队用户的一条消息。</span><span class="sxs-lookup"><span data-stu-id="715ae-104">A proactive message is a message sent to a Microsoft Teams user without a user initiating the conversation.</span></span> <span data-ttu-id="715ae-105">Microsoft 团队中的自定义应用可以使用 bot 向用户发送主动消息。</span><span class="sxs-lookup"><span data-stu-id="715ae-105">Custom apps in Microsoft Teams can send proactive messages to users using a bot.</span></span> <span data-ttu-id="715ae-106">但是，若要执行此操作，需要将 bot 安装为个人应用程序，也可以安装在用户所属的团队中。</span><span class="sxs-lookup"><span data-stu-id="715ae-106">However, to do so, the bot needs to be installed either as a personal app, or in a team that the user is a member of.</span></span> <span data-ttu-id="715ae-107">在需要主动向一组用户发出邮件的情况下，如果这些用户可能已安装团队应用程序，则这一要求可能是不可行的。</span><span class="sxs-lookup"><span data-stu-id="715ae-107">This requirement can be prohibitive in scenarios where you need to proactively message a group of users that might or might not have the Teams app installed.</span></span>

<span data-ttu-id="715ae-108">本文概述了如何将 Microsoft Graph 与 Microsoft 团队应用程序相结合，以安装用户的应用程序，然后使用你的团队应用向其发送一封主动消息，而无需他们手动安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="715ae-108">This article outlines how you can combine Microsoft Graph with a Microsoft Teams app to install the app for your users and then use your Teams app to send them a proactive message, without requiring them to manually install the app.</span></span>

<span data-ttu-id="715ae-109">在高级别上，您将需要：</span><span class="sxs-lookup"><span data-stu-id="715ae-109">At a high level, you'll need to:</span></span>

* [<span data-ttu-id="715ae-110">创建团队应用和 bot</span><span class="sxs-lookup"><span data-stu-id="715ae-110">Create your Teams app and bot</span></span>](#create-your-teams-app-and-bot)
* [<span data-ttu-id="715ae-111">将应用程序部署到租户应用程序目录</span><span class="sxs-lookup"><span data-stu-id="715ae-111">Deploy your app to your tenant app catalog</span></span>](#deploy-your-app-to-your-tenant-app-catalog)
* [<span data-ttu-id="715ae-112">为您的用户安装应用程序</span><span class="sxs-lookup"><span data-stu-id="715ae-112">Install the app for your users</span></span>](#install-the-app-for-your-users)

## <a name="create-your-teams-app-and-bot"></a><span data-ttu-id="715ae-113">创建团队应用和 bot</span><span class="sxs-lookup"><span data-stu-id="715ae-113">Create your Teams app and bot</span></span>

<span data-ttu-id="715ae-114">如果您尚不具有可发送邮件的 bot 的 Microsoft 团队应用程序，则需要创建一个。</span><span class="sxs-lookup"><span data-stu-id="715ae-114">If you do not already have a Microsoft Teams app with a bot that can send the message, you'll need to create one.</span></span> <span data-ttu-id="715ae-115">请参阅在团队平台文档中[向团队应用添加 bot](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-overview) 。</span><span class="sxs-lookup"><span data-stu-id="715ae-115">See [Add bots to Teams apps](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-overview) in the Teams platform documentation.</span></span> <span data-ttu-id="715ae-116">有关创建用于主动消息的 bot 的详细信息，请参阅[主动型消息 for bot](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive)。</span><span class="sxs-lookup"><span data-stu-id="715ae-116">For specifics about creating a bot for proactive messaging, see [Proactive messaging for bots](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).</span></span>

<span data-ttu-id="715ae-117">您还可以使用[公司 Communicator 应用模板](https://github.com/OfficeDev/microsoft-teams-company-communicator-app)作为您的应用程序的一个很棒的入门点。</span><span class="sxs-lookup"><span data-stu-id="715ae-117">You can also use the [Company Communicator app template](https://github.com/OfficeDev/microsoft-teams-company-communicator-app) as a good starting point for your app.</span></span> <span data-ttu-id="715ae-118">此应用模板是一个生产就绪的 Microsoft 团队应用，可以创建、安排和分发公司范围的邮件。</span><span class="sxs-lookup"><span data-stu-id="715ae-118">This app template is a production-ready Microsoft Teams app capable of creating, scheduling, and distributing company-wide messages.</span></span>

<span data-ttu-id="715ae-119">创建您的应用程序时，请确保记下在 `id` 应用程序清单中使用的，在后续步骤中，你将需要安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="715ae-119">When creating your app, make sure that you take note of the `id` you use in your application manifest; you'll need it to install the app in a subsequent step.</span></span>

<span data-ttu-id="715ae-120">如果你对大型组织执行此操作，则来自你的 bot 的欢迎邮件可能会受到限制。</span><span class="sxs-lookup"><span data-stu-id="715ae-120">If you're doing this for a large organization, the welcome messages from your bot might get throttled.</span></span> <span data-ttu-id="715ae-121">如果可能，请成批执行安装，并在你的 bot 中实施后端功能。</span><span class="sxs-lookup"><span data-stu-id="715ae-121">If possible, perform the installations in batches, and implement back-off functionality in your bot.</span></span> <span data-ttu-id="715ae-122">有关详细信息，请参阅[处理速率限制](/microsoftteams/platform/concepts/bots/rate-limit)。</span><span class="sxs-lookup"><span data-stu-id="715ae-122">For details, see [handling rate limiting](/microsoftteams/platform/concepts/bots/rate-limit).</span></span>

## <a name="deploy-your-app-to-your-tenant-app-catalog"></a><span data-ttu-id="715ae-123">将应用程序部署到租户应用程序目录</span><span class="sxs-lookup"><span data-stu-id="715ae-123">Deploy your app to your tenant app catalog</span></span>

<span data-ttu-id="715ae-124">Microsoft Graph 只能安装已添加到租户应用程序目录中的应用程序，也可以在公共 Microsoft 团队应用商店中使用。</span><span class="sxs-lookup"><span data-stu-id="715ae-124">Microsoft Graph can only install apps that have been added to your tenant app catalog, or are available in the public Microsoft Teams app store.</span></span> <span data-ttu-id="715ae-125">如果你正在使用新的应用程序，你需要确保它是[租户应用程序目录](https://docs.microsoft.com/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog)。</span><span class="sxs-lookup"><span data-stu-id="715ae-125">If you're working with a new app, you'll need to make sure it is [tenant app catalog](https://docs.microsoft.com/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog).</span></span>

## <a name="install-the-app-for-your-users"></a><span data-ttu-id="715ae-126">为您的用户安装应用程序</span><span class="sxs-lookup"><span data-stu-id="715ae-126">Install the app for your users</span></span>

<span data-ttu-id="715ae-127">若要为您的用户安装团队应用程序，首先需要确保 Microsoft Graph 应用程序具有正确的权限–你将需要用户的 ReadWrite. All 或所有的 ReadWrite。安装团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="715ae-127">To install the Teams app for your users, you'll first need to ensure that your Microsoft Graph application has the right permissions – you'll need User.ReadWrite.All or Directory.ReadWrite.All to install the Teams app.</span></span> <span data-ttu-id="715ae-128">你还需要聊天。请参阅。所有后续步骤。</span><span class="sxs-lookup"><span data-stu-id="715ae-128">You'll also need Chat.Read.All for a subsequent step.</span></span> <span data-ttu-id="715ae-129">这两项权限都需要管理员同意，而您需要使用应用程序权限而不是用户委派，因为您将向用户以外的用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="715ae-129">Both permissions will require admin consent, and you'll need to use application permissions rather than user delegated because you will be installing apps to users other than yourself.</span></span>

### <a name="check-to-see-if-the-app-is-already-installed"></a><span data-ttu-id="715ae-130">检查是否已安装应用程序</span><span class="sxs-lookup"><span data-stu-id="715ae-130">Check to see if the app is already installed</span></span>

<span data-ttu-id="715ae-131">首先，您需要查看您的团队应用是否已为您要安装它的用户安装，如示例中所示。</span><span class="sxs-lookup"><span data-stu-id="715ae-131">First, you'll want to check to see if your Teams app is already installed for the users you want to install it from, as shown in the example.</span></span>

```http
GET /users/{user-id}/teamwork/installedApps?$expand=teamsAppDefinition&$filter=teamsAppDefinition/teamsAppId eq '{teamsAppid}'
```

<span data-ttu-id="715ae-132">其中， `{teamsAppId}` 是 `id` 您之前所做的团队应用程序清单中的。</span><span class="sxs-lookup"><span data-stu-id="715ae-132">Where `{teamsAppId}` is the `id` in the Teams app manifest that you made note of previously.</span></span> <span data-ttu-id="715ae-133">请注意，这可能与您在 `appid` Microsoft Graph 呼叫和中的不同 `botId` 。</span><span class="sxs-lookup"><span data-stu-id="715ae-133">Note that this might be different from your `appid` for Microsoft Graph calls, and from your `botId`.</span></span> <span data-ttu-id="715ae-134">您可能会发现为用户手动安装应用程序并测试该用户的呼叫，以确保获得正确的值，这非常有用 `id` 。</span><span class="sxs-lookup"><span data-stu-id="715ae-134">You might find it useful to manually install the app for a user and test the call against that user to ensure that you've got the correct `id` value.</span></span>

<span data-ttu-id="715ae-135">如果未安装应用程序，则该调用将返回一个空数组; 或者，如果已安装了一个[teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) ，则返回一个数组。</span><span class="sxs-lookup"><span data-stu-id="715ae-135">The call will return an empty array if the app is not installed, or an array with a single [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) if it is already installed.</span></span>

### <a name="install-the-app"></a><span data-ttu-id="715ae-136">安装应用程序</span><span class="sxs-lookup"><span data-stu-id="715ae-136">Install the app</span></span>

<span data-ttu-id="715ae-137">如果尚未为该用户安装该应用程序，则可以按照以下示例所示安装它。</span><span class="sxs-lookup"><span data-stu-id="715ae-137">If the app is not already installed for that user, you can then install it as shown in the following example.</span></span>

```http
POST /users/{user-id}/teamwork/installedApps
{
   "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppid}"
}
```

<span data-ttu-id="715ae-138">有关详细信息，请参阅为[用户安装应用程序](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="715ae-138">For more information, see [Install app for user](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta).</span></span>

<span data-ttu-id="715ae-139">如果用户运行的是 Microsoft 团队，他们可能会立即或看不到应用程序安装，可能需要重新启动应用才能看到安装。</span><span class="sxs-lookup"><span data-stu-id="715ae-139">If the user has Microsoft Teams running, they might or might not see the app installation right away – they might need to restart the app to see the installation.</span></span>

## <a name="get-the-chat-thread-id"></a><span data-ttu-id="715ae-140">获取聊天线索 ID</span><span class="sxs-lookup"><span data-stu-id="715ae-140">Get the chat thread ID</span></span>

<span data-ttu-id="715ae-141">为用户安装应用程序时，bot 将获取一个 `conversationUpdate` 事件，该事件将包含用于发送主动消息的必要信息。</span><span class="sxs-lookup"><span data-stu-id="715ae-141">When the app is installed for the user, the bot will get a `conversationUpdate` event that will contain the necessary information for it to send the proactive message.</span></span> <span data-ttu-id="715ae-142">有关详细信息，请参阅[Bot 事件](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-notifications)。</span><span class="sxs-lookup"><span data-stu-id="715ae-142">For more information, see [Bot events](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-notifications).</span></span>

<span data-ttu-id="715ae-143">如果您丢失了 `chatThreadId` ，可以通过调用以下命令再次找到它：</span><span class="sxs-lookup"><span data-stu-id="715ae-143">If you lose the `chatThreadId`, you can find it again by calling:</span></span>

```http
GET /users/{user-id}/chats?$filter=installedApps/any(a:a/teamsApp/id eq '{teamsAppid}')
```

<span data-ttu-id="715ae-144">结果的**id**属性是 chatThread id。</span><span class="sxs-lookup"><span data-stu-id="715ae-144">The **id** property of the result is the chatThread ID.</span></span>

## <a name="sending-the-message"></a><span data-ttu-id="715ae-145">发送邮件</span><span class="sxs-lookup"><span data-stu-id="715ae-145">Sending the message</span></span>

<span data-ttu-id="715ae-146">现在，你的 bot 具有必要的信息，你可以[发送一封主动消息](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive)。</span><span class="sxs-lookup"><span data-stu-id="715ae-146">Now that your bot has the necessary information, you can [send a proactive message](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).</span></span>

## <a name="c-sample"></a><span data-ttu-id="715ae-147">C # 示例</span><span class="sxs-lookup"><span data-stu-id="715ae-147">C# sample</span></span>

<span data-ttu-id="715ae-148">请参阅 https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg （注释 "分支"）。</span><span class="sxs-lookup"><span data-stu-id="715ae-148">See https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg (note the branch).</span></span>
<span data-ttu-id="715ae-149">GraphService.cs 中有有趣的代码 `InstallAppToAllUsers()` 。 [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs)</span><span class="sxs-lookup"><span data-stu-id="715ae-149">Interesting code is in `InstallAppToAllUsers()` in [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs).</span></span>
