---
title: 将 Android 应用与用户通知客户端 SDK 相集成
description: 将 Android 应用与用户通知客户端 SDK 相集成
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: a0c3050d7f9c644c23696d9a2071e7427b6b565d
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620302"
---
# <a name="integrate-your-android-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="d6824-103">将 Android 应用与用户通知客户端 SDK 相集成</span><span class="sxs-lookup"><span data-stu-id="d6824-103">Integrate your Android app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="d6824-104">在 Azure 门户[注册你的应用](notifications-integration-app-registration.md)并在合作伙伴开发人员中心载入你的[跨设备体验](notifications-integration-cross-device-experiences-onboarding.md)之后，下一步是将客户端应用与适用于 Android 应用的客户端 SDK 相集成。</span><span class="sxs-lookup"><span data-stu-id="d6824-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK forAndroid apps.</span></span>  

<span data-ttu-id="d6824-105">借助客户端 SDK，你的应用可以执行所需的注册步骤，以开始接收从应用服务器发布的面向当前登录用户的通知。</span><span class="sxs-lookup"><span data-stu-id="d6824-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="d6824-106">SDK 随后会管理客户端上的通知，包括接收新传入的通知，管理通知状态以实现全局消除等方案，以及检索完整的通知历史记录。</span><span class="sxs-lookup"><span data-stu-id="d6824-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="d6824-107">新传入的通知流</span><span class="sxs-lookup"><span data-stu-id="d6824-107">New incoming notification flow</span></span>

<span data-ttu-id="d6824-108">对于接收新传入的通知，数据流如下图所示。</span><span class="sxs-lookup"><span data-stu-id="d6824-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Android 应用的新通知流](images/notifications-new-notification-android.png)

<span data-ttu-id="d6824-110">该过程涉及几个组件：</span><span class="sxs-lookup"><span data-stu-id="d6824-110">he process involves a few components:</span></span>

* <span data-ttu-id="d6824-111">应用服务器 - 应用程序的后端</span><span class="sxs-lookup"><span data-stu-id="d6824-111">App server - The back end of your application</span></span>
* <span data-ttu-id="d6824-112">应用客户端 - 应用程序的前端（UWP 应用、Android 应用或 iOS 应用）</span><span class="sxs-lookup"><span data-stu-id="d6824-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="d6824-113">Microsoft Graph 通知 - 一种服务组件，支持在跨设备和平台的各种应用客户端实例中发布、存储和同步用户通知</span><span class="sxs-lookup"><span data-stu-id="d6824-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="d6824-114">FCM - Firebase Cloud Messaging，Android 作为 Google Play Services 一部分提供的推送通知服务。</span><span class="sxs-lookup"><span data-stu-id="d6824-114">FCM - Firebase Cloud Messaging, the push notification service provided by Android as a part of Google Play Services.</span></span> <span data-ttu-id="d6824-115">Microsoft Graph 通知使用此服务向 Android 应用客户端发送有关用户通知数据更改的信号。</span><span class="sxs-lookup"><span data-stu-id="d6824-115">Microsoft Graph notifications use this service to signal the Android app clients about user notification data changes.</span></span>  

<span data-ttu-id="d6824-116">该图显示了以下步骤：</span><span class="sxs-lookup"><span data-stu-id="d6824-116">The accompanying diagram shows the following scenario:</span></span> 

