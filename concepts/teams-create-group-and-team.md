---
title: 使用 Microsoft Graph 创建团队和管理成员
description: '创建包含团队的组涉及以下步骤： '
author: hachandr
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6befb6c6df047c7802e142843180b390f854f6ec
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934834"
---
# <a name="creating-teams-and-managing-members-using-microsoft-graph"></a><span data-ttu-id="370b8-103">使用 Microsoft Graph 创建团队和管理成员</span><span class="sxs-lookup"><span data-stu-id="370b8-103">Creating teams and managing members using Microsoft Graph</span></span>

<span data-ttu-id="370b8-104">可使用 Microsoft Graph 中的 Microsoft Teams API 以多种方式创建团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-104">You can use the Microsoft Teams API in Microsoft Graph to create teams in multiple ways.</span></span> <span data-ttu-id="370b8-105">本文介绍了为获得最佳效果而推荐的方法。</span><span class="sxs-lookup"><span data-stu-id="370b8-105">This article describes the approach that we recommend for the best results.</span></span>


## <a name="initial-team-creation"></a><span data-ttu-id="370b8-106">初始团队创建</span><span class="sxs-lookup"><span data-stu-id="370b8-106">Initial team creation</span></span>

<span data-ttu-id="370b8-107">所有团队都由 Office 365 组提供支持。</span><span class="sxs-lookup"><span data-stu-id="370b8-107">All teams are backed by Office 365 groups.</span></span> <span data-ttu-id="370b8-108">在通过 Microsoft Graph 创建新团队时，建立并运营团队的最快方法是设置新的 Office 365 组、所有者和成员，然后将其转换为团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-108">The quickest way to get your team up and running when you create new teams via Microsoft Graph is to set up a new Office 365 group, all owners and members, and convert that into a team.</span></span>

