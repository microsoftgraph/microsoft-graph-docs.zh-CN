---
title: Microsoft Graph 中的 Microsoft 365 组概述
description: 'Microsoft 365 组为用户提供了用于共享对话、文件、便笺、日历、计划和许多其他资产的基础成员身份服务。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0ea28b5f4ff69faba5146ebc790703e423d9e8ba
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896110"
---
# <a name="overview-of-microsoft-365-groups-in-microsoft-graph"></a><span data-ttu-id="77cf7-103">Microsoft Graph 中的 Microsoft 365 组概述</span><span class="sxs-lookup"><span data-stu-id="77cf7-103">Overview of Microsoft 365 groups in Microsoft Graph</span></span>

<span data-ttu-id="77cf7-104">Microsoft 365 组为用户提供了用于共享对话、文件、便笺、日历、计划和许多其他资产的基础成员身份服务。</span><span class="sxs-lookup"><span data-stu-id="77cf7-104">Microsoft 365 groups provide the foundational membership service for users to share conversations, files, notes, calendars, plans, and many other assets.</span></span> 


> [!VIDEO https://www.youtube-nocookie.com/embed/WB9w6QM9xIU]

## <a name="why-integrate-with-microsoft-365-groups"></a><span data-ttu-id="77cf7-105">为什么要与 Microsoft 365 组集成？</span><span class="sxs-lookup"><span data-stu-id="77cf7-105">Why integrate with Microsoft 365 groups?</span></span>   

<span data-ttu-id="77cf7-106">各个组会形成一个基础，让用户能够跨服务进行协作和集成，以支持任务计划、团队合作、教育等丰富的应用场景。</span><span class="sxs-lookup"><span data-stu-id="77cf7-106">Groups form the foundation that enables user collaboration and integration across services to support rich scenarios in task planning, teamwork, education, and more.</span></span> <span data-ttu-id="77cf7-107">当您与 Microsoft 365 组集成时，您的应用程序可以支持数百万个用户在 Microsoft 365 套件中的不同体验之间过渡。</span><span class="sxs-lookup"><span data-stu-id="77cf7-107">When you integrate with Microsoft 365 groups, your application can support millions of users as they transition across various experiences in the Microsoft 365 suite and beyond.</span></span>  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a><span data-ttu-id="77cf7-108">创建组以促进跨服务的团队合作</span><span class="sxs-lookup"><span data-stu-id="77cf7-108">Create groups to facilitate teamwork across services</span></span> 
 
<span data-ttu-id="77cf7-109">你可以使用 Microsoft Graph API 在整个协作生命周期中创建、管理或删除组。</span><span class="sxs-lookup"><span data-stu-id="77cf7-109">You can use the Microsoft Graph API to create, manage, or delete groups throughout the lifecycle of collaboration.</span></span> <span data-ttu-id="77cf7-110">例如，可以执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="77cf7-110">For example, you can do the following:</span></span>  
 
- <span data-ttu-id="77cf7-111">使用[创建组](/graph/api/group-post-groups?view=graph-rest-1.0) API 预配一个新组。</span><span class="sxs-lookup"><span data-stu-id="77cf7-111">Use the [Create group](/graph/api/group-post-groups?view=graph-rest-1.0) API to provision a new group.</span></span> <span data-ttu-id="77cf7-112">然后，该组可用于一系列应用程序，例如 Outlook、SharePoint、Microsoft Teams、Planner，甚至 Microsoft Stream。</span><span class="sxs-lookup"><span data-stu-id="77cf7-112">The group is then made available in a range of applications, such as Outlook, SharePoint, Microsoft Teams, Planner, and even Microsoft Stream.</span></span> <span data-ttu-id="77cf7-113">Microsoft Graph 可跨这些连接的服务进行同步，以对所有组成员无缝提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="77cf7-113">Microsoft Graph synchronizes across these connected services to seamlessly provide access to all group members.</span></span>  
 
    <span data-ttu-id="77cf7-114">**每个 Microsoft 365 组都与一组默认的 Microsoft 365 服务集成**</span><span class="sxs-lookup"><span data-stu-id="77cf7-114">**Every Microsoft 365 group is integrated with a default set of Microsoft 365 services**</span></span>

    ![显示 Microsoft 365 组与文件、备注、任务、网站、对话和日历集成的图示](images/office365-groups-concept-overview-related-services-infographic.png)  

- <span data-ttu-id="77cf7-116">允许成员指示某个组是他们的[收藏夹](/graph/api/group-addfavorite?view=graph-rest-1.0)之一，或者在他们选择时[将其从收藏夹中删除](/graph/api/group-removefavorite?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-116">Enable members to indicate that a group is one of their [favorites](/graph/api/group-addfavorite?view=graph-rest-1.0), or [remove it from their favorites](/graph/api/group-removefavorite?view=graph-rest-1.0) if they choose.</span></span> 
- <span data-ttu-id="77cf7-117">从自定义应用程序中[创建](/graph/api/group-post-conversations?view=graph-rest-1.0)、[获取](/graph/api/group-get-conversation?view=graph-rest-1.0)或[删除](/graph/api/group-delete-conversation?view=graph-rest-1.0)组对话。</span><span class="sxs-lookup"><span data-stu-id="77cf7-117">[Create](/graph/api/group-post-conversations?view=graph-rest-1.0), [get](/graph/api/group-get-conversation?view=graph-rest-1.0), or [delete](/graph/api/group-delete-conversation?view=graph-rest-1.0) group conversations from your custom application.</span></span> 
- <span data-ttu-id="77cf7-118">在组日历上计划日历[事件](/graph/api/resources/event?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-118">Schedule calendar [events](/graph/api/resources/event?view=graph-rest-1.0) on the group calendar.</span></span> 
- <span data-ttu-id="77cf7-119">获取与组关联的 [SharePoint 网站](/graph/api/resources/site?view=graph-rest-1.0)的相关信息，如文档库[列表](/graph/api/list-list?view=graph-rest-1.0)或[子网站](/graph/api/site-list-subsites?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-119">Get information about the [SharePoint site](/graph/api/resources/site?view=graph-rest-1.0) that's associated with a group, such as the document library [lists](/graph/api/list-list?view=graph-rest-1.0) or [subsites](/graph/api/site-list-subsites?view=graph-rest-1.0).</span></span> 
- <span data-ttu-id="77cf7-120">在 Planner 中[创建一个属于组的计划](/graph/api/planner-post-buckets?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-120">[Create a plan](/graph/api/planner-post-buckets?view=graph-rest-1.0) in Planner that is owned by a group.</span></span> <span data-ttu-id="77cf7-121">该计划通过允许[创建任务](/graph/api/planner-post-tasks?view=graph-rest-1.0)（可以[跨存储桶进行组织](/graph/api/planner-post-buckets?view=graph-rest-1.0)），提供了一种直观的方式来跟踪团队合作。</span><span class="sxs-lookup"><span data-stu-id="77cf7-121">The plan provides a visual way to track teamwork by allowing you to [create tasks](/graph/api/planner-post-tasks?view=graph-rest-1.0) that can be [organized across buckets](/graph/api/planner-post-buckets?view=graph-rest-1.0).</span></span> 
- <span data-ttu-id="77cf7-122">访问与组关联的 [OneNote](/graph/api/resources/onenote?view=graph-rest-1.0) 笔记本，这可用于收集会议记录和整理想法。</span><span class="sxs-lookup"><span data-stu-id="77cf7-122">Access the [OneNote](/graph/api/resources/onenote?view=graph-rest-1.0) notebook associated with a group, which can be used for collecting meeting notes and organizing ideas.</span></span> 
  
    <span data-ttu-id="77cf7-123">**Outlook 网页中的 Microsoft 365 组和对话**</span><span class="sxs-lookup"><span data-stu-id="77cf7-123">**Microsoft 365 groups and conversations in Outlook in the web**</span></span>

    ![Outlook 网页版在“组”文件夹中列出组的屏幕截图](images/office365-groups-concept-overview-groups-in-outlook.png) 

- <span data-ttu-id="77cf7-125">[为 Microsoft Teams 启用组](/graph/api/team-put-teams?view=graph-rest-beta)（预览版），以允许组成员参与持久聊天。</span><span class="sxs-lookup"><span data-stu-id="77cf7-125">[Enable a group for Microsoft Teams](/graph/api/team-put-teams?view=graph-rest-beta) (preview) to allow group members to engage in persistent chat.</span></span>  
- <span data-ttu-id="77cf7-126">[删除组](/graph/api/group-delete?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-126">[Delete groups](/graph/api/group-delete?view=graph-rest-1.0).</span></span> <span data-ttu-id="77cf7-127">删除组时，所有关联的内容也会一并删除，从而防止孤立的站点、对话或计划。</span><span class="sxs-lookup"><span data-stu-id="77cf7-127">When a group is deleted, all associated content is also deleted, which prevents orphaned sites, conversations, or plans.</span></span> 
 
### <a name="manage-group-membership-seamlessly"></a><span data-ttu-id="77cf7-128">无缝管理组成员身份</span><span class="sxs-lookup"><span data-stu-id="77cf7-128">Manage group membership seamlessly</span></span> 
 
<span data-ttu-id="77cf7-129">Microsoft 365 组是共享 Microsoft 服务或应用程序中资源的访问权限的用户集合。</span><span class="sxs-lookup"><span data-stu-id="77cf7-129">Microsoft 365 groups are collections of users who share access to resources in Microsoft services or within your app.</span></span> <span data-ttu-id="77cf7-130">由于组成员身份是集中管理的，因此，对成员身份的任何更改都会影响与该组关联的所有服务。</span><span class="sxs-lookup"><span data-stu-id="77cf7-130">Because group membership is managed centrally, any changes to membership affect all services associated with the group.</span></span> <span data-ttu-id="77cf7-131">你可使用 Microsoft Graph 执行以下组成员身份任务：</span><span class="sxs-lookup"><span data-stu-id="77cf7-131">You can use Microsoft Graph to perform the following group membership tasks:</span></span>
 
- <span data-ttu-id="77cf7-132">从现有组中[添加](/graph/api/group-post-members?view=graph-rest-1.0)和[删除](/graph/api/group-delete-members?view=graph-rest-1.0)成员。</span><span class="sxs-lookup"><span data-stu-id="77cf7-132">[Add](/graph/api/group-post-members?view=graph-rest-1.0) and [remove](/graph/api/group-delete-members?view=graph-rest-1.0) members from an existing group.</span></span> 
- <span data-ttu-id="77cf7-133">获取组的[所有者列表](/graph/api/group-list-owners?view=graph-rest-1.0)或[成员列表](/graph/api/group-list-members?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-133">Get a [list of owners](/graph/api/group-list-owners?view=graph-rest-1.0) or a [list of members](/graph/api/group-list-members?view=graph-rest-1.0) for a group.</span></span> <span data-ttu-id="77cf7-134">这有助于传达哪些人员可以访问组内容，或者哪些人员可能需要执行管理职责，如续订组或批准加入请求。</span><span class="sxs-lookup"><span data-stu-id="77cf7-134">This helps communicate who has access to group content, or who might need to perform administrative duties, such as renewing the group or approving a join request.</span></span> 
- <span data-ttu-id="77cf7-135">通过[更新组](/graph/api/group-update?view=graph-rest-1.0)操作，可将组指定为**公开**（其中组内容对同一组织中的任何人都可见），或者**私人**（其中组内容仅对成员可见）。</span><span class="sxs-lookup"><span data-stu-id="77cf7-135">Designate groups as **Public**, where group content is visible to anyone in the same organization, or **Private**, where group content is only visible to members, via the [update group](/graph/api/group-update?view=graph-rest-1.0) operation.</span></span> 
- <span data-ttu-id="77cf7-136">从组所有者列表中[删除不再参与特定组所有权职责的所有者](/graph/api/group-delete-owners?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-136">[Remove owners](/graph/api/group-delete-owners?view=graph-rest-1.0) who are no longer participating in the ownership responsibilities for a particular group from the list of group owners.</span></span> 
 
### <a name="establish-and-maintain-group-policy-settings"></a><span data-ttu-id="77cf7-137">建立和维护组策略设置</span><span class="sxs-lookup"><span data-stu-id="77cf7-137">Establish and maintain group policy settings</span></span> 
 
<span data-ttu-id="77cf7-138">随着组织内创建的组数量开始增长，Microsoft Graph 支持管理组的使用情况和生命周期的能力。</span><span class="sxs-lookup"><span data-stu-id="77cf7-138">As the number of groups created within an organization begins to grow, Microsoft Graph supports the ability to govern the usage and lifecycle of the group.</span></span> <span data-ttu-id="77cf7-139">你可以跨组织中的所有组强制执行组策略。</span><span class="sxs-lookup"><span data-stu-id="77cf7-139">You can enforce group policies across all groups within an organization.</span></span> <span data-ttu-id="77cf7-140">可以使用 Microsoft Graph API 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="77cf7-140">You can use the Microsoft Graph API to:</span></span>

- <span data-ttu-id="77cf7-141">配置广泛的[组策略设置](/graph/api/resources/groupsetting?view=graph-rest-1.0)，以帮助定义行为，例如，自动删除组，除非它们由所有者续订并强制实施 Microsoft 365 组上的命名策略。</span><span class="sxs-lookup"><span data-stu-id="77cf7-141">Configure a broad range of [group policy settings](/graph/api/resources/groupsetting?view=graph-rest-1.0) that help define behaviors, such as automatically deleting groups unless they are renewed by an owner and enforcing naming policies on Microsoft 365 groups.</span></span> 
- <span data-ttu-id="77cf7-142">[续订](/graph/api/group-renew?view=graph-rest-1.0)即将到期的组，以让团队成员继续协作和访问内容。</span><span class="sxs-lookup"><span data-stu-id="77cf7-142">[Renew](/graph/api/group-renew?view=graph-rest-1.0) groups that are about to expire to allow team members to continue with collaboration and accessing content.</span></span> <span data-ttu-id="77cf7-143">如果未根据已建立的过期策略续订组，则会自动删除该组。</span><span class="sxs-lookup"><span data-stu-id="77cf7-143">If the group is not renewed according to the established expiration policy, the group is automatically deleted.</span></span> 
- <span data-ttu-id="77cf7-144">[还原](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0)已删除组。</span><span class="sxs-lookup"><span data-stu-id="77cf7-144">[Restore](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) deleted groups.</span></span>

## <a name="api-reference"></a><span data-ttu-id="77cf7-145">API 参考</span><span class="sxs-lookup"><span data-stu-id="77cf7-145">API reference</span></span>
<span data-ttu-id="77cf7-146">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="77cf7-146">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="77cf7-147">Microsoft Graph v1.0 中的组 API</span><span class="sxs-lookup"><span data-stu-id="77cf7-147">Groups API in Microsoft Graph v1.0</span></span>](/graph/api/resources/groups-overview?view=graph-rest-1.0)
- [<span data-ttu-id="77cf7-148">Microsoft Graph beta 中的组 API</span><span class="sxs-lookup"><span data-stu-id="77cf7-148">Groups API in Microsoft Graph beta</span></span>](/graph/api/resources/groups-overview?view=graph-rest-beta)


## <a name="next-steps"></a><span data-ttu-id="77cf7-149">后续步骤</span><span class="sxs-lookup"><span data-stu-id="77cf7-149">Next steps</span></span>

- <span data-ttu-id="77cf7-150">在 [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) 中尝试一些示例 API 请求。</span><span class="sxs-lookup"><span data-stu-id="77cf7-150">Try out some sample API requests in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> 
- <span data-ttu-id="77cf7-151">详细了解如何在 Microsoft Graph 中[使用组 API](/graph/api/resources/groups-overview?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="77cf7-151">Learn more about how to [use the groups API](/graph/api/resources/groups-overview?view=graph-rest-1.0) in Microsoft Graph.</span></span>
