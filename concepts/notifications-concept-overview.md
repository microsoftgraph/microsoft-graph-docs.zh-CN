---
title: '利用 Microsoft Graph 通知实现以人为中心的通知体验 '
description: '通知是与应用程序用户再次交互的最有效的方式之一。 绝佳的通知体验有助于在你和你的应用程序用户之间开启一个近乎实时的沟通渠道，这转而可在适当的时间提高应用参与度、帮助用户提升工作效率，并就重要事件或可能需采取的及时操作提醒他们。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: b83e91be74de44dbd72315331964379992b811de
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133563"
---
# <a name="enabling-human-centric-notification-experiences-using-microsoft-graph-notifications"></a><span data-ttu-id="4b8c4-104">利用 Microsoft Graph 通知实现以人为中心的通知体验</span><span class="sxs-lookup"><span data-stu-id="4b8c4-104">Enabling human-centric notification experiences using Microsoft Graph notifications</span></span>

<span data-ttu-id="4b8c4-105">通知是与应用程序用户再次交互的最有效的方式之一。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-105">Notifications are one of the most effective and direct ways to communicate to and engage with your users.</span></span> <span data-ttu-id="4b8c4-106">绝佳的通知体验有助于在你和你的用户之间开启一个近乎实时的沟通渠道，这转而可在适当的时间提高应用参与度、帮助用户提升工作效率，并就重要事件或必需操作提醒他们。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-106">A great notification experience can help open a near real-time communication channel between you and your users, and that in turn can increase app engagement at the right time, make users more productive, and alert them to important events or required actions.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/cmpPFhrS8ZA]

<span data-ttu-id="4b8c4-107">如今，用户可通过各种各样的平台，在各种外观设置下访问你的应用程序和服务。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-107">Today, users can access your applications and services via a wide variety of platforms and form factors.</span></span> <span data-ttu-id="4b8c4-108">设备如此多样，就需要你了解和支持多平台通知系统、将用户映射到终结点，并保证不同设备的通知状态一致。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-108">This mix of devices requires that you understand and support multiplatform notification systems, map users to endpoints, and maintain notification state across devices.</span></span> 

<span data-ttu-id="4b8c4-109">其他的大部分通知系统都消除了理解和定向平台专用推送通知系统的需求，但仍然设计为针对每款设备。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-109">Most other notification systems eliminate the need to understand and target platform-specific push notification systems, but are still  designed to target each device.</span></span> <span data-ttu-id="4b8c4-110">Microsoft Graph 提供了一种以人为中心的方法，让你能够应对所有设备终结点中的应用。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-110">Microsoft Graph notifications provide a human-centric approach that gives you the ability to target your  users across any and all device endpoints.</span></span>

![一张图像，其中显示与 Microsoft Graph 通信来向多个终结点发送通知的应用服务](images/notifications-flow-overview.png)

## <a name="why-integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="4b8c4-112">为何要与 Microsoft Graph 通知集成？</span><span class="sxs-lookup"><span data-stu-id="4b8c4-112">Why integrate with Microsoft Graph notifications?</span></span>

<span data-ttu-id="4b8c4-113">Microsoft Graph 通知提供了一个以用户为中心的通知平台，给你的应用程序带去四大关键优势。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-113">Microsoft Graph notifications provide a user-centric notification platform that brings four key benefits to your applications.</span></span>

### <a name="effortlessly-target-your-user-for-notification-delivery-across-different-endpoints"></a><span data-ttu-id="4b8c4-114">轻松实现用户定向，跨不同终结点提供通知</span><span class="sxs-lookup"><span data-stu-id="4b8c4-114">Effortlessly target your user for notification delivery across different endpoints</span></span>