1. <span data-ttu-id="370b8-109">使用“[创建组](/graph/api/group-post-groups?view=graph-rest-1.0)”操作来创建 [Office 365 组](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)。</span><span class="sxs-lookup"><span data-stu-id="370b8-109">Create an [Office 365 group](https://support.office.com/article/learn-about-office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2) using the [create group](/graph/api/group-post-groups?view=graph-rest-1.0) operation.</span></span> <span data-ttu-id="370b8-110">你可以指定所有者和成员。</span><span class="sxs-lookup"><span data-stu-id="370b8-110">You can specify owners and members.</span></span> <span data-ttu-id="370b8-111">确保新创建的组拥有正确的所有者，如步骤 2 所述。</span><span class="sxs-lookup"><span data-stu-id="370b8-111">Make sure that you have the right owners for the newly created group, as described in Step 2.</span></span>

    <span data-ttu-id="370b8-112">为了为此组创建团队，需要设置以下属性值，如下所示：</span><span class="sxs-lookup"><span data-stu-id="370b8-112">In order to create a team for this group, you need to set the following property values, as shown:</span></span>

    - <span data-ttu-id="370b8-113">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="370b8-113">**groupTypes** = { "Unified" }</span></span> 
    - <span data-ttu-id="370b8-114">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="370b8-114">**mailEnabled** = true</span></span>
    - <span data-ttu-id="370b8-115">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="370b8-115">**securityEnabled** = false</span></span>

    ```http
    POST /groups
    {
        "displayName":"Flight 157",
        "mailNickname":"flight157",
        "description":"Everything about flight 157",
        "visibility":"Private",
        "groupTypes":["Unified"],
        "mailEnabled":true,
        "securityEnabled":false,
        "members@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
            "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
        ],
        "owners@odata.bind":[
            "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
            "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
        ]
    }
    ```

    <span data-ttu-id="370b8-116">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="370b8-116">The following example shows the response.</span></span> 

    ><span data-ttu-id="370b8-117">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="370b8-117">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="370b8-118">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="370b8-118">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Content-length: xxx
    {
        "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
        "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
    }
    ```

2. <span data-ttu-id="370b8-119">确保组有两个或多个所有者。</span><span class="sxs-lookup"><span data-stu-id="370b8-119">Ensure the group has two or more owners.</span></span> <span data-ttu-id="370b8-120">可通过“[添加所有者](/graph/api/group-post-owners?view=graph-rest-1.0)”操作来实现这一点。</span><span class="sxs-lookup"><span data-stu-id="370b8-120">You can do so via the [add owner](/graph/api/group-post-owners?view=graph-rest-1.0) operation.</span></span> <span data-ttu-id="370b8-121">这些应为真实的用户帐户，而不是服务帐户。</span><span class="sxs-lookup"><span data-stu-id="370b8-121">These should be real user accounts and not service accounts.</span></span> <span data-ttu-id="370b8-122">拥有两个所有者有助于处理以下情况：一个所有者离开公司或无法执行团队管理操作。</span><span class="sxs-lookup"><span data-stu-id="370b8-122">Having two owners helps handle cases where one owner leaves the company or is unavailable to perform team management operations.</span></span>

3. <span data-ttu-id="370b8-123">使用“[添加成员](/graph/api/group-post-members?view=graph-rest-1.0)”操作将所有成员（以及来宾，如有必要）添加到组中（如果在步骤 1 中未执行此操作）。</span><span class="sxs-lookup"><span data-stu-id="370b8-123">Add all members (and guests if necessary) to the group using the [add member](/graph/api/group-post-members?view=graph-rest-1.0) operation, if you did not do so in Step 1.</span></span> <span data-ttu-id="370b8-124">若要添加多个成员，请在每个添加操作后添加 1 秒延迟。</span><span class="sxs-lookup"><span data-stu-id="370b8-124">If you're adding multiple members, add a 1 second delay after each add operation.</span></span> 

4. <span data-ttu-id="370b8-125">成功创建组（完成步骤 1 后最长需要 15 分钟）后，使用“[从组创建团队](/graph/api/team-post?view=graph-rest-beta#example-4-create-a-team-from-group)”操作来创建 Microsoft Teams 团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-125">After the group is successfully created, which can take up to 15 minutes after completing Step 1, create a Microsoft Teams team using the [create team from group](/graph/api/team-post?view=graph-rest-beta#example-4-create-a-team-from-group) operation.</span></span> <span data-ttu-id="370b8-126">如果遇到错误，则可能无法完成组创建过程；请尝试稍等几分钟。</span><span class="sxs-lookup"><span data-stu-id="370b8-126">If you run into an error, the group creation process might not be completed; try waiting a few more minutes.</span></span> 

    ```http
    POST https://graph.microsoft.com/beta/teams
    Content-Type: application/json
    {
      "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
      "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
    }
    ```

    <span data-ttu-id="370b8-127">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="370b8-127">The following example shows the response.</span></span> 

    ><span data-ttu-id="370b8-128">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="370b8-128">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="370b8-129">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="370b8-129">All the properties will be returned from an actual call.</span></span>

    ```http
    HTTP/1.1 202 Accepted
    Content-Type: application/json
    Location: /teams/{teamId}/operations/{operationId}
    Content-Location: /teams/{teamId}
    {
    }
    ```

    <span data-ttu-id="370b8-130">已创建团队的 ID 与组相同。</span><span class="sxs-lookup"><span data-stu-id="370b8-130">The created team has the same ID as the group.</span></span>

5. <span data-ttu-id="370b8-131">完成此过程后，所有的所有者和成员都应能够在其 Teams 客户端中查看新创建的团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-131">After this process finishes, all owners and members should be able to see the newly created team in their Teams client.</span></span>

## <a name="adding-or-managing-members"></a><span data-ttu-id="370b8-132">添加或管理成员</span><span class="sxs-lookup"><span data-stu-id="370b8-132">Adding or managing members</span></span>

<span data-ttu-id="370b8-133">若要在创建团队后添加成员，请使用“[添加成员](/graph/api/group-post-members?view=graph-rest-1.0)”操作。</span><span class="sxs-lookup"><span data-stu-id="370b8-133">To add members after a team is created, you use the [add member](/graph/api/group-post-members?view=graph-rest-1.0) operation.</span></span> <span data-ttu-id="370b8-134">建议在添加操作之间添加 1 秒延迟。</span><span class="sxs-lookup"><span data-stu-id="370b8-134">We recommend adding a 1 second delay between add operations.</span></span> <span data-ttu-id="370b8-135">请注意以下与成员身份更改有关的事项：</span><span class="sxs-lookup"><span data-stu-id="370b8-135">Note the following with respect to membership changes:</span></span>

1. <span data-ttu-id="370b8-136">对 Office 365 组进行的成员身份更改通过后台同步机制同步到 Teams，此过程通常需要 24 小时（在某些情况下需要更长时间）。</span><span class="sxs-lookup"><span data-stu-id="370b8-136">Membership changes made to Office 365 groups sync to Teams via a background sync mechanism that typically takes 24 hours (or more in some cases).</span></span>

2. <span data-ttu-id="370b8-137">仅当团队中的一个或多个用户（所有者或成员）在 Teams 桌面客户端中处于活动状态时，才会触发后台进程。</span><span class="sxs-lookup"><span data-stu-id="370b8-137">The background process is triggered only if one or more users in the team (owner or member) is active in the Teams desktop client.</span></span> <span data-ttu-id="370b8-138">启动 Teams 应用程序和/或使其运行即构成活动 — 用户无需访问专门修改的团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-138">Launching the Teams application and/or having it running constitutes activity — a user does not need to visit the team that is being modified specifically.</span></span>

    ><span data-ttu-id="370b8-139">**注意：** Teams 移动客户端不会触发成员身份同步。应至少有一个用户位于桌面客户端上，以确保此后台进程顺利运行。</span><span class="sxs-lookup"><span data-stu-id="370b8-139">**Note:** The Teams mobile clients do not trigger the membership sync. At least one user should be on the desktop client to that ensure this background process goes smoothly.</span></span>

## <a name="checklist-for-validation"></a><span data-ttu-id="370b8-140">验证清单</span><span class="sxs-lookup"><span data-stu-id="370b8-140">Checklist for validation</span></span>

<span data-ttu-id="370b8-141">创建团队后，可使用以下清单验证是否已成功创建该团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-141">After you create a team, you can use the following checklist to verify that the team was created successfully.</span></span>

### <a name="validate-team-creation"></a><span data-ttu-id="370b8-142">验证团队创建</span><span class="sxs-lookup"><span data-stu-id="370b8-142">Validate team creation</span></span>

1. <span data-ttu-id="370b8-143">验证为团队提供支持的 Office 365 组是通过 Azure AD 还是 Microsoft 365 管理中心创建的。</span><span class="sxs-lookup"><span data-stu-id="370b8-143">Verify that the Office 365 group backing the team is created via the Azure AD or Microsoft 365 admin centers.</span></span>

2. <span data-ttu-id="370b8-144">通过 Teams 管理门户验证团队创建是否成功。</span><span class="sxs-lookup"><span data-stu-id="370b8-144">Verify that the team creation succeeded via the Teams admin portal.</span></span>

3. <span data-ttu-id="370b8-145">验证团队是否拥有通过 Teams 管理门户列出的正确所有者和成员。</span><span class="sxs-lookup"><span data-stu-id="370b8-145">Verify that the team has the correct owners and members listed via the Teams admin portal.</span></span>

4. <span data-ttu-id="370b8-146">验证团队所有者登录 Teams 桌面或 Web 客户端后是否可以看到该团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-146">Verify that the team owners can see the team after signing into the Teams desktop or web client.</span></span>

5. <span data-ttu-id="370b8-147">验证成员登录 Teams 桌面或 Web 客户端后是否可以看到该团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-147">Verify that members can see the team after signing into the Teams desktop or web client.</span></span>

### <a name="validate-addition-of-members"></a><span data-ttu-id="370b8-148">验证成员的添加</span><span class="sxs-lookup"><span data-stu-id="370b8-148">Validate addition of members</span></span>

1. <span data-ttu-id="370b8-149">验证新成员是否通过 Azure AD 或 Microsoft 365 管理中心显示在组中。</span><span class="sxs-lookup"><span data-stu-id="370b8-149">Verify that newly members show up in the group via the Azure AD or Microsoft 365 admin center.</span></span>

2. <span data-ttu-id="370b8-150">验证新添加的成员登录 Teams 桌面或 Web 客户端后是否可以看到该团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-150">Verify that newly added members can see the team after signing into the Teams desktop or web client.</span></span>



## <a name="how-office-365-group-membership-changes-are-synchronized-to-microsoft-teams"></a><span data-ttu-id="370b8-151">Office 365 组成员身份更改如何同步到 Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="370b8-151">How Office 365 group membership changes are synchronized to Microsoft Teams</span></span>

<span data-ttu-id="370b8-152">通过 Microsoft Graph API 或管理门户（Teams 客户端外部）对支持团队的 Office 365 组所做的成员身份更改必须同步到 Teams 服务，以便新添加的用户能够查看并加入该团队。</span><span class="sxs-lookup"><span data-stu-id="370b8-152">Membership changes made to an Office 365 group backing a team via the Microsoft Graph API or through the admin portal (outside of the Teams client) have to sync to the Teams service in order for newly added users to be able to see and participate in the team.</span></span> <span data-ttu-id="370b8-153">直接对组成员身份所做的更改将通过后台进程同步到 Teams 服务。</span><span class="sxs-lookup"><span data-stu-id="370b8-153">Changes made directly to the group membership are synchronized to the Teams service via a background process.</span></span> <span data-ttu-id="370b8-154">此后台进程在 Teams 服务中运行，并由 Teams 桌面和 Web 客户端中的用户活动触发。</span><span class="sxs-lookup"><span data-stu-id="370b8-154">This background process runs in the Teams service and is triggered by user activity in Teams desktop and web clients.</span></span>

<span data-ttu-id="370b8-155">为了触发此进程，此团队的当前所有者或成员（可在 Teams 客户端中看到该团队的人员）必须打开 Teams 桌面（理想情况下）或 Web 客户端。</span><span class="sxs-lookup"><span data-stu-id="370b8-155">For the process to get triggered, a current owner or member of that team (someone who can see the team in the Teams client) must have the Teams desktop (ideally) or web client open.</span></span> <span data-ttu-id="370b8-156">移动客户端不会触发此同步。</span><span class="sxs-lookup"><span data-stu-id="370b8-156">Mobile clients do not trigger this sync.</span></span>

<span data-ttu-id="370b8-157">当客户端活动触发同步后，用于同步对组所做的成员身份更改的当前 SLA 最长为 24 小时。</span><span class="sxs-lookup"><span data-stu-id="370b8-157">The current SLA for synchronizing membership changes made to groups to Teams is up to 24 hours after the sync is triggered by client activity.</span></span> <span data-ttu-id="370b8-158">在某些情况下，可能会花费更长的时间（例如，由服务负载所致）。</span><span class="sxs-lookup"><span data-stu-id="370b8-158">It can take longer under certain circumstances (due to service load, for example).</span></span>


![名单同步流程。](images/teams-roster-sync.png)

