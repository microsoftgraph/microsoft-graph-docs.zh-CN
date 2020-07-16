---
title: Microsoft Graph REST API 1.0 版参考
description: 欢迎使用 1.0 版终结点的 Microsoft Graph REST API 参考。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: non-product-specific
doc_type: conceptualPageType
ms.openlocfilehash: 75672eedd4b1693b31058de6531c470db548a033
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897930"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a><span data-ttu-id="aeded-103">Microsoft Graph REST API 1.0 版参考</span><span class="sxs-lookup"><span data-stu-id="aeded-103">Microsoft Graph REST API v1.0 reference</span></span>

<span data-ttu-id="aeded-104">欢迎使用 1.0 版终结点的 Microsoft Graph REST API 参考。</span><span class="sxs-lookup"><span data-stu-id="aeded-104">Welcome to Microsoft Graph REST API reference for the v1.0 endpoint.</span></span>

<span data-ttu-id="aeded-105">1.0 版终结点 (`https://graph.microsoft.com/v1.0`) 上的 API 集处于一般可用 (GA) 状态，并经过与客户进行严格的审查和反馈流程，以满足实际的生产需求。</span><span class="sxs-lookup"><span data-stu-id="aeded-105">API sets on the v1.0 endpoint (`https://graph.microsoft.com/v1.0`) are in general availability (GA) status, and have gone through a rigorous review-and-feedback process with customers to meet practical, production needs.</span></span> <span data-ttu-id="aeded-106">此终结点上的 API 更新本质上可以累加，并且不会破坏现有应用场景。</span><span class="sxs-lookup"><span data-stu-id="aeded-106">Updates to APIs on this endpoint are additive in nature and do not break existing app scenarios.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="aeded-107">常见用例</span><span class="sxs-lookup"><span data-stu-id="aeded-107">Common use cases</span></span>

<span data-ttu-id="aeded-108">Microsoft Graph 的强大之处在于可以在单个 Microsoft Graph REST 终结点公开的不同服务之间轻松导航实体和关系。</span><span class="sxs-lookup"><span data-stu-id="aeded-108">The power of Microsoft Graph lies in easy navigation of entities and relationships across different services exposed on a single Microsoft Graph REST endpoint.</span></span>

<span data-ttu-id="aeded-109">很多服务旨在围绕[用户](./resources/user.md)和[组](./resources/group.md)实现丰富的应用场景。</span><span class="sxs-lookup"><span data-stu-id="aeded-109">A number of these services are designed to enable rich scenarios around a [user](./resources/user.md) and around a [group](./resources/group.md).</span></span>

### <a name="user-centric-use-cases-in-v10"></a><span data-ttu-id="aeded-110">1.0 版中以用户为中心的用例</span><span class="sxs-lookup"><span data-stu-id="aeded-110">User-centric use cases in v1.0</span></span>