1. <span data-ttu-id="d6824-117">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="d6824-117">Application logic.</span></span> <span data-ttu-id="d6824-118">此步骤可捕获用于触发向用户发布通知的事件。</span><span class="sxs-lookup"><span data-stu-id="d6824-118">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="d6824-119">这是特定于应用的逻辑，它可以是 Microsoft Graph 中的事件或其他内容的数据更新（例如新的日历事件或任务分配），也可以是应用服务希望向用户通知的其他内容。</span><span class="sxs-lookup"><span data-stu-id="d6824-119">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="d6824-120">应用服务器通过 Microsoft Graph 通知 API 向目标用户发布通知。</span><span class="sxs-lookup"><span data-stu-id="d6824-120">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="d6824-121">有关详细信息，请参阅[服务器端集成](notifications-integrating-app-server.md)。</span><span class="sxs-lookup"><span data-stu-id="d6824-121">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="d6824-122">在收到包含新通知的 Web 请求后，Microsoft Graph 通知会在此应用和此用户的云中安全地保留通知内容。</span><span class="sxs-lookup"><span data-stu-id="d6824-122">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="d6824-123">对于订阅接收此用户通知的每个应用客户端实例，Microsoft Graph 通知会通过操作系统提供的本机推送服务发送信号以通知应用客户端。</span><span class="sxs-lookup"><span data-stu-id="d6824-123">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="d6824-124">在这种情况下，应用程序为 Android 应用程序，它使用 [FCM 数据消息](https://firebase.google.com/docs/cloud-messaging/concept-options)发送信号。</span><span class="sxs-lookup"><span data-stu-id="d6824-124">In this case, the application is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
5. <span data-ttu-id="d6824-125">由传入的推送通知向应用程序发出信号后，它会要求 SDK 获取用户通知存储中的更改。</span><span class="sxs-lookup"><span data-stu-id="d6824-125">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="d6824-126">SDK 将与 Microsoft Graph 中的用户通知存储区建立安全且合规的连接。</span><span class="sxs-lookup"><span data-stu-id="d6824-126">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="d6824-127">SDK 将获取数据更改 - 在本例中为新通知内容。</span><span class="sxs-lookup"><span data-stu-id="d6824-127">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="d6824-128">SDK 会触发事件回调，以在成功检索到更改后通知该应用。</span><span class="sxs-lookup"><span data-stu-id="d6824-128">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="d6824-129">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="d6824-129">Application logic.</span></span> <span data-ttu-id="d6824-130">此步骤可捕获你的应用选择在事件回调内执行的操作。</span><span class="sxs-lookup"><span data-stu-id="d6824-130">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="d6824-131">通常，这会导致本地应用数据更改和本地 UI 更新。</span><span class="sxs-lookup"><span data-stu-id="d6824-131">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="d6824-132">在这种情况下，该应用通常会构建定制通知弹出窗口，以通知用户有关通知内容的信息。</span><span class="sxs-lookup"><span data-stu-id="d6824-132">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="d6824-133">更新通知流</span><span class="sxs-lookup"><span data-stu-id="d6824-133">Notification update flow</span></span>

<span data-ttu-id="d6824-134">使用 Microsoft Graph 通知的主要好处之一是它可以安全地在云中保留通知，并将其转换为有状态资源类型。</span><span class="sxs-lookup"><span data-stu-id="d6824-134">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="d6824-135">因此，它可以帮助你的应用在跨设备方案中为同一登录用户跨不同设备管理和同步通知的正确状态。</span><span class="sxs-lookup"><span data-stu-id="d6824-135">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="d6824-136">当某台设备上的通知已标记为“已消除”或“已读”时，可以实时通知其他设备。</span><span class="sxs-lookup"><span data-stu-id="d6824-136">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="d6824-137">作为用户通知体验的一部分，可以真正实现“处理一次，每处均消除”的效果。</span><span class="sxs-lookup"><span data-stu-id="d6824-137">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="d6824-138">下图显示了在一台设备上更改通知状态或删除通知，以及在另一台设备上接收/处理状态更改或删除的数据流。</span><span class="sxs-lookup"><span data-stu-id="d6824-138">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Android 应用的更新通知流](images/notifications-notification-update-android.png)

<span data-ttu-id="d6824-140">请注意，流的第二部分与用于处理新传入通知的流相似。</span><span class="sxs-lookup"><span data-stu-id="d6824-140">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="d6824-141">这是设计使然 - 设计的 SDK 编程模式使应用程序客户端可以相似的方式处理所有类型的用户通知数据更改（新传入的通知、通知状态更改、已删除的通知）。</span><span class="sxs-lookup"><span data-stu-id="d6824-141">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="d6824-142">该图显示了以下步骤：</span><span class="sxs-lookup"><span data-stu-id="d6824-142">The accompanying diagram shows the following scenario:</span></span>

