---
title: 团队资源类型
description: 'Microsoft Teams 团队是频道的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 892d9bedb188ea0a39a611fdb207248958624f28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056427"
---
# <a name="team-resource-type"></a><span data-ttu-id="e7e9d-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="e7e9d-103">team resource type</span></span>

<span data-ttu-id="e7e9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7e9d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e7e9d-105">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="e7e9d-106">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="e7e9d-107">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="e7e9d-108">该组具有与团队相同的 ID，例如 /groups/{id}/team 与 /teams/{id} 相同。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="e7e9d-109">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e7e9d-110">方法</span><span class="sxs-lookup"><span data-stu-id="e7e9d-110">Methods</span></span>

| <span data-ttu-id="e7e9d-111">方法</span><span class="sxs-lookup"><span data-stu-id="e7e9d-111">Method</span></span>       | <span data-ttu-id="e7e9d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7e9d-112">Return Type</span></span>  |<span data-ttu-id="e7e9d-113">说明</span><span class="sxs-lookup"><span data-stu-id="e7e9d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7e9d-114">创建团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-114">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="e7e9d-115">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e7e9d-115">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="e7e9d-116">从头开始创建团队。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-116">Create a team from scratch.</span></span> |
|[<span data-ttu-id="e7e9d-117">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-117">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="e7e9d-118">team</span><span class="sxs-lookup"><span data-stu-id="e7e9d-118">team</span></span>](team.md) | <span data-ttu-id="e7e9d-119">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-119">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="e7e9d-120">获取团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-120">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="e7e9d-121">team</span><span class="sxs-lookup"><span data-stu-id="e7e9d-121">team</span></span>](team.md) | <span data-ttu-id="e7e9d-122">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-122">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="e7e9d-123">更新团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-123">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="e7e9d-124">team</span><span class="sxs-lookup"><span data-stu-id="e7e9d-124">team</span></span>](team.md) |<span data-ttu-id="e7e9d-125">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-125">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="e7e9d-126">删除团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-126">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="e7e9d-127">无</span><span class="sxs-lookup"><span data-stu-id="e7e9d-127">None</span></span> |<span data-ttu-id="e7e9d-128">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-128">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="e7e9d-129">克隆团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-129">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="e7e9d-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e7e9d-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e7e9d-131">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-131">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="e7e9d-132">存档团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-132">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="e7e9d-133">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e7e9d-133">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e7e9d-134">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-134">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="e7e9d-135">解档团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-135">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="e7e9d-136">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="e7e9d-136">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="e7e9d-137">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-137">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="e7e9d-138">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-138">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="e7e9d-139">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e9d-139">[team](team.md) collection</span></span> | <span data-ttu-id="e7e9d-140">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-140">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="e7e9d-141">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-141">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="e7e9d-142">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e9d-142">[group](group.md) collection</span></span> | <span data-ttu-id="e7e9d-143">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-143">List all groups that have teams.</span></span> |
|[<span data-ttu-id="e7e9d-144">将应用发布到你的组织</span><span class="sxs-lookup"><span data-stu-id="e7e9d-144">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="e7e9d-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e7e9d-145">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="e7e9d-146">创建仅对你的组织可见的 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-146">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="e7e9d-147">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="e7e9d-147">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="e7e9d-148">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e7e9d-148">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="e7e9d-149">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-149">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="e7e9d-150">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="e7e9d-150">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e7e9d-151">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e7e9d-151">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="e7e9d-152">将选项卡添加（安装）到团队的频道。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-152">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7e9d-153">属性</span><span class="sxs-lookup"><span data-stu-id="e7e9d-153">Properties</span></span>

| <span data-ttu-id="e7e9d-154">属性</span><span class="sxs-lookup"><span data-stu-id="e7e9d-154">Property</span></span> | <span data-ttu-id="e7e9d-155">类型</span><span class="sxs-lookup"><span data-stu-id="e7e9d-155">Type</span></span> | <span data-ttu-id="e7e9d-156">说明</span><span class="sxs-lookup"><span data-stu-id="e7e9d-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e7e9d-157">displayName</span><span class="sxs-lookup"><span data-stu-id="e7e9d-157">displayName</span></span>|<span data-ttu-id="e7e9d-158">string</span><span class="sxs-lookup"><span data-stu-id="e7e9d-158">string</span></span>| <span data-ttu-id="e7e9d-159">团队的名称。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-159">The name of the team.</span></span> |
|<span data-ttu-id="e7e9d-160">description</span><span class="sxs-lookup"><span data-stu-id="e7e9d-160">description</span></span>|<span data-ttu-id="e7e9d-161">string</span><span class="sxs-lookup"><span data-stu-id="e7e9d-161">string</span></span>| <span data-ttu-id="e7e9d-162">组的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-162">An optional description for the team.</span></span> |
|<span data-ttu-id="e7e9d-163">classification</span><span class="sxs-lookup"><span data-stu-id="e7e9d-163">classification</span></span>|<span data-ttu-id="e7e9d-164">string</span><span class="sxs-lookup"><span data-stu-id="e7e9d-164">string</span></span>| <span data-ttu-id="e7e9d-165">标签（可选）。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-165">An optional label.</span></span> <span data-ttu-id="e7e9d-166">通常说明团队的数据或业务敏感性。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-166">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="e7e9d-167">必须与租户目录中的一个预配置集匹配。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-167">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="e7e9d-168">specialization</span><span class="sxs-lookup"><span data-stu-id="e7e9d-168">specialization</span></span>|[<span data-ttu-id="e7e9d-169">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="e7e9d-169">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="e7e9d-170">可选。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-170">Optional.</span></span> <span data-ttu-id="e7e9d-171">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-171">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="e7e9d-172">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-172">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="e7e9d-173">visibility</span><span class="sxs-lookup"><span data-stu-id="e7e9d-173">visibility</span></span>|[<span data-ttu-id="e7e9d-174">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="e7e9d-174">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="e7e9d-175">组和团队的可见性。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-175">The visibility of the group and team.</span></span> <span data-ttu-id="e7e9d-176">默认值为 Public。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-176">Defaults to Public.</span></span> |
|<span data-ttu-id="e7e9d-177">funSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-177">funSettings</span></span>|[<span data-ttu-id="e7e9d-178">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-178">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="e7e9d-179">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-179">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="e7e9d-180">guestSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-180">guestSettings</span></span>|[<span data-ttu-id="e7e9d-181">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-181">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="e7e9d-182">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-182">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="e7e9d-183">internalId</span><span class="sxs-lookup"><span data-stu-id="e7e9d-183">internalId</span></span> | <span data-ttu-id="e7e9d-184">字符串</span><span class="sxs-lookup"><span data-stu-id="e7e9d-184">string</span></span> | <span data-ttu-id="e7e9d-185">已在一些位置（如审核日志/[Office 365 管理活动 API](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-185">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="e7e9d-186">isArchived</span><span class="sxs-lookup"><span data-stu-id="e7e9d-186">isArchived</span></span>|<span data-ttu-id="e7e9d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7e9d-187">Boolean</span></span>|<span data-ttu-id="e7e9d-188">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-188">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="e7e9d-189">memberSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-189">memberSettings</span></span>|[<span data-ttu-id="e7e9d-190">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-190">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="e7e9d-191">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-191">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="e7e9d-192">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-192">messagingSettings</span></span>|[<span data-ttu-id="e7e9d-193">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="e7e9d-193">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="e7e9d-194">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-194">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="e7e9d-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="e7e9d-195">webUrl</span></span>|<span data-ttu-id="e7e9d-196">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="e7e9d-196">string (readonly)</span></span> | <span data-ttu-id="e7e9d-197">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-197">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="e7e9d-198">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-198">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="e7e9d-199">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-199">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e7e9d-200">关系</span><span class="sxs-lookup"><span data-stu-id="e7e9d-200">Relationships</span></span>

| <span data-ttu-id="e7e9d-201">关系</span><span class="sxs-lookup"><span data-stu-id="e7e9d-201">Relationship</span></span> | <span data-ttu-id="e7e9d-202">类型</span><span class="sxs-lookup"><span data-stu-id="e7e9d-202">Type</span></span> | <span data-ttu-id="e7e9d-203">说明</span><span class="sxs-lookup"><span data-stu-id="e7e9d-203">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e7e9d-204">channels</span><span class="sxs-lookup"><span data-stu-id="e7e9d-204">channels</span></span>|<span data-ttu-id="e7e9d-205">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e9d-205">[channel](channel.md) collection</span></span>|<span data-ttu-id="e7e9d-206">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-206">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="e7e9d-207">installedApps</span><span class="sxs-lookup"><span data-stu-id="e7e9d-207">installedApps</span></span>|<span data-ttu-id="e7e9d-208">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e9d-208">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="e7e9d-209">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-209">The apps installed in this team.</span></span>|
|<span data-ttu-id="e7e9d-210">members</span><span class="sxs-lookup"><span data-stu-id="e7e9d-210">members</span></span>|<span data-ttu-id="e7e9d-211">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e9d-211">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="e7e9d-212">团队的成员和所有者。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-212">Members and owners of the team.</span></span>|
|<span data-ttu-id="e7e9d-213">operations</span><span class="sxs-lookup"><span data-stu-id="e7e9d-213">operations</span></span>|<span data-ttu-id="e7e9d-214">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e9d-214">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="e7e9d-215">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-215">The async operations that ran or are running on this team.</span></span> | 
|[<span data-ttu-id="e7e9d-216">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="e7e9d-216">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="e7e9d-217">频道</span><span class="sxs-lookup"><span data-stu-id="e7e9d-217">channel</span></span>](channel.md)| <span data-ttu-id="e7e9d-218">团队的常规频道。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-218">The general channel for the team.</span></span> | 
|<span data-ttu-id="e7e9d-219">schedule</span><span class="sxs-lookup"><span data-stu-id="e7e9d-219">schedule</span></span>|[<span data-ttu-id="e7e9d-220">日程安排</span><span class="sxs-lookup"><span data-stu-id="e7e9d-220">schedule</span></span>](schedule.md)| <span data-ttu-id="e7e9d-221">此团队的排班安排。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-221">The schedule of shifts for this team.</span></span>|
|<span data-ttu-id="e7e9d-222">template</span><span class="sxs-lookup"><span data-stu-id="e7e9d-222">template</span></span>|[<span data-ttu-id="e7e9d-223">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="e7e9d-223">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="e7e9d-224">创建此团队时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-224">The template this team was created from.</span></span> <span data-ttu-id="e7e9d-225">请参阅[可用模板](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-225">See [available templates](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e7e9d-226">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7e9d-226">JSON representation</span></span>

<span data-ttu-id="e7e9d-227">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-227">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="e7e9d-228">**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。</span><span class="sxs-lookup"><span data-stu-id="e7e9d-228">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e7e9d-229">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e7e9d-229">See Also</span></span>
- [<span data-ttu-id="e7e9d-230">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="e7e9d-230">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="e7e9d-231">使用 Teams API</span><span class="sxs-lookup"><span data-stu-id="e7e9d-231">Using Teams APIs</span></span>](teams-api-overview.md)