1. <span data-ttu-id="aeded-111">获取用户 Lisa 的[个人资料](./api/user-get.md)和[照片](./resources/profilephoto.md)。</span><span class="sxs-lookup"><span data-stu-id="aeded-111">[Get the profile](./api/user-get.md) and [photo](./resources/profilephoto.md) of a user, Lisa.</span></span>
2. <span data-ttu-id="aeded-112">[获取 Lisa 的经理的个人资料信息](./api/user-list-manager.md)和[她的直接下属的 ID](./api/user-list-directreports.md)，全都存储在 Azure Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="aeded-112">[Get the profile information about Lisa's manager](./api/user-list-manager.md) and [IDs of her direct reports](./api/user-list-directreports.md), all stored in Azure Active Directory.</span></span>
3. <span data-ttu-id="aeded-113">[访问 Lisa 在 OneDrive for Business 上的文件](./api/driveitem-list-children.md)，查找最后修改[文件](./resources/driveitem.md)的人员的[身份](./resources/identityset.md)，并导航到此人的个人资料。</span><span class="sxs-lookup"><span data-stu-id="aeded-113">[Access Lisa's files on OneDrive for Business](./api/driveitem-list-children.md), find the [identity](./resources/identityset.md) of the last person who modified a [file](./resources/driveitem.md) there, and navigate to that person's profile.</span></span>
4. <span data-ttu-id="aeded-114">在 Exchange Online 中[访问 Lisa 的日历](./api/calendar-get.md)，并[确定 Lisa 与团队成员在接下来的两周内会面的最佳时间](./api/user-findmeetingtimes.md)。</span><span class="sxs-lookup"><span data-stu-id="aeded-114">[Access Lisa's calendar](./api/calendar-get.md) on Exchange Online and [determine the best time for Lisa to meet with her team](./api/user-findmeetingtimes.md) in the next two weeks.</span></span>
5. <span data-ttu-id="aeded-115">在 Lisa 的日历中[订阅](./api/subscription-post-subscriptions.md)并[跟踪更改](./api/event-delta.md)，当她花费在会议上的时间超过 80% 时通知她。</span><span class="sxs-lookup"><span data-stu-id="aeded-115">[Subscribe to](./api/subscription-post-subscriptions.md) and [track changes](./api/event-delta.md) in Lisa's calendar, tell Lisa when she is spending more than 80% of her time in meetings.</span></span>
6. <span data-ttu-id="aeded-116">设置当 Lisa 不在办公室时的[自动答复](./api/user-update-mailboxsettings.md#example-1)。</span><span class="sxs-lookup"><span data-stu-id="aeded-116">[Set automatic replies](./api/user-update-mailboxsettings.md#example-1) when Lisa is away from the office.</span></span>
7. <span data-ttu-id="aeded-117">根据通信、协作和业务关系，[获取与 Lisa 最相关的人员](./api/user-list-people.md)。</span><span class="sxs-lookup"><span data-stu-id="aeded-117">[Get the people who are most relevant to Lisa](./api/user-list-people.md), based on communication, collaboration, and business relationships.</span></span>
8. <span data-ttu-id="aeded-118">在 Lisa 的 OneDrive for Business 的 Excel 文件中，从一个[图表](./resources/chart.md)获取最新销售预测。</span><span class="sxs-lookup"><span data-stu-id="aeded-118">Get the latest sales projection from a [chart](./resources/chart.md) in an Excel file in Lisa's OneDrive for Business.</span></span>
9. <span data-ttu-id="aeded-119">[在 Planner 中查找分配给 Lisa 的任务](./api/planneruser-list-tasks.md)。</span><span class="sxs-lookup"><span data-stu-id="aeded-119">[Find the tasks assigned to Lisa in Planner](./api/planneruser-list-tasks.md).</span></span>

### <a name="microsoft-365-group-use-cases-in-v10"></a><span data-ttu-id="aeded-120">1.0 版中的 Microsoft 365 组用例</span><span class="sxs-lookup"><span data-stu-id="aeded-120">Microsoft 365 group use cases in v1.0</span></span>

1. <span data-ttu-id="aeded-121">对组织中的 Microsoft 365 组运行报告，并确定[组成员之间通讯](./api/reportroot-getoffice365groupsactivitycounts.md)最多的组。</span><span class="sxs-lookup"><span data-stu-id="aeded-121">Run a report on Microsoft 365 groups in an organization and identify the group with the most [communication among group members](./api/reportroot-getoffice365groupsactivitycounts.md).</span></span>
2. <span data-ttu-id="aeded-122">[查找此 Microsoft 365 组的计划](./api/plannergroup-list-plans.md)，并在该计划中[分配任务](./resources/plannerassignments.md)。</span><span class="sxs-lookup"><span data-stu-id="aeded-122">[Find the plans of this Microsoft 365 group](./api/plannergroup-list-plans.md), and the [assignment of tasks](./resources/plannerassignments.md) in that plan.</span></span>
3. <span data-ttu-id="aeded-123">在 Microsoft 365 组中[启动一个新对话](./api/group-post-conversations.md)，以确定成员是否要[创建另一个组](./api/group-post-groups.md)来共享工作负荷。</span><span class="sxs-lookup"><span data-stu-id="aeded-123">[Start a new conversation](./api/group-post-conversations.md) in the Microsoft 365 group to determine if members want to [create another group](./api/group-post-groups.md) to share the workload.</span></span>
4. <span data-ttu-id="aeded-124">为组[获取默认笔记本](./api/notebook-get.md)并[创建一个页面](./api/section-post-pages.md)注明调查结果。</span><span class="sxs-lookup"><span data-stu-id="aeded-124">[Get the default notebook](./api/notebook-get.md) for the group and [create a page](./api/section-post-pages.md) to note the outcome of the investigation.</span></span>

## <a name="other-api-versions"></a><span data-ttu-id="aeded-125">其他 API 版本</span><span class="sxs-lookup"><span data-stu-id="aeded-125">Other API versions</span></span>

<span data-ttu-id="aeded-126">目前有两个版本的 Microsoft Graph REST API：1.0 版 和 beta 版。</span><span class="sxs-lookup"><span data-stu-id="aeded-126">There are currently 2 versions of Microsoft Graph REST APIs - v1.0 and beta.</span></span>
<span data-ttu-id="aeded-127">如需了解仍处于预览状态的新 API 或增强 API，请参阅 [Microsoft Graph beta 终结点参考](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="aeded-127">If you're interested in new or enhanced APIs that are still in preview status, see [Microsoft Graph beta endpoint reference](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta).</span></span> <span data-ttu-id="aeded-128">请注意，预览状态的 API 可能会发生更改，并可能在无通知的情况下破坏现有应用场景。</span><span class="sxs-lookup"><span data-stu-id="aeded-128">Be aware that APIs in preview status are subject to change, and may break existing scenarios without notice.</span></span> <span data-ttu-id="aeded-129">不要对 beta 终结点的 API 产生依赖。</span><span class="sxs-lookup"><span data-stu-id="aeded-129">Don't take a production dependency on APIs in the beta endpoint.</span></span>

<span data-ttu-id="aeded-130">请参阅[版本控制和支持](/graph/versioning-and-support)了解更多信息。</span><span class="sxs-lookup"><span data-stu-id="aeded-130">Find more information about [versioning and support](/graph/versioning-and-support).</span></span>

## <a name="call-the-v10-endpoint"></a><span data-ttu-id="aeded-131">调用 v1.0 终结点</span><span class="sxs-lookup"><span data-stu-id="aeded-131">Call the v1.0 endpoint</span></span>

<span data-ttu-id="aeded-132">针对 v1.0 终结点的 Microsoft Graph API 请求使用以下模式：</span><span class="sxs-lookup"><span data-stu-id="aeded-132">Microsoft Graph API requests to the v1.0 endpoint use the following pattern:</span></span>

```
https://graph.microsoft.com/v1.0/{resource}?[query_parameters]
```

<span data-ttu-id="aeded-133">有关详细信息，请参阅[使用 Microsoft Graph API](/graph/use-the-api)。</span><span class="sxs-lookup"><span data-stu-id="aeded-133">For details, see [Use the Microsoft Graph API](/graph/use-the-api).</span></span>

## <a name="whats-new"></a><span data-ttu-id="aeded-134">最近更新</span><span class="sxs-lookup"><span data-stu-id="aeded-134">What's new</span></span>
<span data-ttu-id="aeded-135">了解 v1.0 终结点中的[最新新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="aeded-135">Find out about the [latest new features and updates](/graph/whats-new-overview) in the v1.0 endpoint.</span></span>

## <a name="connect-with-us"></a><span data-ttu-id="aeded-136">与我们联系</span><span class="sxs-lookup"><span data-stu-id="aeded-136">Connect with us</span></span>

<span data-ttu-id="aeded-137">是否希望在 Microsoft Graph 中增加其他 API 或功能？</span><span class="sxs-lookup"><span data-stu-id="aeded-137">Are there additional APIs or features you'd like to see in Microsoft Graph?</span></span> <span data-ttu-id="aeded-138">在 [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632) 上发布新功能请求。</span><span class="sxs-lookup"><span data-stu-id="aeded-138">Post new feature requests on [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).</span></span>

<span data-ttu-id="aeded-139">对现有 Microsoft Graph API 有反馈意见？</span><span class="sxs-lookup"><span data-stu-id="aeded-139">Have feedback for existing Microsoft Graph APIs?</span></span> <span data-ttu-id="aeded-140">在 [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues) 上与我们联系。</span><span class="sxs-lookup"><span data-stu-id="aeded-140">Connect with us on [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).</span></span>
