---
title: '使用 Microsoft Graph API 处理 Project 罗马 '
description: '项目罗马是 Microsoft 计划，用于构建一个平台，使应用程序开发人员能够生成强大的跨设备体验。 Project 罗马启用不同的功能，以便在用户使用相同的 Microsoft 帐户或工作或学校帐户登录时连接不同的服务和客户端终结点。 这使您能够实现以用户任务（而不是设备）为中心的跨设备和跨平台体验。 '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: f9d9900aecb7226ed33c5e0cf51c7ccfaf3d2e8d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809319"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="eec5c-105">使用 Microsoft Graph API 处理 Project 罗马</span><span class="sxs-lookup"><span data-stu-id="eec5c-105">Use the Microsoft Graph API to work with Project Rome</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eec5c-106">[项目罗马](https://developer.microsoft.com/en-us/windows/project-rome) 是 Microsoft 计划，用于构建一个平台，使应用程序开发人员能够生成强大的跨设备体验。</span><span class="sxs-lookup"><span data-stu-id="eec5c-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="eec5c-107">Project 罗马启用不同的功能，以便在用户使用相同的 Microsoft 帐户或工作或学校帐户登录时连接不同的服务和客户端终结点。</span><span class="sxs-lookup"><span data-stu-id="eec5c-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="eec5c-108">这使您能够实现以用户任务（而不是设备）为中心的跨设备和跨平台体验。</span><span class="sxs-lookup"><span data-stu-id="eec5c-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="eec5c-109">通过 Microsoft Graph 公开三个关键项目罗马功能，可帮助您实现大量的跨设备体验：活动、设备和通知。</span><span class="sxs-lookup"><span data-stu-id="eec5c-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span>

## <a name="activities"></a><span data-ttu-id="eec5c-110">活动</span><span class="sxs-lookup"><span data-stu-id="eec5c-110">Activities</span></span>

<span data-ttu-id="eec5c-111">通过 Microsoft Graph 中的活动，您可以在设备和平台之间推动用户参与应用。</span><span class="sxs-lookup"><span data-stu-id="eec5c-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="eec5c-112">活动是用户接洽的单位，由三个组件组成：</span><span class="sxs-lookup"><span data-stu-id="eec5c-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="eec5c-113">深层链接</span><span class="sxs-lookup"><span data-stu-id="eec5c-113">A deep link</span></span>
- <span data-ttu-id="eec5c-114">可视化表示形式</span><span class="sxs-lookup"><span data-stu-id="eec5c-114">A visual representation</span></span>
- <span data-ttu-id="eec5c-115">使用共享词汇描述活动的内容元数据 [https://schema.org/](https://schema.org/)</span><span class="sxs-lookup"><span data-stu-id="eec5c-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="eec5c-116">当应用程序创建会话时，会向活动中添加一个历史记录项目，以反映用户参与的时段。</span><span class="sxs-lookup"><span data-stu-id="eec5c-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="eec5c-117">用户每次 reengages 活动时，都会向活动中添加一个新的历史记录项，以计入用户约定。</span><span class="sxs-lookup"><span data-stu-id="eec5c-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="eec5c-118">当应用程序发布用户活动对象时，该对象将显示在 Windows 中的一些新 UI 图面上;例如，Cortana 通知和时间线。</span><span class="sxs-lookup"><span data-stu-id="eec5c-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="eec5c-119">您可以指定丰富的元数据 (，以允许在活动对象中使用 [自适应卡片](https://adaptivecards.io/) 标记) 仅在适当的上下文中显示活动) 和丰富的视觉对象 (。</span><span class="sxs-lookup"><span data-stu-id="eec5c-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="eec5c-120">您可以使用以下 Microsoft Graph Api 来创建和检索用户活动：</span><span class="sxs-lookup"><span data-stu-id="eec5c-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="eec5c-121">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="eec5c-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="eec5c-122">获取活动</span><span class="sxs-lookup"><span data-stu-id="eec5c-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="eec5c-123">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="eec5c-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="eec5c-124">删除活动</span><span class="sxs-lookup"><span data-stu-id="eec5c-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="eec5c-125">创建或替换历史记录项</span><span class="sxs-lookup"><span data-stu-id="eec5c-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="eec5c-126">删除历史记录项</span><span class="sxs-lookup"><span data-stu-id="eec5c-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="eec5c-127">设备</span><span class="sxs-lookup"><span data-stu-id="eec5c-127">Devices</span></span>

<span data-ttu-id="eec5c-128">您可以使用 Microsoft Graph 中的 Project 罗马 Api 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="eec5c-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="eec5c-129">发现并连接到用户的设备</span><span class="sxs-lookup"><span data-stu-id="eec5c-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="eec5c-130">在这些设备上远程启动应用程序</span><span class="sxs-lookup"><span data-stu-id="eec5c-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="eec5c-131">将邮件发送到这些设备上的应用程序</span><span class="sxs-lookup"><span data-stu-id="eec5c-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="eec5c-132">使用这些 Api，您可以生成可在一个设备上创建丰富体验的应用程序。</span><span class="sxs-lookup"><span data-stu-id="eec5c-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="eec5c-133">例如，您可以扩展您的应用程序，使其在更大的屏幕上启动。</span><span class="sxs-lookup"><span data-stu-id="eec5c-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="eec5c-134">或者，您可以为用户设备上的另一个应用创建配套体验。</span><span class="sxs-lookup"><span data-stu-id="eec5c-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="eec5c-135">您可以使用以下 Microsoft Graph Api 与其他 Windows 设备进行通信：</span><span class="sxs-lookup"><span data-stu-id="eec5c-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="eec5c-136">列出用户的设备</span><span class="sxs-lookup"><span data-stu-id="eec5c-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="eec5c-137">向设备发送命令</span><span class="sxs-lookup"><span data-stu-id="eec5c-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="eec5c-138">获取命令状态</span><span class="sxs-lookup"><span data-stu-id="eec5c-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="whats-new"></a><span data-ttu-id="eec5c-139">最近更新</span><span class="sxs-lookup"><span data-stu-id="eec5c-139">What's new</span></span>
<span data-ttu-id="eec5c-140">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="eec5c-140">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>