1. <span data-ttu-id="d6824-143">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="d6824-143">Application logic.</span></span> <span data-ttu-id="d6824-144">某事件触发了要更改或删除的通知。</span><span class="sxs-lookup"><span data-stu-id="d6824-144">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="d6824-145">一般来说，任何事件均可触发更改通知。</span><span class="sxs-lookup"><span data-stu-id="d6824-145">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="d6824-146">调用客户端 SDK 以更新或删除通知的应用。</span><span class="sxs-lookup"><span data-stu-id="d6824-146">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="d6824-147">目前，我们公布了两种与状态更改相关的属性 - **userActionState** 和 **readState**，但是，应用程序可以定义这些状态以及何时需要更新它们。</span><span class="sxs-lookup"><span data-stu-id="d6824-147">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="d6824-148">例如，当用户消除通知弹出窗口时，你可以将 **userActionState** 更新为“已消除”。</span><span class="sxs-lookup"><span data-stu-id="d6824-148">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="d6824-149">当用户单击通知弹出窗口并启动应用以使用相应的应用内容时，你可以将 **userActionState** 更新为“已激活”和并将 **readState** 更新为“已读”。</span><span class="sxs-lookup"><span data-stu-id="d6824-149">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="d6824-150">调用相应的 API 以更新或删除通知后，SDK 将调用云中的用户通知存储区，以将此更改扇出至同一登录用户的其他应用客户端实例。</span><span class="sxs-lookup"><span data-stu-id="d6824-150">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="d6824-151">从客户端接收更新/删除请求时，Microsoft Graph 通知将更新通知存储区，并标识已订阅此更改的其他应用客户端实例。</span><span class="sxs-lookup"><span data-stu-id="d6824-151">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="d6824-152">对于每个应用客户端订阅，Microsoft Graph 通知会通过操作系统提供的本机推送服务发送信号以通知应用客户端。</span><span class="sxs-lookup"><span data-stu-id="d6824-152">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="d6824-153">在这种情况下，这是 Android 应用程序，它使用 [FCM 数据消息](https://firebase.google.com/docs/cloud-messaging/concept-options)发送信号。</span><span class="sxs-lookup"><span data-stu-id="d6824-153">In this case, this is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
6. <span data-ttu-id="d6824-154">由传入的推送通知向应用程序发出信号后，它会要求 SDK 获取用户通知存储中的更改。</span><span class="sxs-lookup"><span data-stu-id="d6824-154">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="d6824-155">SDK 将与 Microsoft Graph 中的用户通知存储区建立安全且合规的连接。</span><span class="sxs-lookup"><span data-stu-id="d6824-155">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="d6824-156">SDK 获取数据更改 - 在这种情况下，更改为通知状态更新或通知删除。</span><span class="sxs-lookup"><span data-stu-id="d6824-156">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="d6824-157">SDK 会触发事件回调，以在成功检索到更改后通知该应用。</span><span class="sxs-lookup"><span data-stu-id="d6824-157">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="d6824-158">应用程序逻辑。</span><span class="sxs-lookup"><span data-stu-id="d6824-158">Application logic.</span></span> <span data-ttu-id="d6824-159">此步骤可捕获你的应用选择在事件回调内执行的操作。</span><span class="sxs-lookup"><span data-stu-id="d6824-159">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="d6824-160">通常，这会导致本地应用数据更改和本地 UI 更新。</span><span class="sxs-lookup"><span data-stu-id="d6824-160">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="d6824-161">在这种情况下，由于存在通知更新，因此应用应本地更新 UI 以反映状态更改。</span><span class="sxs-lookup"><span data-stu-id="d6824-161">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="d6824-162">例如，如果通知已标记为“已激活”，则你可以删除 Android 通知托盘中的相应通知消息，以实现“处理一次，每处均消除”的效果。</span><span class="sxs-lookup"><span data-stu-id="d6824-162">For example, if a notification is marked as activated, you can remove the corresponding notification message inside Android's notification tray to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="d6824-163">有关 Microsoft Graph 通知的详细信息，请参阅 [Microsoft Graph 通知概述](notifications-concept-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="d6824-163">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="d6824-164">与 Microsoft Graph 通知进行端到端集成所需步骤相关的详细信息，请参阅 Microsoft Graph 通知[集成概述](notifications-integration-e2e-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="d6824-164">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="development-environment-and-requirements"></a><span data-ttu-id="d6824-165">开发环境和要求</span><span class="sxs-lookup"><span data-stu-id="d6824-165">Development and authoring requirements</span></span>

<span data-ttu-id="d6824-166">若要使用 Microsoft Graph 通知，你需要使用采用受支持架构（**armeabi-v7a**、**arm64-v8a**、**x86** 或 **x86_64**）之一或枚举器的 Android 应用开发 IDE 和 Android 设备。</span><span class="sxs-lookup"><span data-stu-id="d6824-166">To use Microsoft Graph notifications, you will need an Android app development IDE and an Android device with one of the supported architectures (**armeabi-v7a**, **arm64-v8a**, **x86**, or **x86_64**) or an emulator.</span></span> <span data-ttu-id="d6824-167">系统必须运行 Android 4.4.2 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d6824-167">The system must be running Android 4.4.2 or later.</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="d6824-168">向项目添加 SDK</span><span class="sxs-lookup"><span data-stu-id="d6824-168">Adding the references needed to your project</span></span>

<span data-ttu-id="d6824-169">将以下存储库引用插入到项目根处的 *build.gradle* 文件中。</span><span class="sxs-lookup"><span data-stu-id="d6824-169">Insert the following repository references into the *build.gradle* file at the root of your project.</span></span>

```Java
allprojects {
    repositories {
    jcenter()
    maven { url 'https://maven.google.com' }
    maven { url 'https://projectrome.bintray.com/maven/' }
    }
}
```

<span data-ttu-id="d6824-170">然后，将以下依赖项插入到项目文件夹中的 _build.gradle_ 文件中。</span><span class="sxs-lookup"><span data-stu-id="d6824-170">Then, insert the following dependency into the _build.gradle_ file that is in your project folder.</span></span>

```Java
dependencies { 
    ...
    implementation 'com.microsoft.connecteddevices:connecteddevices-sdk:+'
}
```

<span data-ttu-id="d6824-171">如果想要在应用中使用 ProGuard，请为这些新 API 添加 ProGuard 规则。</span><span class="sxs-lookup"><span data-stu-id="d6824-171">If you want to use ProGuard in your app, add the ProGuard Rules for these new APIs.</span></span> <span data-ttu-id="d6824-172">在项目的 *App* 文件中创建名为 *proguard-rules.txt* 的文件，然后粘贴到 [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt) 目录中。</span><span class="sxs-lookup"><span data-stu-id="d6824-172">Create a file called *proguard-rules.txt* in the *App* folder of your project, and paste in the contents of [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt).</span></span>
<span data-ttu-id="d6824-173">在项目的 *AndroidManifest.xml* 文件中，在 `manifest` 元素内添加以下权限（如果尚不存在）。</span><span class="sxs-lookup"><span data-stu-id="d6824-173">In your project's *AndroidManifest.xml* file, add the following permissions inside the `manifest` element (if they are not already present).</span></span> <span data-ttu-id="d6824-174">这为你的应用提供了连接至 Internet 和在设备上启用蓝牙发现功能的权限。</span><span class="sxs-lookup"><span data-stu-id="d6824-174">This gives your app permission to connect to the Internet and to enable Bluetooth discovery on your device.</span></span>
<span data-ttu-id="d6824-175">请注意，只有使用蓝牙发现功能时才需要蓝牙相关权限；对于连接设备平台中的其他功能，无需此权限。</span><span class="sxs-lookup"><span data-stu-id="d6824-175">Note that the Bluetooth-related permissions are only necessary for using Bluetooth discovery; they are not needed for the other features in the Connected Devices Platform.</span></span> <span data-ttu-id="d6824-176">此外，只有 Android SDK 21 或更高版本才需要 `ACCESS_COARSE_LOCATION`。</span><span class="sxs-lookup"><span data-stu-id="d6824-176">Additionally, `ACCESS_COARSE_LOCATION` is only required on Android SDKs 21 and later.</span></span> <span data-ttu-id="d6824-177">在 Android SDK 23 及更高版本上，还必须提示用户授予运行时位置访问权限。</span><span class="sxs-lookup"><span data-stu-id="d6824-177">On Android SDKs 23 and later, you must also prompt the user to grant location access at runtime.</span></span>

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.BLUETOOTH" />
<uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```
<span data-ttu-id="d6824-178">接着，转至你希望找到连接设备功能的活动类。</span><span class="sxs-lookup"><span data-stu-id="d6824-178">Next, go to the activity classes where you would like the Connected Devices functionality to be located.</span></span> <span data-ttu-id="d6824-179">导入以下命名空间。</span><span class="sxs-lookup"><span data-stu-id="d6824-179">Add the following namespaces.</span></span>

```java
import com.microsoft.connecteddevices;
import com.microsoft.connecteddevices.userdata;
import com.microsoft.connecteddevices.userdata.usernotifications;
```

## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="d6824-180">初始化连接设备平台</span><span class="sxs-lookup"><span data-stu-id="d6824-180">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="d6824-181">客户端 SDK 构建在称为“连接设备平台”的基础结构之上。</span><span class="sxs-lookup"><span data-stu-id="d6824-181">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="d6824-182">在使用任何功能之前，必须在你的应用中初始化该平台。</span><span class="sxs-lookup"><span data-stu-id="d6824-182">Before any feature can be used, the platform must be initialized within your app.</span></span> <span data-ttu-id="d6824-183">应该通过主类 **OnCreate** 方法执行初始化步骤，因为在通知方案发生之前必须执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="d6824-183">The initialization steps should occur in your main class **OnCreate** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="d6824-184">你必须通过实例化 [**ConnectedDevicesPlatform**](https://docs.microsoft.com/en-us/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest) 类来构建并初始化该平台。</span><span class="sxs-lookup"><span data-stu-id="d6824-184">You must construct and initialize the platform by instantiating the [**ConnectedDevicesPlatform**](https://docs.microsoft.com/en-us/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest) class.</span></span> <span data-ttu-id="d6824-185">执行此操作之前，请确保连接事件处理程序，因为启动平台之后，可能会开始触发事件。</span><span class="sxs-lookup"><span data-stu-id="d6824-185">Before doing that, make sure to hook up event handlers, because after the platform is started, the events might begin to fire.</span></span> 

```java
ConnectedDevicesPlatform platform = new ConnectedDevicesPlatform(context);

platform.getAccountManager().accessTokenRequested().subscribe((accountManager, args) -> onAccessTokenRequested(accountManager, args));
platform.getAccountManager().accessTokenInvalidated().subscribe((accountManager, args) -> onAccessTokenInvalidated(accountManager, args));
platform.getNotificationRegistrationManager().notificationRegistrationStateChanged().subscribe((notificationRegistrationManager, args) -> onNotificationRegistrationStateChanged(notificationRegistrationManager, args));

platform.start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="d6824-186">处理帐户访问令牌</span><span class="sxs-lookup"><span data-stu-id="d6824-186">Handling account access token</span></span>

<span data-ttu-id="d6824-187">SDK 发起的所有 Web 调用（包括检索新传入通知的内容、更新通知状态等）都会读取或写入用户的数据，因此始终需要有效的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d6824-187">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="d6824-188">SDK 要求你处理以下事件 - 在请求访问令牌或访问令牌失效时调用 - 以确保在初始化平台后正确处理用户的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d6824-188">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accesstokenrequested"></a><span data-ttu-id="d6824-189">accessTokenRequested</span><span class="sxs-lookup"><span data-stu-id="d6824-189">accessTokenRequested</span></span> 

<span data-ttu-id="d6824-190">有关完整实施，请参阅 [Android 示例应用](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java)。</span><span class="sxs-lookup"><span data-stu-id="d6824-190">For a full implementation, see the [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenRequested(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args) {
    ConnectedDevicesAccessTokenRequest request = args.getRequest();
    List<String> scopes = request.getScopes();

    // We always need to complete the request, even if a matching account is not found
    if (account == null) {
        request.completeWithErrorMessage("The app could not find a matching ConnectedDevicesAccount to get a token");
        return;
    }

    // Complete the request with a token
    account.getAccessTokenAsync(scopes)
        .thenAcceptAsync((String token) -> {
            request.completeWithAccessToken(token);
        }).exceptionally(throwable -> {
            request.completeWithErrorMessage("The Account could not return a token with those scopes");
            return null;
    });
}
```

#### <a name="accesstokeninvalidated"></a><span data-ttu-id="d6824-191">accessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="d6824-191">accessTokenInvalidated</span></span>

<span data-ttu-id="d6824-192">有关完整实施，请参阅 [Android 示例应用](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java)。</span><span class="sxs-lookup"><span data-stu-id="d6824-192">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args, List<Account> accounts) {
    Log.i(TAG, "Token invalidated for account: " + args.getAccount().getId());
}

```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="d6824-193">处理推送注册过期</span><span class="sxs-lookup"><span data-stu-id="d6824-193">Handling push registration expiration</span></span> 

<span data-ttu-id="d6824-194">Microsoft Graph 通知使用 FCM（Android 上的本机推送平台）向客户端应用程序发送有关用户通知数据更改的信号。</span><span class="sxs-lookup"><span data-stu-id="d6824-194">Microsoft Graph notifications uses FCM, the native push platform on Android, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="d6824-195">当从应用服务器发布新传入的通知时，或者在跨设备方案中的具有同一登录用户的其他设备上更新任何通知状态时，会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="d6824-195">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="d6824-196">因此，需要一个允许数据通知消息成功通过的有效 FCM 令牌。</span><span class="sxs-lookup"><span data-stu-id="d6824-196">Therefore, a valid FCM token that allows data notification messages to come through successfully is required.</span></span> <span data-ttu-id="d6824-197">以下事件回调处理 FCM 推送令牌到期。</span><span class="sxs-lookup"><span data-stu-id="d6824-197">The following event callback handles FCM push token expirations.</span></span> 

#### <a name="notificationregistrationstatechanged"></a><span data-ttu-id="d6824-198">notificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="d6824-198">notificationRegistrationStateChanged</span></span>

<span data-ttu-id="d6824-199">有关完整实施，请参阅 [Android 示例应用](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java)。</span><span class="sxs-lookup"><span data-stu-id="d6824-199">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

## <a name="signing-in-your-user"></a><span data-ttu-id="d6824-200">登录用户</span><span class="sxs-lookup"><span data-stu-id="d6824-200">Signing in your user</span></span>

<span data-ttu-id="d6824-201">与 Microsoft Graph 中的许多其他资源类型一样，Microsoft Graph 通知也以用户为中心。</span><span class="sxs-lookup"><span data-stu-id="d6824-201">Microsoft Graph notifications, like many other resource types in Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="d6824-202">为了让你的应用订阅并开始接收已登录用户的通知，你首先需要获取在注册过程中使用的有效 OAuth 令牌。</span><span class="sxs-lookup"><span data-stu-id="d6824-202">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="d6824-203">你可以使用生成和管理 OAuth 令牌的首选方法。</span><span class="sxs-lookup"><span data-stu-id="d6824-203">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="d6824-204">示例应用使用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="d6824-204">The sample app used ADAL.</span></span> 

<span data-ttu-id="d6824-205">如果你使用的是 Microsoft 帐户，则需要在登录请求中包含以下权限：`wl.offline_access"`、`ccs.ReadWrite`、`wns.connect`、`asimovrome.telemetry` 和 `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`。</span><span class="sxs-lookup"><span data-stu-id="d6824-205">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="d6824-206">如果你使用的是 Azure AD 帐户，则需要请求以下受众：`https://cdpcs.access.microsoft.com`。</span><span class="sxs-lookup"><span data-stu-id="d6824-206">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>

## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="d6824-207">将用户帐户添加到平台</span><span class="sxs-lookup"><span data-stu-id="d6824-207">Adding the user account to the platform</span></span> 

<span data-ttu-id="d6824-208">你需要使用 SDK 注册已登录用户的帐户，这涉及添加帐户并注册推送通道以通过 FCM 接收初始推送通知。</span><span class="sxs-lookup"><span data-stu-id="d6824-208">You need to register the signed in user account with the SDK, which involves adding the account and registering a push channel in order to receive the initial push notifications through FCM.</span></span> 

```Java
public AsyncOperation<Boolean> prepareAccountAsync(final Context context) {
    // Accounts can be in 3 different scenarios:
    // 1: cached account in good standing (initialized in the SDK and our token cache).
    // 2: account missing from the SDK but present in our cache: Add and initialize account.
    // 3: account missing from our cache but present in the SDK. Log the account out async

    // Subcomponents (e.g. UserDataFeed) can only be initialized when an account is in both the app cache
    // and the SDK cache.
    // For scenario 1, initialize our subcomponents.
    // For scenario 2, subcomponents will be initialized after InitializeAccountAsync registers the account with the SDK.
    // For scenario 3, InitializeAccountAsync will unregister the account and subcomponents will never be initialized.
    switch (mState) {
        // Scenario 1
        case IN_APP_CACHE_AND_SDK_CACHE:
            mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
            return registerAccountWithSdkAsync();
        // Scenario 2
        case IN_APP_CACHE_ONLY: {
            // Add the this account to the ConnectedDevicesPlatform.AccountManager
            return mPlatform.getAccountManager().addAccountAsync(mAccount).thenComposeAsync((ConnectedDevicesAddAccountResult result) -> {
                // We failed to add the account, so exit with a failure to prepare bool
                if (result.getStatus() != ConnectedDevicesAccountAddedStatus.SUCCESS) {
                    result.getStatus());
                    return AsyncOperation.completedFuture(false);
                }

                // Set the registration state of this account as in both app and sdk cache
                mState = AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE;
                mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
                return registerAccountWithSdkAsync();
            });
        }
        // Scenario 3
        case IN_SDK_CACHE_ONLY:
            // Remove the account from the SDK since the app has no knowledge of it
            mPlatform.getAccountManager().removeAccountAsync(mAccount);
            // This account could not be prepared
            return AsyncOperation.completedFuture(false);
        default:
            // This account could not be prepared
            Log.e(TAG, "Failed to prepare account " + mAccount.getId() + " due to unknown state!");
            return AsyncOperation.completedFuture(false);
    }
}
```

```Java
public AsyncOperation<Boolean> registerAccountWithSdkAsync() {
    if (mState != AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE) {
        AsyncOperation<Boolean> toReturn = new AsyncOperation<>();
        toReturn.completeExceptionally(new IllegalStateException("Cannot register this account due to bad state: " + mAccount.getId()));
        return toReturn;
    }

    // Grab the shared GCM/FCM notification token from this app's BroadcastReceiver
    return RomeNotificationReceiver.getNotificationRegistrationAsync().thenComposeAsync((ConnectedDevicesNotificationRegistration notificationRegistration) -> {
        // Perform the registration using the NotificationRegistration
        return mPlatform.getNotificationRegistrationManager().registerAsync(mAccount, notificationRegistration)
            .thenComposeAsync((result) -> {
                if (result.getStatus() == ConnectedDevicesNotificationRegistrationStatus.SUCCESS) {
                    Log.i(TAG, "Successfully registered account " + mAccount.getId() + " for cloud notifications");
                } else {
                    // It would be a good idea for apps to take a look at the different statuses here and perhaps attempt some sort of remediation.
                    // For example, token request failed could mean that the user needs to sign in again. An app could prompt the user for this action 
                    // and retry the operation afterwards.
                    Log.e(TAG, "Failed to register account " + mAccount.getId() + " for cloud notifications!");
                    return AsyncOperation.completedFuture(false);
                }

                return mUserNotificationsManager.registerForAccountAsync();
            });
    });
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="d6824-209">订阅以接收用户的通知</span><span class="sxs-lookup"><span data-stu-id="d6824-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="d6824-210">你需要为此已登录用户实例化应用程序的 **UserDataFeed** 对象。</span><span class="sxs-lookup"><span data-stu-id="d6824-210">You need to instantiate a **UserDataFeed** object for your application for this logged in user.</span></span> <span data-ttu-id="d6824-211">你的应用程序由你在[跨设备体验载入](notifications-integration-cross-device-experiences-onboarding.md)过程中提供的跨平台应用 ID 进行标识。</span><span class="sxs-lookup"><span data-stu-id="d6824-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md).</span></span>

```Java
public UserNotificationsManager(@NonNull Context context, @NonNull ConnectedDevicesAccount account, @NonNull ConnectedDevicesPlatform platform)
{
    Context context = new Context;
    UserDataFeed feed = UserDataFeed.getForAccount(account, platform, Secrets.APP_HOST_NAME);
    UserNotificationChannel channel = new UserNotificationChannel(feed);
    UserNotificationReader reader = channel.createReader();
    reader.dataChanged().subscribe((reader, aVoid) -> readFromCache(reader));
    }
}
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="d6824-212">接收和管理用户通知</span><span class="sxs-lookup"><span data-stu-id="d6824-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="d6824-213">本主题前面的流程图显示，处理来自应用服务器的新传入通知的编程模式与处理从另一个应用客户端实例启动的通知更新或删除的编程模式类似。</span><span class="sxs-lookup"><span data-stu-id="d6824-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="d6824-214">以下是处理这些数据更改的步骤。</span><span class="sxs-lookup"><span data-stu-id="d6824-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="d6824-215">处理传入推送通知信号</span><span class="sxs-lookup"><span data-stu-id="d6824-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="d6824-216">所有类型的用户通知数据更改均会生成一个作为推送通知传递至应用客户端的信号。</span><span class="sxs-lookup"><span data-stu-id="d6824-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="d6824-217">对于 Android 应用，信号将作为 FCM 推送数据消息的一部分传递。</span><span class="sxs-lookup"><span data-stu-id="d6824-217">For Android apps, the signal is delivered as a FCM push data message.</span></span> <span data-ttu-id="d6824-218">接收数据消息信号时，应用应调用 **TryParse** 以触发 SDK 从 Microsoft Graph 通知服务中提取实际数据更改。</span><span class="sxs-lookup"><span data-stu-id="d6824-218">On receiving the data message signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```Java
public void onMessageReceived(RemoteMessage message) {
    Map data = message.getData();
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.tryParse(data);

    if (notification != null) {
        try {
            ConnectedDevicesPlatform platform = ConnectedDevicesManager.getConnectedDevicesManager(getApplicationContext()).getPlatform();

            // NOTE: it may be useful to attach completion to this async in order to know when the notification is done being processed.
            // This would be a good time to stop a background service or otherwise cleanup.
            platform.processNotificationAsync(notification);
        } catch (Exception e) {
            Log.e(TAG, "Failed to process FCM notification" + e.getMessage());
        }
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="d6824-219">处理用户通知数据更改</span><span class="sxs-lookup"><span data-stu-id="d6824-219">Handling user notification data changes</span></span>

<span data-ttu-id="d6824-220">SDK 成功完成数据更改提取之后，将会调用事件回调且应用客户端有望处理通知创建、更新或删除。</span><span class="sxs-lookup"><span data-stu-id="d6824-220">After the SDK successfully completes fetching the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```Java
private void readFromCache(final UserNotificationReader reader)
{
    reader.readBatchAsync(Long.MAX_VALUE).thenAccept(notifications -> {
        synchronized (this) {
            for (final UserNotification notification : notifications) {
                if (notification.getStatus() == UserNotificationStatus.ACTIVE) {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));

                    if (notification.getUserActionState() == UserNotificationUserActionState.NO_INTERACTION) {
                        mNewNotifications.add(notification);
                        if (notification.getReadState() != UserNotificationReadState.READ) {
                            clearNotification(mContext.getApplicationContext(), notification.getId());
                            addNotification(mContext.getApplicationContext(), notification.getContent(), notification.getId());
                        }
                    } else {
                        clearNotification(mContext.getApplicationContext(), notification.getId());
                    }

                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    mHistoricalNotifications.add(0, notification);
                } else {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));
                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    clearNotification(mContext.getApplicationContext(), notification.getId());
                }
            }
        }

    });
}
```

### <a name="update-state-of-a-notification"></a><span data-ttu-id="d6824-221">更新通知状态</span><span class="sxs-lookup"><span data-stu-id="d6824-221">Update state of a notification</span></span>

<span data-ttu-id="d6824-222">如果从此应用客户端实例发起通知状态更改（例如，如果此设备上的定制通知弹出窗口由用户激活），则应用需要调用 SDK 更新通知状态，以便在同一用户使用的所有设备中同步此状态更改操作。</span><span class="sxs-lookup"><span data-stu-id="d6824-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```Java
notification.setUserActionState(UserNotificationUserActionState.ACTIVATED);
notification.saveAsync().whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully activated the notification");
    }
});

