---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5e56d74e35bf55caade6c0137619d0d24ecc7323
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865849"
---
# <a name="whats-new-in-microsoft-graph"></a><span data-ttu-id="98401-103">Microsoft Graph 新增功能</span><span class="sxs-lookup"><span data-stu-id="98401-103">What's new in Microsoft Graph</span></span>

<span data-ttu-id="98401-104">查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。</span><span class="sxs-lookup"><span data-stu-id="98401-104">See highlights of what's new in Microsoft Graph, and how you can [share your ideas](#want-to-stay-in-the-loop).</span></span> <span data-ttu-id="98401-105">有关 API 更新的完整列表，请参阅 API 更改日志的 [12 月](changelog.md#december-2019)和 [11 月](changelog.md#november-2019)部分。</span><span class="sxs-lookup"><span data-stu-id="98401-105">For a complete list of API updates, see the [December](changelog.md#december-2019) and [November](changelog.md#november-2019) sections of the API changelog.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="98401-106">_预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。</span><span class="sxs-lookup"><span data-stu-id="98401-106">Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to generally available (GA) status.</span></span> <span data-ttu-id="98401-107">不要在成品应用中使用预览功能。</span><span class="sxs-lookup"><span data-stu-id="98401-107">Do not use preview features in production apps.</span></span>

## <a name="february-2020-new-and-generally-available"></a><span data-ttu-id="98401-108">2020 年 2 月：新版本和正式版</span><span class="sxs-lookup"><span data-stu-id="98401-108">February 2020: New and generally available</span></span>

### <a name="calendar"></a><span data-ttu-id="98401-109">日历</span><span class="sxs-lookup"><span data-stu-id="98401-109">Calendar</span></span>
<span data-ttu-id="98401-110">浏览“[在共享或委派日历中创建事件](outlook-create-event-in-shared-delegated-calendar.md)”示例，或浏览可用于此流程期间的代理人、受邀者和日历所有者的操作与属性。</span><span class="sxs-lookup"><span data-stu-id="98401-110">Walk through an example of [creating an event in a shared or delegated calendar](outlook-create-event-in-shared-delegated-calendar.md), and the actions and properties available to the delegate, invitees, and calendar owner during this process.</span></span>

### <a name="security"></a><span data-ttu-id="98401-111">安全性</span><span class="sxs-lookup"><span data-stu-id="98401-111">Security</span></span>
<span data-ttu-id="98401-112">为了提升在订阅“[更改用户通知](webhooks.md)”的安全性，强制在通知流程中使用的客户端和网站服务器上[强制执行传输层安全性（TLS）1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2)或更高。</span><span class="sxs-lookup"><span data-stu-id="98401-112">To improve security when subscribing to [change notifications of user data](webhooks.md), [enforce Transport Layer Security (TLS) 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) or higher on clients and site servers used in the notification process.</span></span> <span data-ttu-id="98401-113">新要求自 2020 年 2 月 15 日起分阶段推出。</span><span class="sxs-lookup"><span data-stu-id="98401-113">The new requirement is rolled out in stages starting February 15 2020.</span></span> <span data-ttu-id="98401-114">到 2020 年 5 月 15 日，所有通知端点必须符合新的 TLS 要求。</span><span class="sxs-lookup"><span data-stu-id="98401-114">By May 15, 2020, all notification endpoints must meet the new TLS requirement.</span></span> <span data-ttu-id="98401-115">[找出推出阶段](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/)，如有必要，请使用新的 **latestSupportedTlsVersion** 属性作为临时解决方法，以避免订阅失败，然后再完成 TLS 升级。</span><span class="sxs-lookup"><span data-stu-id="98401-115">[Find out the stages of the rollout](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) and if necessary, use the new **latestSupportedTlsVersion** property as a temporary workaround to avoid subscription failures, before completing the TLS upgrade.</span></span>

## <a name="february-2020-new-in-preview"></a><span data-ttu-id="98401-116">2020 年 2 月：预览版新增功能</span><span class="sxs-lookup"><span data-stu-id="98401-116">February 2020: New in preview</span></span>

