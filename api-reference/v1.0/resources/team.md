---
title: 团队资源类型
description: 'Microsoft Teams 团队是频道的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0772457d91b2f6ad1bca1330841ba247dad62dba
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582028"
---
# <a name="team-resource-type"></a><span data-ttu-id="d0fbe-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="d0fbe-103">team resource type</span></span>

<span data-ttu-id="d0fbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0fbe-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d0fbe-105">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="d0fbe-106">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="d0fbe-107">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="d0fbe-108">该组具有与团队相同的 ID，例如 /groups/{id}/team 与 /teams/{id} 相同。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="d0fbe-109">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d0fbe-110">方法</span><span class="sxs-lookup"><span data-stu-id="d0fbe-110">Methods</span></span>

| <span data-ttu-id="d0fbe-111">方法</span><span class="sxs-lookup"><span data-stu-id="d0fbe-111">Method</span></span>       | <span data-ttu-id="d0fbe-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0fbe-112">Return Type</span></span>  |<span data-ttu-id="d0fbe-113">说明</span><span class="sxs-lookup"><span data-stu-id="d0fbe-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0fbe-114">创建团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-114">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="d0fbe-115">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d0fbe-115">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="d0fbe-116">从头开始创建团队。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-116">Create a team from scratch.</span></span> |
|[<span data-ttu-id="d0fbe-117">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-117">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="d0fbe-118">team</span><span class="sxs-lookup"><span data-stu-id="d0fbe-118">team</span></span>](team.md) | <span data-ttu-id="d0fbe-119">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-119">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="d0fbe-120">获取团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-120">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="d0fbe-121">team</span><span class="sxs-lookup"><span data-stu-id="d0fbe-121">team</span></span>](team.md) | <span data-ttu-id="d0fbe-122">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-122">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="d0fbe-123">更新团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-123">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="d0fbe-124">team</span><span class="sxs-lookup"><span data-stu-id="d0fbe-124">team</span></span>](team.md) |<span data-ttu-id="d0fbe-125">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-125">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="d0fbe-126">删除团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-126">Delete team</span></span>](../api/group-delete.md) | <span data-ttu-id="d0fbe-127">无</span><span class="sxs-lookup"><span data-stu-id="d0fbe-127">None</span></span> |<span data-ttu-id="d0fbe-128">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-128">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="d0fbe-129">List members</span><span class="sxs-lookup"><span data-stu-id="d0fbe-129">List members</span></span>](../api/team-list-members.md)|<span data-ttu-id="d0fbe-130">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0fbe-130">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="d0fbe-131">从成员导航属性中获取 conversationMembers。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-131">Get the conversationMembers from the members navigation property.</span></span>|
|[<span data-ttu-id="d0fbe-132">添加成员</span><span class="sxs-lookup"><span data-stu-id="d0fbe-132">Add members</span></span>](../api/team-post-members.md)|[<span data-ttu-id="d0fbe-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d0fbe-133">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d0fbe-134">添加新成员。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-134">Add a new member.</span></span>|
|[<span data-ttu-id="d0fbe-135">删除成员</span><span class="sxs-lookup"><span data-stu-id="d0fbe-135">Remove members</span></span>](../api/team-delete-members.md)|<span data-ttu-id="d0fbe-136">无</span><span class="sxs-lookup"><span data-stu-id="d0fbe-136">None</span></span>|<span data-ttu-id="d0fbe-137">删除 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-137">Delete a [conversationMember](../resources/conversationmember.md) object.</span></span>|
|[<span data-ttu-id="d0fbe-138">更改成员角色</span><span class="sxs-lookup"><span data-stu-id="d0fbe-138">Change member's role</span></span>](/graph/api/conversationmember-update?view=graph-rest-beta&tabs=http&preserve-view=true)|[<span data-ttu-id="d0fbe-139">conversationMember</span><span class="sxs-lookup"><span data-stu-id="d0fbe-139">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="d0fbe-140">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-140">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="d0fbe-141">存档团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-141">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="d0fbe-142">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d0fbe-142">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="d0fbe-143">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-143">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="d0fbe-144">解档团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-144">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="d0fbe-145">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d0fbe-145">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="d0fbe-146">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-146">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="d0fbe-147">克隆团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-147">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="d0fbe-148">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d0fbe-148">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="d0fbe-149">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-149">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="d0fbe-150">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-150">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="d0fbe-151">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0fbe-151">[team](team.md) collection</span></span> | <span data-ttu-id="d0fbe-152">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-152">List the teams you are a member of.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0fbe-153">属性</span><span class="sxs-lookup"><span data-stu-id="d0fbe-153">Properties</span></span>

| <span data-ttu-id="d0fbe-154">属性</span><span class="sxs-lookup"><span data-stu-id="d0fbe-154">Property</span></span> | <span data-ttu-id="d0fbe-155">类型</span><span class="sxs-lookup"><span data-stu-id="d0fbe-155">Type</span></span> | <span data-ttu-id="d0fbe-156">说明</span><span class="sxs-lookup"><span data-stu-id="d0fbe-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d0fbe-157">displayName</span><span class="sxs-lookup"><span data-stu-id="d0fbe-157">displayName</span></span>|<span data-ttu-id="d0fbe-158">string</span><span class="sxs-lookup"><span data-stu-id="d0fbe-158">string</span></span>| <span data-ttu-id="d0fbe-159">团队的名称。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-159">The name of the team.</span></span> |
|<span data-ttu-id="d0fbe-160">description</span><span class="sxs-lookup"><span data-stu-id="d0fbe-160">description</span></span>|<span data-ttu-id="d0fbe-161">string</span><span class="sxs-lookup"><span data-stu-id="d0fbe-161">string</span></span>| <span data-ttu-id="d0fbe-162">组的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-162">An optional description for the team.</span></span> |
|<span data-ttu-id="d0fbe-163">classification</span><span class="sxs-lookup"><span data-stu-id="d0fbe-163">classification</span></span>|<span data-ttu-id="d0fbe-164">string</span><span class="sxs-lookup"><span data-stu-id="d0fbe-164">string</span></span>| <span data-ttu-id="d0fbe-165">标签（可选）。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-165">An optional label.</span></span> <span data-ttu-id="d0fbe-166">通常说明团队的数据或业务敏感性。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-166">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="d0fbe-167">必须与租户目录中的一个预配置集匹配。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-167">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="d0fbe-168">specialization</span><span class="sxs-lookup"><span data-stu-id="d0fbe-168">specialization</span></span>|[<span data-ttu-id="d0fbe-169">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="d0fbe-169">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="d0fbe-170">可选。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-170">Optional.</span></span> <span data-ttu-id="d0fbe-171">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-171">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="d0fbe-172">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-172">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="d0fbe-173">visibility</span><span class="sxs-lookup"><span data-stu-id="d0fbe-173">visibility</span></span>|[<span data-ttu-id="d0fbe-174">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="d0fbe-174">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="d0fbe-175">组和团队的可见性。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-175">The visibility of the group and team.</span></span> <span data-ttu-id="d0fbe-176">默认值为 Public。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-176">Defaults to Public.</span></span> |
|<span data-ttu-id="d0fbe-177">funSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-177">funSettings</span></span>|[<span data-ttu-id="d0fbe-178">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-178">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="d0fbe-179">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-179">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="d0fbe-180">guestSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-180">guestSettings</span></span>|[<span data-ttu-id="d0fbe-181">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-181">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="d0fbe-182">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-182">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="d0fbe-183">internalId</span><span class="sxs-lookup"><span data-stu-id="d0fbe-183">internalId</span></span> | <span data-ttu-id="d0fbe-184">字符串</span><span class="sxs-lookup"><span data-stu-id="d0fbe-184">string</span></span> | <span data-ttu-id="d0fbe-185">已在一些位置（如审核日志/[Office 365 管理活动 API](/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-185">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="d0fbe-186">isArchived</span><span class="sxs-lookup"><span data-stu-id="d0fbe-186">isArchived</span></span>|<span data-ttu-id="d0fbe-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fbe-187">Boolean</span></span>|<span data-ttu-id="d0fbe-188">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-188">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="d0fbe-189">memberSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-189">memberSettings</span></span>|[<span data-ttu-id="d0fbe-190">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-190">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="d0fbe-191">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-191">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="d0fbe-192">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-192">messagingSettings</span></span>|[<span data-ttu-id="d0fbe-193">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="d0fbe-193">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="d0fbe-194">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-194">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="d0fbe-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="d0fbe-195">webUrl</span></span>|<span data-ttu-id="d0fbe-196">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="d0fbe-196">string (readonly)</span></span> | <span data-ttu-id="d0fbe-197">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-197">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="d0fbe-198">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-198">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="d0fbe-199">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-199">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d0fbe-200">关系</span><span class="sxs-lookup"><span data-stu-id="d0fbe-200">Relationships</span></span>

| <span data-ttu-id="d0fbe-201">关系</span><span class="sxs-lookup"><span data-stu-id="d0fbe-201">Relationship</span></span> | <span data-ttu-id="d0fbe-202">类型</span><span class="sxs-lookup"><span data-stu-id="d0fbe-202">Type</span></span> | <span data-ttu-id="d0fbe-203">说明</span><span class="sxs-lookup"><span data-stu-id="d0fbe-203">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d0fbe-204">channels</span><span class="sxs-lookup"><span data-stu-id="d0fbe-204">channels</span></span>|<span data-ttu-id="d0fbe-205">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0fbe-205">[channel](channel.md) collection</span></span>|<span data-ttu-id="d0fbe-206">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-206">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="d0fbe-207">installedApps</span><span class="sxs-lookup"><span data-stu-id="d0fbe-207">installedApps</span></span>|<span data-ttu-id="d0fbe-208">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0fbe-208">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="d0fbe-209">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-209">The apps installed in this team.</span></span>|
|<span data-ttu-id="d0fbe-210">members</span><span class="sxs-lookup"><span data-stu-id="d0fbe-210">members</span></span>|<span data-ttu-id="d0fbe-211">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0fbe-211">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="d0fbe-212">团队的成员和所有者。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-212">Members and owners of the team.</span></span>|
|<span data-ttu-id="d0fbe-213">operations</span><span class="sxs-lookup"><span data-stu-id="d0fbe-213">operations</span></span>|<span data-ttu-id="d0fbe-214">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0fbe-214">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="d0fbe-215">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-215">The async operations that ran or are running on this team.</span></span> | 
|[<span data-ttu-id="d0fbe-216">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="d0fbe-216">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="d0fbe-217">频道</span><span class="sxs-lookup"><span data-stu-id="d0fbe-217">channel</span></span>](channel.md)| <span data-ttu-id="d0fbe-218">团队的常规频道。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-218">The general channel for the team.</span></span> | 
|<span data-ttu-id="d0fbe-219">schedule</span><span class="sxs-lookup"><span data-stu-id="d0fbe-219">schedule</span></span>|[<span data-ttu-id="d0fbe-220">日程安排</span><span class="sxs-lookup"><span data-stu-id="d0fbe-220">schedule</span></span>](schedule.md)| <span data-ttu-id="d0fbe-221">此团队的排班安排。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-221">The schedule of shifts for this team.</span></span>|
|<span data-ttu-id="d0fbe-222">template</span><span class="sxs-lookup"><span data-stu-id="d0fbe-222">template</span></span>|[<span data-ttu-id="d0fbe-223">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="d0fbe-223">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="d0fbe-224">创建此团队时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-224">The template this team was created from.</span></span> <span data-ttu-id="d0fbe-225">请参阅[可用模板](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-225">See [available templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0fbe-226">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0fbe-226">JSON representation</span></span>

<span data-ttu-id="d0fbe-227">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-227">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="d0fbe-228">**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。</span><span class="sxs-lookup"><span data-stu-id="d0fbe-228">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d0fbe-229">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d0fbe-229">See also</span></span>

- [<span data-ttu-id="d0fbe-230">将 Microsoft Graph API 与 Microsoft Teams 结合使用</span><span class="sxs-lookup"><span data-stu-id="d0fbe-230">Use the Microsoft Graph API to work with Microsoft Teams</span></span>](teams-api-overview.md)
- [<span data-ttu-id="d0fbe-231">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="d0fbe-231">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="d0fbe-232">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="d0fbe-232">List all teams</span></span>](/graph/teams-list-all-teams)