```

### <a name="delete-a-notification"></a><span data-ttu-id="d6824-223">删除通知</span><span class="sxs-lookup"><span data-stu-id="d6824-223">Delete a notification</span></span>

<span data-ttu-id="d6824-224">如果从此应用客户端实例发起通知删除（例如，如果此通知对应的任务标记为“完成”并从应用数据库中删除），则应用需要调用 SDK 删除通知，以便在同一用户使用的所有设备中同步此删除操作。</span><span class="sxs-lookup"><span data-stu-id="d6824-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="d6824-225">仅当通知过期或者被显式删除时，它才会从用户通知存储区中删除。</span><span class="sxs-lookup"><span data-stu-id="d6824-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="d6824-226">将 **UserActionState** 更新为“已消除”时，用户通知不会删除，因为 **UserActionState** 的语义定义是由应用程序本身定义。</span><span class="sxs-lookup"><span data-stu-id="d6824-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```Java
channel.deleteUserNotificationAsync(notification.getId()).whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully deleted the notification");
    }
});
```

## <a name="see-also"></a><span data-ttu-id="d6824-227">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d6824-227">See also</span></span>

- <span data-ttu-id="d6824-228">[API 参考](https://docs.microsoft.com/zh-CN/windows/project-rome/notifications/api-reference-for-android)，以获取与 SDK 中的通知功能相关的整套 API。</span><span class="sxs-lookup"><span data-stu-id="d6824-228">[API reference](https://docs.microsoft.com/zh-CN/windows/project-rome/notifications/api-reference-for-android) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="d6824-229">适用于 Android 应用的[客户端示例](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample)。</span><span class="sxs-lookup"><span data-stu-id="d6824-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample) for Android apps.</span></span>
- <span data-ttu-id="d6824-230">适合于发布通知的[应用服务器示例](notifications-integrating-app-server.md)。</span><span class="sxs-lookup"><span data-stu-id="d6824-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
