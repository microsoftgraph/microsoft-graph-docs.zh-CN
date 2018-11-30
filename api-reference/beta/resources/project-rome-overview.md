---
title: '使用 Microsoft Graph API 来处理项目 Rome '
description: '项目 Rome 是 Microsoft 旨在构建一个平台，使应用程序开发人员可以构建出色的跨设备体验。 项目 Rome 启用连接不同的服务和客户端终结点，当用户迹象使用同一 Microsoft 帐户或工作或学校帐户时的不同功能。 这样，您可以实现跨设备和跨平台围绕用户任务，而不是设备的体验。 '
ms.openlocfilehash: f779c04a76331d27fdcae6436e758bacfc052f8e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043778"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="5e728-105">使用 Microsoft Graph API 来处理项目 Rome</span><span class="sxs-lookup"><span data-stu-id="5e728-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

> <span data-ttu-id="5e728-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e728-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e728-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e728-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e728-108">[项目 Rome](https://developer.microsoft.com/en-us/windows/project-rome)是 Microsoft 旨在构建一个平台，使应用程序开发人员可以构建出色的跨设备体验。</span><span class="sxs-lookup"><span data-stu-id="5e728-108">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="5e728-109">项目 Rome 启用连接不同的服务和客户端终结点，当用户迹象使用同一 Microsoft 帐户或工作或学校帐户时的不同功能。</span><span class="sxs-lookup"><span data-stu-id="5e728-109">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="5e728-110">这样，您可以实现跨设备和跨平台围绕用户任务，而不是设备的体验。</span><span class="sxs-lookup"><span data-stu-id="5e728-110">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="5e728-111">三个主要项目 Rome 功能公开通过 Microsoft Graph 可帮助您启用绝佳跨设备体验： 活动、 设备和通知。</span><span class="sxs-lookup"><span data-stu-id="5e728-111">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="5e728-112">活动</span><span class="sxs-lookup"><span data-stu-id="5e728-112">Activities</span></span>

<span data-ttu-id="5e728-113">跨设备和平台中，Microsoft Graph 中的活动使您能够与您的应用程序的驱动器用户工作效率。</span><span class="sxs-lookup"><span data-stu-id="5e728-113">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="5e728-114">活动用户工作效率的单位，包括三个组件：</span><span class="sxs-lookup"><span data-stu-id="5e728-114">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="5e728-115">深度链接</span><span class="sxs-lookup"><span data-stu-id="5e728-115">A deep link</span></span>
- <span data-ttu-id="5e728-116">直观表示形式</span><span class="sxs-lookup"><span data-stu-id="5e728-116">A visual representation</span></span>
- <span data-ttu-id="5e728-117">描述该活动的内容元数据使用[https://schema.org/](https://schema.org/)共享词汇</span><span class="sxs-lookup"><span data-stu-id="5e728-117">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="5e728-118">应用程序创建会话时, 的历史记录项添加到活动的以反映用户工作效率期。</span><span class="sxs-lookup"><span data-stu-id="5e728-118">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="5e728-119">每次用户 reengages 与活动，新的历史记录项添加到活动以应计用户工作效率。</span><span class="sxs-lookup"><span data-stu-id="5e728-119">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="5e728-120">当应用程序发布用户活动对象时，该对象将显示某些 Windows; 中新的 UI 曲面例如，Cortana 通知和日程表。</span><span class="sxs-lookup"><span data-stu-id="5e728-120">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="5e728-121">活动对象中，可以指定丰富的元数据 （以允许活动在适当的上下文中呈现） 和丰富的视觉效果 （使用[自适应卡片](https://adaptivecards.io/)标记）。</span><span class="sxs-lookup"><span data-stu-id="5e728-121">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="5e728-122">以下 Microsoft Graph Api 可用于创建和检索用户活动：</span><span class="sxs-lookup"><span data-stu-id="5e728-122">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="5e728-123">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="5e728-123">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="5e728-124">获取活动</span><span class="sxs-lookup"><span data-stu-id="5e728-124">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="5e728-125">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="5e728-125">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="5e728-126">删除活动</span><span class="sxs-lookup"><span data-stu-id="5e728-126">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="5e728-127">创建或替换历史记录项</span><span class="sxs-lookup"><span data-stu-id="5e728-127">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="5e728-128">删除历史记录项</span><span class="sxs-lookup"><span data-stu-id="5e728-128">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="5e728-129">设备</span><span class="sxs-lookup"><span data-stu-id="5e728-129">Devices</span></span>

<span data-ttu-id="5e728-130">您可以在 Microsoft Graph 中使用项目 Rome Api:</span><span class="sxs-lookup"><span data-stu-id="5e728-130">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="5e728-131">发现并连接到用户的设备</span><span class="sxs-lookup"><span data-stu-id="5e728-131">Discover and connect to user's devices</span></span>
- <span data-ttu-id="5e728-132">远程启动这些设备上的应用程序</span><span class="sxs-lookup"><span data-stu-id="5e728-132">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="5e728-133">将邮件发送到您在这些设备上的应用程序</span><span class="sxs-lookup"><span data-stu-id="5e728-133">Send messages to your apps on those devices</span></span>

<span data-ttu-id="5e728-134">使用这些 Api，您可以生成创建跨越单个设备的丰富体验的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5e728-134">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="5e728-135">例如，您可以扩展您的应用程序，以更大的屏幕上启动。</span><span class="sxs-lookup"><span data-stu-id="5e728-135">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="5e728-136">也可以在另一个用户的设备上创建应用程序的辅助体验。</span><span class="sxs-lookup"><span data-stu-id="5e728-136">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="5e728-137">以下 Microsoft Graph Api 可用于与其他 Windows 设备进行通信：</span><span class="sxs-lookup"><span data-stu-id="5e728-137">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="5e728-138">列出用户的设备</span><span class="sxs-lookup"><span data-stu-id="5e728-138">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="5e728-139">向设备发送命令</span><span class="sxs-lookup"><span data-stu-id="5e728-139">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="5e728-140">获取 status 命令</span><span class="sxs-lookup"><span data-stu-id="5e728-140">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="5e728-141">Notifications</span><span class="sxs-lookup"><span data-stu-id="5e728-141">Notifications</span></span>

<span data-ttu-id="5e728-142">您可以使用在 Microsoft Graph 通知 Api 个相同的用户登录的多个终结点发送通知。</span><span class="sxs-lookup"><span data-stu-id="5e728-142">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="5e728-143">发布而不是担心设备地址/通道通知时，您可以直接目标用户。</span><span class="sxs-lookup"><span data-stu-id="5e728-143">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="5e728-144">这种方式，您可以集中设计 human 为中心，而不是一种设备中心的方法中的右侧的通知方案。</span><span class="sxs-lookup"><span data-stu-id="5e728-144">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="5e728-145">您可以发布原始数据通知或直接 visual 通知。</span><span class="sxs-lookup"><span data-stu-id="5e728-145">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="5e728-146">原始数据通知传递到设备的终结点，可以使用[客户端 SDK](https://github.com/Microsoft/project-rome) （Microsoft Graph 通知 SDK for Windows，适用于 iOS 的项目 Rome SDK 和 Android） 接收和管理通知。</span><span class="sxs-lookup"><span data-stu-id="5e728-146">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="5e728-147">直接的可视通知传递到设备的终结点，它向用户显示特定于平台的本机通知。</span><span class="sxs-lookup"><span data-stu-id="5e728-147">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="5e728-148">有关详细信息，请参阅[创建和发送通知](../api/projectrome-notification-post.md)。</span><span class="sxs-lookup"><span data-stu-id="5e728-148">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