### <a name="calendar"></a><span data-ttu-id="98401-117">日历</span><span class="sxs-lookup"><span data-stu-id="98401-117">Calendar</span></span>
<span data-ttu-id="98401-118">参看“[管理日历共享和委派的预览版 API 所支持的任务](outlook-share-or-delegate-calendar.md)”。</span><span class="sxs-lookup"><span data-stu-id="98401-118">See [tasks supported by preview APIs that manage calendar sharing and delegation](outlook-share-or-delegate-calendar.md).</span></span>


## <a name="january-2020-new-and-generally-available"></a><span data-ttu-id="98401-119">2020 年 1 月：新版本和正式版</span><span class="sxs-lookup"><span data-stu-id="98401-119">January 2020: New and generally available</span></span>

### <a name="security"></a><span data-ttu-id="98401-120">安全性</span><span class="sxs-lookup"><span data-stu-id="98401-120">Security</span></span>
<span data-ttu-id="98401-121">作为客户警报管理的一部分，请使用 [update alert](/graph/api/alert-update?view=graph-rest-1.0) 方法并将“**注释**”字段更新为 `Closed in IPC` 或 `Closed in MCAS`。</span><span class="sxs-lookup"><span data-stu-id="98401-121">As part of customer alert management, use the [update alert](/graph/api/alert-update?view=graph-rest-1.0) method and update the **comments** field as either `Closed in IPC` or `Closed in MCAS`.</span></span>

### <a name="teamwork"></a><span data-ttu-id="98401-122">团队合作</span><span class="sxs-lookup"><span data-stu-id="98401-122">Teamwork</span></span>
<span data-ttu-id="98401-123">使用“[团队](/graph/api/resources/team?view=graph-rest-1.0)”的 **primaryChannel** 导航属性来访问默认频道，“**常规**”。</span><span class="sxs-lookup"><span data-stu-id="98401-123">Use the **primaryChannel** navigation property of a [team](/graph/api/resources/team?view=graph-rest-1.0) to access its default channel, **General**.</span></span>

### <a name="users"></a><span data-ttu-id="98401-124">用户</span><span class="sxs-lookup"><span data-stu-id="98401-124">Users</span></span>
<span data-ttu-id="98401-125">使用“**标识**”属性访问[用户](/graph/api/resources/user?view=graph-rest-1.0)可用于登录至 Azure AD 用户账户的一个或多个标识。</span><span class="sxs-lookup"><span data-stu-id="98401-125">Use the **identities** property to access one or more identities that a [user](/graph/api/resources/user?view=graph-rest-1.0) can use to sign in to an Azure AD user account.</span></span> <span data-ttu-id="98401-126">这些标识可由 Microsoft，组织或 Facebook、Google 或 Microsoft 等社交标识提供商提供。</span><span class="sxs-lookup"><span data-stu-id="98401-126">The identities can be provided by Microsoft, organizations, or social identity providers such as Facebook, Google, or Microsoft.</span></span> <span data-ttu-id="98401-127">此属性允许用户使用任一这些身份登录至用户账户。</span><span class="sxs-lookup"><span data-stu-id="98401-127">This property allows the user to sign in to the user account with any of these identities.</span></span>

## <a name="january-2020-new-in-preview"></a><span data-ttu-id="98401-128">2020 年 1 月：预览版新增功能</span><span class="sxs-lookup"><span data-stu-id="98401-128">January 2020: New in preview</span></span>

### <a name="devices-and-apps"></a><span data-ttu-id="98401-129">设备和应用</span><span class="sxs-lookup"><span data-stu-id="98401-129">Devices and apps</span></span>
<span data-ttu-id="98401-130">Intune [1 月](changelog.md#january-2020)更新。</span><span class="sxs-lookup"><span data-stu-id="98401-130">Intune [January](changelog.md#january-2020) updates.</span></span>

<!--
### Identity and access
Access specific types of [policies for an organization](/graph/api/resources/policy-overview?view=graph-rest-beta) using the `/policies` URL segment and specifying the policy type. For example, an organization can enforce a policy to automatically sign a user out from a web session after a period of inactivity; see CRUD operations for instances of [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). This is a [breaking change](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) to make it easier to discover all policies, by grouping all typed policies under the `/policies` segment. Access other typed policies in a similar approach: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), and [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta).
-->


