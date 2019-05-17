---
title: 将 Windows UWP 应用与用户通知客户端 SDK 相集成
description: 将 Windows UWP 应用与用户通知客户端 SDK 相集成。
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: e389e9c319cb2841aa0ddf1dc697134c8c7f4011
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063280"
---
# <a name="integrate-your-windows-uwp-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="6c899-103">将 Windows UWP 应用与用户通知客户端 SDK 相集成</span><span class="sxs-lookup"><span data-stu-id="6c899-103">Integrate your Windows UWP app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="6c899-104">在 Azure 门户[注册你的应用](notifications-integration-app-registration.md)并在合作伙伴开发人员中心载入你的[跨设备体验](notifications-integration-cross-device-experiences-onboarding.md)之后，下一步是将客户端应用与适用于 Windows UWP 应用的客户端 SDK 相集成。</span><span class="sxs-lookup"><span data-stu-id="6c899-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK for Windows UWP apps.</span></span>  

<span data-ttu-id="6c899-105">借助客户端 SDK，你的应用可以执行所需的注册步骤，以开始接收从应用服务器发布的面向当前登录用户的通知。</span><span class="sxs-lookup"><span data-stu-id="6c899-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="6c899-106">SDK 随后会管理客户端上的通知，包括接收新传入的通知，管理通知状态以实现全局消除等方案，以及检索完整的通知历史记录。</span><span class="sxs-lookup"><span data-stu-id="6c899-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="6c899-107">新传入的通知流</span><span class="sxs-lookup"><span data-stu-id="6c899-107">New incoming notification flow</span></span>

<span data-ttu-id="6c899-108">对于接收新传入的通知，数据流如下图所示。</span><span class="sxs-lookup"><span data-stu-id="6c899-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Windows 应用的新通知流](images/notifications-new-notification-windows.png)

<span data-ttu-id="6c899-110">该过程涉及几个组件：</span><span class="sxs-lookup"><span data-stu-id="6c899-110">The process involves a few components:</span></span>

* <span data-ttu-id="6c899-111">应用服务器 - 应用程序的后端</span><span class="sxs-lookup"><span data-stu-id="6c899-111">App server - The back end of your application</span></span>
* <span data-ttu-id="6c899-112">应用客户端 - 应用程序的前端（UWP 应用、Android 应用或 iOS 应用）</span><span class="sxs-lookup"><span data-stu-id="6c899-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="6c899-113">Microsoft Graph 通知 - 一种服务组件，支持在跨设备和平台的各种应用客户端实例中发布、存储和同步用户通知</span><span class="sxs-lookup"><span data-stu-id="6c899-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="6c899-114">WNS - Microsoft Graph 通知用于向客户端发送信号的 Windows 推送通知服务</span><span class="sxs-lookup"><span data-stu-id="6c899-114">WNS - The Windows push notification service that Microsoft Graph notifications uses to signal the clients</span></span>

<span data-ttu-id="6c899-115">该图显示了以下步骤：</span><span class="sxs-lookup"><span data-stu-id="6c899-115">The accompanying diagram shows the following scenario:</span></span> 

