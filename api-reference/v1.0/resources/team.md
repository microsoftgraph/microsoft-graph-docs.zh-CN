---
title: 团队资源类型
description: 'Microsoft Teams 团队是频道的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7eb01d5043ec6857a6b99b5a0eb3f91687d74bdf
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387728"
---
# <a name="team-resource-type"></a><span data-ttu-id="a18d6-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="a18d6-103">team resource type</span></span>

<span data-ttu-id="a18d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18d6-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a18d6-105">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a18d6-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="a18d6-106">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="a18d6-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="a18d6-107">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="a18d6-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="a18d6-108">该组具有与团队相同的 ID，例如 /groups/{id}/team 与 /teams/{id} 相同。</span><span class="sxs-lookup"><span data-stu-id="a18d6-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="a18d6-109">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a18d6-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a18d6-110">方法</span><span class="sxs-lookup"><span data-stu-id="a18d6-110">Methods</span></span>

| <span data-ttu-id="a18d6-111">方法</span><span class="sxs-lookup"><span data-stu-id="a18d6-111">Method</span></span>       | <span data-ttu-id="a18d6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="a18d6-112">Return Type</span></span>  |<span data-ttu-id="a18d6-113">说明</span><span class="sxs-lookup"><span data-stu-id="a18d6-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a18d6-114">创建团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-114">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="a18d6-115">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="a18d6-115">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="a18d6-116">从头开始创建团队。</span><span class="sxs-lookup"><span data-stu-id="a18d6-116">Create a team from scratch.</span></span> |
|[<span data-ttu-id="a18d6-117">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-117">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="a18d6-118">team</span><span class="sxs-lookup"><span data-stu-id="a18d6-118">team</span></span>](team.md) | <span data-ttu-id="a18d6-119">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="a18d6-119">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="a18d6-120">获取团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-120">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="a18d6-121">team</span><span class="sxs-lookup"><span data-stu-id="a18d6-121">team</span></span>](team.md) | <span data-ttu-id="a18d6-122">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a18d6-122">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="a18d6-123">更新团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-123">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="a18d6-124">team</span><span class="sxs-lookup"><span data-stu-id="a18d6-124">team</span></span>](team.md) |<span data-ttu-id="a18d6-125">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="a18d6-125">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="a18d6-126">删除团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-126">Delete team</span></span>](../api/group-delete.md) | <span data-ttu-id="a18d6-127">无</span><span class="sxs-lookup"><span data-stu-id="a18d6-127">None</span></span> |<span data-ttu-id="a18d6-128">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="a18d6-128">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="a18d6-129">List members</span><span class="sxs-lookup"><span data-stu-id="a18d6-129">List members</span></span>](../api/team-list-members.md)|<span data-ttu-id="a18d6-130">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-130">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="a18d6-131">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="a18d6-131">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="a18d6-132">获取成员</span><span class="sxs-lookup"><span data-stu-id="a18d6-132">Get member</span></span>](../api/team-get-members.md) | <span data-ttu-id="a18d6-133">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a18d6-134">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="a18d6-134">Get a member in the team.</span></span>|
|[<span data-ttu-id="a18d6-135">添加成员</span><span class="sxs-lookup"><span data-stu-id="a18d6-135">Add member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="a18d6-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a18d6-136">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="a18d6-137">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="a18d6-137">Add a new member to the team.</span></span>|
|[<span data-ttu-id="a18d6-138">删除成员</span><span class="sxs-lookup"><span data-stu-id="a18d6-138">Remove member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="a18d6-139">无</span><span class="sxs-lookup"><span data-stu-id="a18d6-139">None</span></span>|<span data-ttu-id="a18d6-140">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="a18d6-140">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="a18d6-141">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="a18d6-141">Update member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="a18d6-142">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a18d6-142">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="a18d6-143">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="a18d6-143">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="a18d6-144">存档团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-144">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="a18d6-145">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="a18d6-145">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="a18d6-146">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="a18d6-146">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="a18d6-147">解档团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-147">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="a18d6-148">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="a18d6-148">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="a18d6-149">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="a18d6-149">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="a18d6-150">克隆团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-150">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="a18d6-151">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="a18d6-151">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="a18d6-152">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="a18d6-152">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="a18d6-153">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-153">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="a18d6-154">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-154">[team](team.md) collection</span></span> | <span data-ttu-id="a18d6-155">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="a18d6-155">List the teams you are a member of.</span></span> |

## <a name="properties"></a><span data-ttu-id="a18d6-156">属性</span><span class="sxs-lookup"><span data-stu-id="a18d6-156">Properties</span></span>

| <span data-ttu-id="a18d6-157">属性</span><span class="sxs-lookup"><span data-stu-id="a18d6-157">Property</span></span> | <span data-ttu-id="a18d6-158">类型</span><span class="sxs-lookup"><span data-stu-id="a18d6-158">Type</span></span> | <span data-ttu-id="a18d6-159">说明</span><span class="sxs-lookup"><span data-stu-id="a18d6-159">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a18d6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a18d6-160">displayName</span></span>|<span data-ttu-id="a18d6-161">string</span><span class="sxs-lookup"><span data-stu-id="a18d6-161">string</span></span>| <span data-ttu-id="a18d6-162">团队的名称。</span><span class="sxs-lookup"><span data-stu-id="a18d6-162">The name of the team.</span></span> |
|<span data-ttu-id="a18d6-163">description</span><span class="sxs-lookup"><span data-stu-id="a18d6-163">description</span></span>|<span data-ttu-id="a18d6-164">string</span><span class="sxs-lookup"><span data-stu-id="a18d6-164">string</span></span>| <span data-ttu-id="a18d6-165">组的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="a18d6-165">An optional description for the team.</span></span> |
|<span data-ttu-id="a18d6-166">classification</span><span class="sxs-lookup"><span data-stu-id="a18d6-166">classification</span></span>|<span data-ttu-id="a18d6-167">string</span><span class="sxs-lookup"><span data-stu-id="a18d6-167">string</span></span>| <span data-ttu-id="a18d6-168">标签（可选）。</span><span class="sxs-lookup"><span data-stu-id="a18d6-168">An optional label.</span></span> <span data-ttu-id="a18d6-169">通常说明团队的数据或业务敏感性。</span><span class="sxs-lookup"><span data-stu-id="a18d6-169">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="a18d6-170">必须与租户目录中的一个预配置集匹配。</span><span class="sxs-lookup"><span data-stu-id="a18d6-170">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="a18d6-171">specialization</span><span class="sxs-lookup"><span data-stu-id="a18d6-171">specialization</span></span>|[<span data-ttu-id="a18d6-172">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="a18d6-172">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="a18d6-173">可选。</span><span class="sxs-lookup"><span data-stu-id="a18d6-173">Optional.</span></span> <span data-ttu-id="a18d6-174">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="a18d6-174">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="a18d6-175">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="a18d6-175">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="a18d6-176">visibility</span><span class="sxs-lookup"><span data-stu-id="a18d6-176">visibility</span></span>|[<span data-ttu-id="a18d6-177">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="a18d6-177">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="a18d6-178">组和团队的可见性。</span><span class="sxs-lookup"><span data-stu-id="a18d6-178">The visibility of the group and team.</span></span> <span data-ttu-id="a18d6-179">默认值为 Public。</span><span class="sxs-lookup"><span data-stu-id="a18d6-179">Defaults to Public.</span></span> |
|<span data-ttu-id="a18d6-180">funSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-180">funSettings</span></span>|[<span data-ttu-id="a18d6-181">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-181">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="a18d6-182">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="a18d6-182">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="a18d6-183">guestSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-183">guestSettings</span></span>|[<span data-ttu-id="a18d6-184">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-184">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="a18d6-185">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="a18d6-185">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="a18d6-186">internalId</span><span class="sxs-lookup"><span data-stu-id="a18d6-186">internalId</span></span> | <span data-ttu-id="a18d6-187">字符串</span><span class="sxs-lookup"><span data-stu-id="a18d6-187">string</span></span> | <span data-ttu-id="a18d6-188">已在一些位置（如审核日志/[Office 365 管理活动 API](/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a18d6-188">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="a18d6-189">isArchived</span><span class="sxs-lookup"><span data-stu-id="a18d6-189">isArchived</span></span>|<span data-ttu-id="a18d6-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="a18d6-190">Boolean</span></span>|<span data-ttu-id="a18d6-191">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="a18d6-191">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="a18d6-192">memberSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-192">memberSettings</span></span>|[<span data-ttu-id="a18d6-193">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-193">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="a18d6-194">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="a18d6-194">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="a18d6-195">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-195">messagingSettings</span></span>|[<span data-ttu-id="a18d6-196">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="a18d6-196">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="a18d6-197">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="a18d6-197">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="a18d6-198">webUrl</span><span class="sxs-lookup"><span data-stu-id="a18d6-198">webUrl</span></span>|<span data-ttu-id="a18d6-199">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="a18d6-199">string (readonly)</span></span> | <span data-ttu-id="a18d6-200">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="a18d6-200">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="a18d6-201">这是在 Microsoft Teams 客户端中右键单击团队并选择 **获取团队链接** 时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="a18d6-201">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="a18d6-202">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="a18d6-202">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a18d6-203">关系</span><span class="sxs-lookup"><span data-stu-id="a18d6-203">Relationships</span></span>

| <span data-ttu-id="a18d6-204">关系</span><span class="sxs-lookup"><span data-stu-id="a18d6-204">Relationship</span></span> | <span data-ttu-id="a18d6-205">类型</span><span class="sxs-lookup"><span data-stu-id="a18d6-205">Type</span></span> | <span data-ttu-id="a18d6-206">说明</span><span class="sxs-lookup"><span data-stu-id="a18d6-206">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a18d6-207">channels</span><span class="sxs-lookup"><span data-stu-id="a18d6-207">channels</span></span>|<span data-ttu-id="a18d6-208">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-208">[channel](channel.md) collection</span></span>|<span data-ttu-id="a18d6-209">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="a18d6-209">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="a18d6-210">installedApps</span><span class="sxs-lookup"><span data-stu-id="a18d6-210">installedApps</span></span>|<span data-ttu-id="a18d6-211">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-211">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="a18d6-212">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="a18d6-212">The apps installed in this team.</span></span>|
|<span data-ttu-id="a18d6-213">members</span><span class="sxs-lookup"><span data-stu-id="a18d6-213">members</span></span>|<span data-ttu-id="a18d6-214">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-214">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="a18d6-215">团队的成员和所有者。</span><span class="sxs-lookup"><span data-stu-id="a18d6-215">Members and owners of the team.</span></span>|
|<span data-ttu-id="a18d6-216">operations</span><span class="sxs-lookup"><span data-stu-id="a18d6-216">operations</span></span>|<span data-ttu-id="a18d6-217">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d6-217">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="a18d6-218">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="a18d6-218">The async operations that ran or are running on this team.</span></span> | 
|[<span data-ttu-id="a18d6-219">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="a18d6-219">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="a18d6-220">频道</span><span class="sxs-lookup"><span data-stu-id="a18d6-220">channel</span></span>](channel.md)| <span data-ttu-id="a18d6-221">团队的常规频道。</span><span class="sxs-lookup"><span data-stu-id="a18d6-221">The general channel for the team.</span></span> | 
|<span data-ttu-id="a18d6-222">schedule</span><span class="sxs-lookup"><span data-stu-id="a18d6-222">schedule</span></span>|[<span data-ttu-id="a18d6-223">日程安排</span><span class="sxs-lookup"><span data-stu-id="a18d6-223">schedule</span></span>](schedule.md)| <span data-ttu-id="a18d6-224">此团队的排班安排。</span><span class="sxs-lookup"><span data-stu-id="a18d6-224">The schedule of shifts for this team.</span></span>|
|<span data-ttu-id="a18d6-225">template</span><span class="sxs-lookup"><span data-stu-id="a18d6-225">template</span></span>|[<span data-ttu-id="a18d6-226">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="a18d6-226">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="a18d6-227">创建此团队时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="a18d6-227">The template this team was created from.</span></span> <span data-ttu-id="a18d6-228">请参阅[可用模板](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="a18d6-228">See [available templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a18d6-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a18d6-229">JSON representation</span></span>

<span data-ttu-id="a18d6-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a18d6-230">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="a18d6-231">**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。</span><span class="sxs-lookup"><span data-stu-id="a18d6-231">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="a18d6-232">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a18d6-232">See also</span></span>

- [<span data-ttu-id="a18d6-233">将 Microsoft Graph API 与 Microsoft Teams 结合使用</span><span class="sxs-lookup"><span data-stu-id="a18d6-233">Use the Microsoft Graph API to work with Microsoft Teams</span></span>](teams-api-overview.md)
- [<span data-ttu-id="a18d6-234">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="a18d6-234">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="a18d6-235">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="a18d6-235">List all teams</span></span>](/graph/teams-list-all-teams)