<span data-ttu-id="4b8c4-115">可借助通知 API，定向 Microsoft 个人帐户或 Azure Active Directory (Azure AD) 工作/学校帐户来发送通知。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-115">You can use the notifications API to target a personal Microsoft account or a work or school Azure Active Directory (Azure AD) account to deliver notifications.</span></span> <span data-ttu-id="4b8c4-116">该平台将此通知分发给运行你的应用程序或服务的所有用户终结点，例如 Windows UWP、Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-116">The platform distributes this notification to all user endpoints running your application or service, including Windows UWP, Android, and iOS.</span></span> <span data-ttu-id="4b8c4-117">这一功能可确保无论用户身在何处，都有相应的通知可发送给他们，从而最大限度扩大触及范围。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-117">This capability helps maximize outreach by ensuring appropriate notifications can reach your target, wherever they are.</span></span>

### <a name="easily-manage-notifications-across-endpoints"></a><span data-ttu-id="4b8c4-118">跨终结点轻松管理通知</span><span class="sxs-lookup"><span data-stu-id="4b8c4-118">Easily manage notifications across endpoints</span></span>

<span data-ttu-id="4b8c4-119">借助客户端应用程序中的 [Microsoft Graph 通知客户端 SDK](https://github.com/microsoft/project-rome)，可更改通知的状态并跨所有终结点通知此状态。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-119">Using the [Microsoft Graph notifications client SDK](https://github.com/microsoft/project-rome) within your client application, you can update the state of a notification and sync that state across all endpoints.</span></span> <span data-ttu-id="4b8c4-120">例如，当用户对一个设备上的通知执行操作时，你可以更新此通知的状态（例如将其设置为已读或已消除），并向所有其他终结点分发同一状态更改。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-120">For example, when a user acts on a notification on one device, you can update the state of this notification (such as marking it as read or dismissed), and the same state change will be distributed to all other endpoints.</span></span> <span data-ttu-id="4b8c4-121">Microsoft Graph 通知 API 可集中性地跟踪用户通知的状态，让你能够确保你的通知被处理过一次并在所有位置关闭，从而减少冗余，同时确保客户体验极佳。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-121">The Microsoft Graph notifications API tracks the state of your users' notifications in a centralized way, making it easy for you to ensure that your notifications are handled once, and dismissed everywhere.</span></span>

### <a name="retrieve-notification-state-and-history"></a><span data-ttu-id="4b8c4-122">检索通知状态和历史记录</span><span class="sxs-lookup"><span data-stu-id="4b8c4-122">Retrieve notification state and history</span></span>

<span data-ttu-id="4b8c4-123">可使用通知 API 根据所定义的过期时间（最多 30 天）来检索通知历史记录。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-123">You can use the notifications API to retrieve notification history based on an expiration time you define (up to 30 days).</span></span> <span data-ttu-id="4b8c4-124">标记为“已读”或“已关闭”的通知仍能在历史记录中检索到，从而能在应用内查看通知历史记录，并可在见解和智能的基础上进行构建。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-124">Notifications that are marked as read or dismissed are still retrievable from the history, enabling in-app views of notification history as well as enabling you to build on insights and intelligence.</span></span>

### <a name="privacy-and-compliance"></a><span data-ttu-id="4b8c4-125">隐私与合规性</span><span class="sxs-lookup"><span data-stu-id="4b8c4-125">Privacy and compliance</span></span>

<span data-ttu-id="4b8c4-126">Microsoft Graph 通知满足大部分企业合规性要求，包括 ISO 27001、ISO 27018、EUMC、HIPAA、SOC 1 和 SOC 2，当然也符合 GDPR。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-126">Microsoft Graph notifications meet most enterprise compliance requirements, including ISO 27001, ISO 27018, EUMC, HIPAA, SOC 1, SOC 2, and of course GDPR.</span></span>

## <a name="how-do-i-get-started"></a><span data-ttu-id="4b8c4-127">如何开始使用？</span><span class="sxs-lookup"><span data-stu-id="4b8c4-127">How do I get started?</span></span>

<span data-ttu-id="4b8c4-128">首先，请查看[集成概述](notifications-integration-e2e-overview.md)部分，了解可如何在应用程序中集成以用户为中心的通知。</span><span class="sxs-lookup"><span data-stu-id="4b8c4-128">To get started, see the [integration overview](notifications-integration-e2e-overview.md) section to learn how you can integrate user-centric notifications within your application.</span></span>