## <a name="want-to-stay-in-the-loop"></a><span data-ttu-id="98401-131">保持循环</span><span class="sxs-lookup"><span data-stu-id="98401-131">Want to stay in the loop?</span></span>

<span data-ttu-id="98401-132">我们可以通过以下方式进行参与：</span><span class="sxs-lookup"><span data-stu-id="98401-132">Here are some ways we can engage:</span></span>

- <span data-ttu-id="98401-133">是否有希望 Microsoft Graph 支持的方案？</span><span class="sxs-lookup"><span data-stu-id="98401-133">Are there scenarios you'd like Microsoft Graph to support?</span></span> <span data-ttu-id="98401-134">在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。</span><span class="sxs-lookup"><span data-stu-id="98401-134">Suggest and vote for new features at [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
    <span data-ttu-id="98401-135">某些新功能来源于开发人员社区的热门请求。</span><span class="sxs-lookup"><span data-stu-id="98401-135">Some new features originate as popular requests from the developer community.</span></span> <span data-ttu-id="98401-136">Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：</span><span class="sxs-lookup"><span data-stu-id="98401-136">The Microsoft Graph team regularly evaluates customer needs and releases new features in the following order:</span></span>

    1. <span data-ttu-id="98401-137">处于**_预览_** 状态的 Debut。</span><span class="sxs-lookup"><span data-stu-id="98401-137">Debut in **_preview_** status.</span></span> <span data-ttu-id="98401-138">任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。</span><span class="sxs-lookup"><span data-stu-id="98401-138">Any related REST API updates are in the beta endpoint (`https://graph.microsoft.com/beta`).</span></span>  

    2. <span data-ttu-id="98401-139">如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。</span><span class="sxs-lookup"><span data-stu-id="98401-139">Promoted to **_general availability_ (GA)** status, if sufficient feedback indicates viability.</span></span> <span data-ttu-id="98401-140">任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。</span><span class="sxs-lookup"><span data-stu-id="98401-140">Any related REST API updates are added to the v1.0 endpoint (`https://graph.microsoft.com/v1.0`).</span></span> 
- <span data-ttu-id="98401-141">成为 Microsoft Graph 社区中的活跃成员!</span><span class="sxs-lookup"><span data-stu-id="98401-141">Be an active member in the Microsoft Graph community!</span></span> <span data-ttu-id="98401-142">[参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。</span><span class="sxs-lookup"><span data-stu-id="98401-142">[Join](https://aka.ms/microsoftgraphcall) the monthly Microsoft Graph community call.</span></span>
- <span data-ttu-id="98401-143">注册 [office 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Office 365, 然后开始开发! </span><span class="sxs-lookup"><span data-stu-id="98401-143">Sign up for the [Office 365 developer program](https://developer.microsoft.com/office/dev-program), get a free Office 365 subscription, and start developing!</span></span>


## <a name="see-also"></a><span data-ttu-id="98401-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="98401-144">See also</span></span>
- <span data-ttu-id="98401-145">定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 </span><span class="sxs-lookup"><span data-stu-id="98401-145">Check out the [Microsoft Graph developer blog](https://developer.microsoft.com/graph/blogs/) periodically for release announcements and helpful resources.</span></span>
- <span data-ttu-id="98401-146">浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。</span><span class="sxs-lookup"><span data-stu-id="98401-146">Browse details of Microsoft Graph API additions, and API behavior updates in the [changelog](changelog.md).</span></span>
- <span data-ttu-id="98401-147">查找[早期版本的重点内容](whats-new-earlier.md)。</span><span class="sxs-lookup"><span data-stu-id="98401-147">Find [highlights of earlier releases](whats-new-earlier.md).</span></span>
- <span data-ttu-id="98401-148">了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。</span><span class="sxs-lookup"><span data-stu-id="98401-148">Learn more about [versioning, support, and breaking change policies for Microsoft Graph](versioning-and-support.md).</span></span>