1. <span data-ttu-id="6c899-116">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="6c899-116">Application logic.</span></span> <span data-ttu-id="6c899-117">此步骤可捕获用于触发向用户发布通知的事件。</span><span class="sxs-lookup"><span data-stu-id="6c899-117">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="6c899-118">这是特定于应用的逻辑，它可以是 Microsoft Graph 中的事件或其他内容的数据更新（例如新的日历事件或任务分配），也可以是应用服务希望向用户通知的其他内容。</span><span class="sxs-lookup"><span data-stu-id="6c899-118">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="6c899-119">应用服务器通过 Microsoft Graph 通知 API 向目标用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="6c899-119">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="6c899-120">有关详细信息，请参阅[服务器端集成](notifications-integrating-app-server.md)。</span><span class="sxs-lookup"><span data-stu-id="6c899-120">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="6c899-121">在收到包含新通知的 Web 请求后，Microsoft Graph 通知会在此应用和此用户的云中安全地保留通知内容。</span><span class="sxs-lookup"><span data-stu-id="6c899-121">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="6c899-122">对于订阅接收此用户通知的每个应用客户端实例，Microsoft Graph 通知会通过操作系统提供的本机推送服务发送信号以通知应用客户端。</span><span class="sxs-lookup"><span data-stu-id="6c899-122">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="6c899-123">在这种情况下，应用程序是 Windows 上的 UWP 应用，它使用“[WNS 推送原始通知](https://docs.microsoft.com/zh-CN/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview)”来发送信号。</span><span class="sxs-lookup"><span data-stu-id="6c899-123">In this case, the application is a UWP app on Windows, and it uses [WNS push raw notification](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) to send the signal.</span></span> 
5. <span data-ttu-id="6c899-124">由传入的推送通知向应用程序发出信号后，它会要求 SDK 获取用户通知存储区中的更改。</span><span class="sxs-lookup"><span data-stu-id="6c899-124">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="6c899-125">SDK 将与 Microsoft Graph 中的用户通知存储区建立安全且合规的连接。</span><span class="sxs-lookup"><span data-stu-id="6c899-125">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="6c899-126">SDK 将获取数据更改 - 在本例中为新通知内容。</span><span class="sxs-lookup"><span data-stu-id="6c899-126">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="6c899-127">SDK 会触发事件回调，以在成功检索到更改后通知该应用。</span><span class="sxs-lookup"><span data-stu-id="6c899-127">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="6c899-128">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="6c899-128">Application logic.</span></span> <span data-ttu-id="6c899-129">此步骤可捕获你的应用选择在事件回调内执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6c899-129">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="6c899-130">通常，这会导致本地应用数据更改和本地 UI 更新。</span><span class="sxs-lookup"><span data-stu-id="6c899-130">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="6c899-131">在这种情况下，该应用通常会构建定制通知弹出窗口，以通知用户有关通知内容的信息。</span><span class="sxs-lookup"><span data-stu-id="6c899-131">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="6c899-132">更新通知流</span><span class="sxs-lookup"><span data-stu-id="6c899-132">Notification update flow</span></span>

<span data-ttu-id="6c899-133">使用 Microsoft Graph 通知的主要好处之一是它可以安全地在云中保留通知，并将其转换为有状态资源类型。</span><span class="sxs-lookup"><span data-stu-id="6c899-133">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="6c899-134">因此，它可以帮助你的应用在跨设备方案中为同一登录用户跨不同设备管理和同步通知的正确状态。</span><span class="sxs-lookup"><span data-stu-id="6c899-134">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="6c899-135">当某台设备上的通知已标记为“已消除”或“已读”时，可以实时通知其他设备。</span><span class="sxs-lookup"><span data-stu-id="6c899-135">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="6c899-136">作为用户通知体验的一部分，可以真正实现“处理一次，每处均消除”的效果。</span><span class="sxs-lookup"><span data-stu-id="6c899-136">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="6c899-137">下图显示了在一台设备上更改通知状态或删除通知，以及在另一台设备上接收/处理状态更改或删除的数据流。</span><span class="sxs-lookup"><span data-stu-id="6c899-137">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Windows 应用的更新通知流](images/notifications-notification-update-windows.png)

<span data-ttu-id="6c899-139">请注意，流的第二部分与用于处理新传入通知的流相似。</span><span class="sxs-lookup"><span data-stu-id="6c899-139">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="6c899-140">这是设计使然 - 设计的 SDK 编程模式使应用程序客户端可以相似的方式处理所有类型的用户通知数据更改（新传入的通知、通知状态更改、已删除的通知）。</span><span class="sxs-lookup"><span data-stu-id="6c899-140">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="6c899-141">该图显示了以下步骤：</span><span class="sxs-lookup"><span data-stu-id="6c899-141">The accompanying diagram shows the following scenario:</span></span>

