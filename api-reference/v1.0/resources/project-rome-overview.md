---
title: 使用 Microsoft Graph API 处理 Project 罗马
description: 项目罗马是构建跨设备体验平台的 Microsoft 计划。 Project 罗马启用本地客户端或服务上的应用程序，以便在用户使用用于登录客户端设备的相同 Microsoft 帐户登录时与远程主机上的应用程序和服务进行交互。 这使您可以对用户任务（而不是设备）周围的跨设备和跨平台体验进行编程。
localization_priority: Normal
author: ailae
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: f7e68c50e6e58c4f9f7a2b04bf2f26361fef6063
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806973"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="37a94-105">使用 Microsoft Graph API 处理 Project 罗马</span><span class="sxs-lookup"><span data-stu-id="37a94-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="37a94-106">[项目罗马](https://developer.microsoft.com/en-us/windows/project-rome) 是构建跨设备体验平台的 Microsoft 计划。</span><span class="sxs-lookup"><span data-stu-id="37a94-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="37a94-107">Project 罗马启用本地客户端或服务上的应用程序，以便在用户使用用于登录客户端设备的相同 Microsoft 帐户登录时与远程主机上的应用程序和服务进行交互。</span><span class="sxs-lookup"><span data-stu-id="37a94-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="37a94-108">这使您可以对用户任务（而不是设备）周围的跨设备和跨平台体验进行编程。</span><span class="sxs-lookup"><span data-stu-id="37a94-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="37a94-109">通过 Microsoft Graph 公开一个关键组件，以启用以下体验：活动。</span><span class="sxs-lookup"><span data-stu-id="37a94-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="37a94-110">活动</span><span class="sxs-lookup"><span data-stu-id="37a94-110">Activities</span></span>

<span data-ttu-id="37a94-111">通过 Microsoft Graph 中的活动，您可以在设备和平台之间推动用户参与应用。</span><span class="sxs-lookup"><span data-stu-id="37a94-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="37a94-112">活动是用户接洽的单位，由三个组件组成：</span><span class="sxs-lookup"><span data-stu-id="37a94-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="37a94-113">深层链接</span><span class="sxs-lookup"><span data-stu-id="37a94-113">A deep link</span></span>
- <span data-ttu-id="37a94-114">可视化表示形式</span><span class="sxs-lookup"><span data-stu-id="37a94-114">A visual representation</span></span>
- <span data-ttu-id="37a94-115">使用共享词汇描述活动的内容元数据 [https://schema.org/](https://schema.org/)</span><span class="sxs-lookup"><span data-stu-id="37a94-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="37a94-116">当应用程序创建会话时，会向活动中添加一个历史记录项目，以反映用户参与的时段。</span><span class="sxs-lookup"><span data-stu-id="37a94-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="37a94-117">用户每次 reengages 活动时，都会向活动中添加一个新的历史记录项，以计入用户约定。</span><span class="sxs-lookup"><span data-stu-id="37a94-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="37a94-118">当应用程序发布用户活动对象时，该对象将显示在 Windows 中的一些新 UI 图面上;例如，Cortana 通知和时间线。</span><span class="sxs-lookup"><span data-stu-id="37a94-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="37a94-119">您可以指定丰富的元数据 (，以允许在活动对象中使用 [自适应卡片](https://adaptivecards.io/) 标记) 仅在适当的上下文中显示活动) 和丰富的视觉对象 (。</span><span class="sxs-lookup"><span data-stu-id="37a94-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="37a94-120">您可以使用以下 Microsoft Graph Api 来创建和检索用户活动：</span><span class="sxs-lookup"><span data-stu-id="37a94-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="37a94-121">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="37a94-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="37a94-122">获取活动</span><span class="sxs-lookup"><span data-stu-id="37a94-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="37a94-123">获取最近的活动</span><span class="sxs-lookup"><span data-stu-id="37a94-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="37a94-124">删除活动</span><span class="sxs-lookup"><span data-stu-id="37a94-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="37a94-125">创建或替换历史记录项</span><span class="sxs-lookup"><span data-stu-id="37a94-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="37a94-126">删除历史记录项</span><span class="sxs-lookup"><span data-stu-id="37a94-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a><span data-ttu-id="37a94-127">最近更新</span><span class="sxs-lookup"><span data-stu-id="37a94-127">What's new</span></span>
<span data-ttu-id="37a94-128">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="37a94-128">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>