1. <span data-ttu-id="6c899-142">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="6c899-142">Application logic.</span></span> <span data-ttu-id="6c899-143">某事件触发了要更改或删除的通知。</span><span class="sxs-lookup"><span data-stu-id="6c899-143">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="6c899-144">一般来说，任何事件均可触发更改通知。</span><span class="sxs-lookup"><span data-stu-id="6c899-144">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="6c899-145">调用客户端 SDK 以更新或删除通知的应用。</span><span class="sxs-lookup"><span data-stu-id="6c899-145">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="6c899-146">目前，我们公布了两种与状态更改相关的属性 - **userActionState** 和 **readState**，但是，应用程序可以定义这些状态以及何时需要更新它们。</span><span class="sxs-lookup"><span data-stu-id="6c899-146">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="6c899-147">例如，当用户消除通知弹出窗口时，你可以将 **userActionState** 更新为“已消除”。</span><span class="sxs-lookup"><span data-stu-id="6c899-147">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="6c899-148">当用户单击通知弹出窗口并启动应用以使用相应的应用内容时，你可以将 **userActionState** 更新为“已激活”和并将 **readState** 更新为“已读”。</span><span class="sxs-lookup"><span data-stu-id="6c899-148">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="6c899-149">调用相应的 API 以更新或删除通知后，SDK 将调用云中的用户通知存储区，以将此更改扇出至同一登录用户的其他应用客户端实例。</span><span class="sxs-lookup"><span data-stu-id="6c899-149">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="6c899-150">从客户端接收更新/删除请求时，Microsoft Graph 通知将更新通知存储区，并标识已订阅此更改的其他应用客户端实例。</span><span class="sxs-lookup"><span data-stu-id="6c899-150">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="6c899-151">对于每个应用客户端订阅，Microsoft Graph 通知会通过操作系统提供的本机推送服务发送信号以通知应用客户端。</span><span class="sxs-lookup"><span data-stu-id="6c899-151">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="6c899-152">在这种情况下，它是 Windows 上的 UWP 应用，它使用“[WNS 推送原始通知](https://docs.microsoft.com/zh-CN/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview)”来发送信号。</span><span class="sxs-lookup"><span data-stu-id="6c899-152">In this case, this is a UWP app on Windows, and it uses [WNS push raw notification](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) to send the signal.</span></span> 
6. <span data-ttu-id="6c899-153">由传入的推送通知向应用程序发出信号后，它会要求 SDK 获取用户通知存储区中的更改。</span><span class="sxs-lookup"><span data-stu-id="6c899-153">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="6c899-154">SDK 将与 Microsoft Graph 中的用户通知存储区建立安全且合规的连接。</span><span class="sxs-lookup"><span data-stu-id="6c899-154">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="6c899-155">SDK 获取数据更改 - 在这种情况下，更改为通知状态更新或通知删除。</span><span class="sxs-lookup"><span data-stu-id="6c899-155">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="6c899-156">SDK 会触发事件回调，以在成功检索到更改后通知该应用。</span><span class="sxs-lookup"><span data-stu-id="6c899-156">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="6c899-157">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="6c899-157">Application logic.</span></span> <span data-ttu-id="6c899-158">此步骤可捕获你的应用选择在事件回调内执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6c899-158">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="6c899-159">通常，这会导致本地应用数据更改和本地 UI 更新。</span><span class="sxs-lookup"><span data-stu-id="6c899-159">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="6c899-160">在这种情况下，由于存在通知更新，因此应用应本地更新 UI 以反映状态更改。</span><span class="sxs-lookup"><span data-stu-id="6c899-160">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="6c899-161">例如，如果通知已标记为“已激活”，则你可以删除 Windows 操作中心内的相应定制通知弹出窗口，以实现“处理一次，每处均消除”的效果。</span><span class="sxs-lookup"><span data-stu-id="6c899-161">For example, if a notification is marked as activated, you can remove the corresponding toast notification popup inside Windows action center to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="6c899-162">有关 Microsoft Graph 通知的详细信息，请参阅  [Microsoft Graph 通知概述](notifications-concept-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="6c899-162">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="6c899-163">与 Microsoft Graph 通知进行端到端集成所需步骤相关的详细信息，请参阅 Microsoft Graph 通知[集成概述](notifications-integration-e2e-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="6c899-163">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="6c899-164">向项目添加 SDK</span><span class="sxs-lookup"><span data-stu-id="6c899-164">Adding the references needed to your project</span></span>

<span data-ttu-id="6c899-165">在 Windows 上，客户端 SDK 是一个在 Windows 操作系统之外发布的 NuGet 程序包。</span><span class="sxs-lookup"><span data-stu-id="6c899-165">On Windows, the client-side SDK is a NuGet package that ships outside of the Windows operating system.</span></span> <span data-ttu-id="6c899-166">此 API 采用 C#、C++ 和 WinJS 语言。</span><span class="sxs-lookup"><span data-stu-id="6c899-166">This API is available in C#, C++, and WinJS.</span></span> 

<span data-ttu-id="6c899-167">从 [nuget](https://www.nuget.org/packages/Microsoft.ConnectedDevices.UserNotifications) 下载适用于 Windows 应用的 Microsoft Graph 通知 SDK 的 NuGet 程序包，或按照以下步骤从 Visual Studio 中的应用解决方案下载它：</span><span class="sxs-lookup"><span data-stu-id="6c899-167">Download the NuGet package for the Microsoft Graph notifications SDK for Windows apps on [nuget](https://www.nuget.org/packages/Microsoft.ConnectedDevices.UserNotifications), or use the following steps to download it from your app solution in Visual Studio:</span></span> 

<span data-ttu-id="6c899-168">在 Visual Studio 中，右键单击项目以显示上下文菜单，然后单击“**管理 NuGet 程序包…**”。</span><span class="sxs-lookup"><span data-stu-id="6c899-168">In Visual Studio, right-click the project to bring up the context menu, and then click **Manage NuGet Packages…**.</span></span>

![管理 Nuget 程序包](images/notifications-nuget-1-manage.png)

<span data-ttu-id="6c899-170">转到“**浏览**”选项卡，并搜索 Microsoft.ConnectedDevices.UserNotifications。</span><span class="sxs-lookup"><span data-stu-id="6c899-170">Go to the **Browse** tab, and search for Microsoft.ConnectedDevices.UserNotifications.</span></span>

![查找 Nuget 程序包](images/notifications-nuget-2-find.png)

<span data-ttu-id="6c899-172">你将在搜索结果中看到 Microsoft Graph 通知客户端 SDK。</span><span class="sxs-lookup"><span data-stu-id="6c899-172">You will see the Microsoft Graph notifications client-side SDK in the search results.</span></span> <span data-ttu-id="6c899-173">单击“**安装**”按钮以安装它。</span><span class="sxs-lookup"><span data-stu-id="6c899-173">Click the **Install** button to install it.</span></span> 

![安装 NuGet 程序包](images/notifications-nuget-3-install.png)

<span data-ttu-id="6c899-175">安装完成后，程序包将显示在解决方案资源管理器中的“**引用**”下。</span><span class="sxs-lookup"><span data-stu-id="6c899-175">After the installation finishes, the package shows up under **References** in the Solution Explorer.</span></span> 

<span data-ttu-id="6c899-176">有关在 UWP 应用中包含和使用 NuGet 程序包的更多详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="6c899-176">For more details about including and consuming NuGet packages from your UWP app, see:</span></span>

* <span data-ttu-id="6c899-177">
  [使用来自 nuget.org 的程序包](https://docs.microsoft.com/zh-CN/azure/devops/artifacts/nuget/upstream-sources?view=vsts&tabs=new-nav)</span><span class="sxs-lookup"><span data-stu-id="6c899-177">[Use packages from nuget.org](https://docs.microsoft.com/en-us/azure/devops/artifacts/nuget/upstream-sources?view=vsts&tabs=new-nav)</span></span>
* <span data-ttu-id="6c899-178">
  [快速入门：在 Visual Studio 中安装和使用程序包](https://docs.microsoft.com/zh-CN/nuget/quickstart/install-and-use-a-package-in-visual-studio)</span><span class="sxs-lookup"><span data-stu-id="6c899-178">[Quickstart: Install and use a package in Visual Studio](https://docs.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-in-visual-studio)</span></span>


## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="6c899-179">初始化连接设备平台</span><span class="sxs-lookup"><span data-stu-id="6c899-179">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="6c899-180">客户端 SDK 构建在称为“连接设备平台”的基础结构之上。</span><span class="sxs-lookup"><span data-stu-id="6c899-180">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="6c899-181">在使用任何功能之前，必须在你的应用中初始化该平台。</span><span class="sxs-lookup"><span data-stu-id="6c899-181">Before you can use any features, the platform must be initialized within your app.</span></span> <span data-ttu-id="6c899-182">应该通过主类 **OnLaunched** 或 **onActivated** 方法执行初始化步骤，因为在通知方案发生之前必须执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="6c899-182">The initialization steps should occur in your main class **OnLaunched** or **onActivated** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="6c899-183">你必须通过实例化 **ConnectedDevicesPlatform** 类来构建并初始化该平台。</span><span class="sxs-lookup"><span data-stu-id="6c899-183">You must construct and initialize the platform by instantiating the **ConnectedDevicesPlatform** class.</span></span> <span data-ttu-id="6c899-184">在执行此操作之前，请确保挂接事件处理程序，如图所示，因为在启动平台后，事件可能会开始触发。</span><span class="sxs-lookup"><span data-stu-id="6c899-184">Before doing that, make sure to hook up event handlers, as shown, because after platform is started, the events might begin to fire.</span></span> 


```C#
var platform = new ConnectedDevicesPlatform();
platform.AccountManager.AccessTokenRequested += AccountManager_AccessTokenRequestedAsync;
platform.AccountManager.AccessTokenInvalidated += AccountManager_AccessTokenInvalidated;
platform.NotificationRegistrationManager.NotificationRegistrationStateChanged += NotificationRegistrationManager_NotificationRegistrationStateChanged;
platform.Start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="6c899-185">处理帐户访问令牌</span><span class="sxs-lookup"><span data-stu-id="6c899-185">Handling account access token</span></span>

<span data-ttu-id="6c899-186">SDK 发起的所有 Web 调用（包括检索新传入通知的内容、更新通知状态等）都会读取或写入用户的数据，因此始终需要有效的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6c899-186">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="6c899-187">SDK 要求你处理以下事件 - 在请求访问令牌或访问令牌失效时调用 - 以确保在初始化平台后正确处理用户的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6c899-187">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accountmanageraccesstokenrequestedasync"></a><span data-ttu-id="6c899-188">AccountManager_AccessTokenRequestedAsync</span><span class="sxs-lookup"><span data-stu-id="6c899-188">AccountManager_AccessTokenRequestedAsync</span></span>

<span data-ttu-id="6c899-189">有关完整实施，请参阅 [Windows 应用示例](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs)。</span><span class="sxs-lookup"><span data-stu-id="6c899-189">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private async void AccountManager_AccessTokenRequestedAsync(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args)
{
    private List<Account> accounts = new List<Account>();
    var account = accounts.Find((x) => x.EqualsTo(args.Request.Account));
    if (account != null)
    {
        try
        {
            var accessToken = await account.GetAccessTokenAsync(args.Request.Scopes);
            args.Request.CompleteWithAccessToken(accessToken);
        }
        catch (Exception ex)
        {
            args.Request.CompleteWithErrorMessage(ex.Message);
        }
    }
}
```

#### <a name="accountmanageraccesstokeninvalidated"></a><span data-ttu-id="6c899-190">AccountManager_AccessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="6c899-190">AccountManager_AccessTokenInvalidated</span></span>

<span data-ttu-id="6c899-191">有关完整实施，请参阅 [Windows 应用示例](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs)。</span><span class="sxs-lookup"><span data-stu-id="6c899-191">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private void AccountManager_AccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args)
{
    Logger.Instance.LogMessage($"Token Invalidated. AccountId: {args.Account.Id}, AccountType: {args.Account.Id}, scopes: {string.Join(" ", args.Scopes)}");
}
```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="6c899-192">处理推送注册过期</span><span class="sxs-lookup"><span data-stu-id="6c899-192">Handling push registration expiration</span></span> 

<span data-ttu-id="6c899-193">Microsoft Graph 通知使用 WNS（Windows 上的本机推送平台）向客户端应用程序发送有关用户通知数据更改的信号。</span><span class="sxs-lookup"><span data-stu-id="6c899-193">Microsoft Graph notifications uses WNS, the native push platform on Windows, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="6c899-194">当从应用服务器发布新传入的通知时，或者在跨设备方案中的具有同一登录用户的其他设备上更新任何通知状态时，会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="6c899-194">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="6c899-195">因此，需要一个允许原始推送通知成功通过的有效 WNS 通道。</span><span class="sxs-lookup"><span data-stu-id="6c899-195">For this reason, a valid WNS channel that allows raw push notifications to come through successfully is required.</span></span> <span data-ttu-id="6c899-196">以下事件回调负责处理 WNS 推送通道过期。</span><span class="sxs-lookup"><span data-stu-id="6c899-196">The following event callback handles WNS push channel expirations.</span></span> 

#### <a name="notificationregistrationmanagernotificationregistrationstatechanged"></a><span data-ttu-id="6c899-197">NotificationRegistrationManager_NotificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="6c899-197">NotificationRegistrationManager_NotificationRegistrationStateChanged</span></span>

<span data-ttu-id="6c899-198">有关完整实施，请参阅 [Windows 应用示例](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs)。</span><span class="sxs-lookup"><span data-stu-id="6c899-198">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private async void NotificationRegistrationManager_NotificationRegistrationStateChanged(ConnectedDevicesNotificationRegistrationManager sender, ConnectedDevicesNotificationRegistrationStateChangedEventArgs args)
{
    if ((args.State == ConnectedDevicesNotificationRegistrationState.Expired) || (args.State == ConnectedDevicesNotificationRegistrationState.Expiring))
    {
        var account = m_accounts.Find((x) => x.EqualsTo(args.Account));
        if (account != null)
        {
            await account.RegisterAccountWithSdkAsync();
        }
    }
}
```

## <a name="signing-in-your-user"></a><span data-ttu-id="6c899-199">登录用户</span><span class="sxs-lookup"><span data-stu-id="6c899-199">Signing in your user</span></span>

<span data-ttu-id="6c899-200">与 Microsoft Graph 中的许多其他资源类型一样，Microsoft Graph 通知也以用户为中心。</span><span class="sxs-lookup"><span data-stu-id="6c899-200">Microsoft Graph notifications, like many other resource types inside Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="6c899-201">为了让你的应用订阅并开始接收已登录用户的通知，你首先需要获取在注册过程中使用的有效 OAuth 令牌。</span><span class="sxs-lookup"><span data-stu-id="6c899-201">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="6c899-202">你可以使用生成和管理 OAuth 令牌的首选方法。</span><span class="sxs-lookup"><span data-stu-id="6c899-202">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="6c899-203">示例应用使用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="6c899-203">The sample app uses ADAL.</span></span> 

<span data-ttu-id="6c899-204">如果你使用的是 Microsoft 帐户，则需要在登录请求中包含以下权限：`wl.offline_access"`、`ccs.ReadWrite`、`wns.connect`、`asimovrome.telemetry` 和 `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`。</span><span class="sxs-lookup"><span data-stu-id="6c899-204">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="6c899-205">如果你使用的是 Azure AD 帐户，则需要请求以下受众：`https://cdpcs.access.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="6c899-205">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>


## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="6c899-206">将用户帐户添加到平台</span><span class="sxs-lookup"><span data-stu-id="6c899-206">Adding the user account to the platform</span></span> 

<span data-ttu-id="6c899-207">你需要使用 SDK 注册已登录用户的帐户。</span><span class="sxs-lookup"><span data-stu-id="6c899-207">You need to register the signed in user account with the SDK.</span></span> <span data-ttu-id="6c899-208">这涉及添加帐户并注册推送通道以通过 WNS 接收初始推送通知。</span><span class="sxs-lookup"><span data-stu-id="6c899-208">This involves adding the account and registering a push channel to receive the initial push notifications through WNS.</span></span> 

```C#
var account = new ConnectedDevicesAccount(accountId, accountType);           
var addResult = await platform.AccountManager.AddAccountAsync(account);
if (addResult.Status != ConnectedDevicesAccountAddedStatus.Success)
{
    throw new Exception("Add account failed with " + addResult.Status + "!");
}            

var pushChannel = await PushNotificationChannelManager.CreatePushNotificationChannelForApplicationAsync();
ConnectedDevicesNotificationRegistration registration = new ConnectedDevicesNotificationRegistration();
registration.Type = ConnectedDevicesNotificationType.WNS;
registration.Token = pushChannel.Uri;
var registerResult = await platform.NotificationRegistrationManager.RegisterAsync(account, registration);
if (registerResult.Status != ConnectedDevicesNotificationRegistrationStatus.Success)
{
    throw new Exception("Register push channel failed with " + registerResult.Status + "!");
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="6c899-209">订阅以接收用户的通知</span><span class="sxs-lookup"><span data-stu-id="6c899-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="6c899-210">你需要为此已登录用户实例化应用程序的 **UserDataFeed** 对象。</span><span class="sxs-lookup"><span data-stu-id="6c899-210">You need to instantiate a **UserDataFeed** object for your application for this signed in user.</span></span> <span data-ttu-id="6c899-211">你的应用程序由你在[跨设备体验载入](notifications-integration-cross-device-experiences-onboarding.md)过程中提供的跨平台应用 ID 进行标识。</span><span class="sxs-lookup"><span data-stu-id="6c899-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md) process.</span></span>

```C#
UserDataFeed feed = UserDataFeed.GetForAccount(account, platform, "YOUR_HOST_HERE");

var scopes = new List<UserDataFeedSyncScope> { UserNotificationChannel.SyncScope };
var subscribeResult = await feed.SubscribeToSyncScopesAsync(scopes);
if (!subscribeResult)
{
    throw new Exception("Subsribe failed!");
}
var channel = new UserNotificationChannel(feed);
var reader = channel.CreateReader();
reader.DataChanged += Reader_DataChanged;
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="6c899-212">接收和管理用户通知</span><span class="sxs-lookup"><span data-stu-id="6c899-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="6c899-213">本主题前面的流程图显示，处理来自应用服务器的新传入通知的编程模式与处理从另一个应用客户端实例启动的通知更新或删除的编程模式类似。</span><span class="sxs-lookup"><span data-stu-id="6c899-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="6c899-214">以下是处理这些数据更改的步骤。</span><span class="sxs-lookup"><span data-stu-id="6c899-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="6c899-215">处理传入推送通知信号</span><span class="sxs-lookup"><span data-stu-id="6c899-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="6c899-216">所有类型的用户通知数据更改均会生成一个作为推送通知传递至应用客户端的信号。</span><span class="sxs-lookup"><span data-stu-id="6c899-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="6c899-217">对于 Windows UWP 应用程序，作为 WNS 推送原始通知提供信号。</span><span class="sxs-lookup"><span data-stu-id="6c899-217">For Windows UWP apps, the signal is delivered as a WNS push raw notification.</span></span> <span data-ttu-id="6c899-218">接收原始推送信号时，应用应调用 **TryParse** 以触发 SDK 从 Microsoft Graph 通知服务中提取实际数据更改。</span><span class="sxs-lookup"><span data-stu-id="6c899-218">On receiving the raw push signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```C#
public async Task ReceiveNotificationAsync(string content)
{
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.TryParse(content);
    if (notification != null)
    {
        await platform.ProcessNotificationAsync(notification);
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="6c899-219">处理用户通知数据更改</span><span class="sxs-lookup"><span data-stu-id="6c899-219">Handling user notification data changes</span></span>

<span data-ttu-id="6c899-220">SDK 成功提取数据更改之后，将会调用事件回调且应用客户端有望处理通知创建、更新或删除。</span><span class="sxs-lookup"><span data-stu-id="6c899-220">After the SDK successfully fetches the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```C#
private async void Reader_DataChanged(UserNotificationReader reader, object args)
{
    var notifications = await reader.ReadBatchAsync(UInt32.MaxValue);

    foreach (var notification in notifications)
    {
        // Handle notification changes based on change type;
    }
}
```


### <a name="update-state-of-a-notification"></a><span data-ttu-id="6c899-221">更新通知状态</span><span class="sxs-lookup"><span data-stu-id="6c899-221">Update state of a notification</span></span>

<span data-ttu-id="6c899-222">如果从此应用客户端实例发起通知状态更改（例如，如果此设备上的定制通知弹出窗口由用户激活），则应用需要调用 SDK 更新通知状态，以便在同一用户使用的所有设备中同步此状态更改操作。</span><span class="sxs-lookup"><span data-stu-id="6c899-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```C#
notification.UserActionState = UserNotificationUserActionState.Activated;
await notification.SaveAsync();
```

### <a name="delete-a-notification"></a><span data-ttu-id="6c899-223">删除通知</span><span class="sxs-lookup"><span data-stu-id="6c899-223">Delete a notification</span></span>

<span data-ttu-id="6c899-224">如果从此应用客户端实例发起通知删除（例如，如果此通知对应的任务标记为“完成”并从应用数据库中删除），则应用需要调用 SDK 删除通知，以便在同一用户使用的所有设备中同步此删除操作。</span><span class="sxs-lookup"><span data-stu-id="6c899-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="6c899-225">仅当通知过期或者被显式删除时，它才会从用户通知存储区中删除。</span><span class="sxs-lookup"><span data-stu-id="6c899-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="6c899-226">将 **UserActionState** 更新为“已消除”时，用户通知不会删除，因为 **UserActionState** 的语义定义是由应用程序本身定义。</span><span class="sxs-lookup"><span data-stu-id="6c899-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```C#
await channel.DeleteUserNotificationAsync(notification.Id);
```

## <a name="see-also"></a><span data-ttu-id="6c899-227">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6c899-227">See also</span></span>

- <span data-ttu-id="6c899-228">
  [API 参考](https://docs.microsoft.com/zh-CN/windows/project-rome/notifications/api-reference-for-windows/)，以获取与 SDK 中的通知功能相关的整套 API。</span><span class="sxs-lookup"><span data-stu-id="6c899-228">[API reference](https://docs.microsoft.com/en-us/windows/project-rome/notifications/api-reference-for-windows/) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="6c899-229">适用于 Windows UWP 应用的[客户端示例](https://github.com/Microsoft/project-rome/tree/master/Windows/samples/GraphNotificationsSample)。</span><span class="sxs-lookup"><span data-stu-id="6c899-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Windows/samples/GraphNotificationsSample) for Windows UWP apps.</span></span>
- <span data-ttu-id="6c899-230">适合于发布通知的[应用服务器示例](notifications-integrating-app-server.md)。</span><span class="sxs-lookup"><span data-stu-id="6c899-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
