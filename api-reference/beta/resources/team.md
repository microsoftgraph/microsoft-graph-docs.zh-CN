---
title: 团队资源类型
description: 'Microsoft Teams 中的团队是频道的集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cf94e73bfd7ad05fea8f52ea1f2f219b7933ffa7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793736"
---
# <a name="team-resource-type"></a><span data-ttu-id="87aec-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="87aec-103">team resource type</span></span>

<span data-ttu-id="87aec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87aec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87aec-105">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="87aec-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span> <span data-ttu-id="87aec-106">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="87aec-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="87aec-107">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="87aec-107">Every team is associated with a [group](../resources/group.md).</span></span> <span data-ttu-id="87aec-108">该组具有与团队相同的 ID，例如 `/groups/{id}/team` 与 `/teams/{id}` 相同。</span><span class="sxs-lookup"><span data-stu-id="87aec-108">The group has the same ID as the team - for example, `/groups/{id}/team` is the same as `/teams/{id}`.</span></span> <span data-ttu-id="87aec-109">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="87aec-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="87aec-110">方法</span><span class="sxs-lookup"><span data-stu-id="87aec-110">Methods</span></span>

| <span data-ttu-id="87aec-111">方法</span><span class="sxs-lookup"><span data-stu-id="87aec-111">Method</span></span>       | <span data-ttu-id="87aec-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="87aec-112">Return Type</span></span>  |<span data-ttu-id="87aec-113">说明</span><span class="sxs-lookup"><span data-stu-id="87aec-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="87aec-114">创建团队</span><span class="sxs-lookup"><span data-stu-id="87aec-114">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="87aec-115">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="87aec-115">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="87aec-116">从头开始创建团队。</span><span class="sxs-lookup"><span data-stu-id="87aec-116">Create a team from scratch.</span></span> |
|[<span data-ttu-id="87aec-117">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="87aec-117">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="87aec-118">team</span><span class="sxs-lookup"><span data-stu-id="87aec-118">team</span></span>](team.md) | <span data-ttu-id="87aec-119">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="87aec-119">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="87aec-120">获取团队</span><span class="sxs-lookup"><span data-stu-id="87aec-120">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="87aec-121">team</span><span class="sxs-lookup"><span data-stu-id="87aec-121">team</span></span>](team.md) | <span data-ttu-id="87aec-122">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87aec-122">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="87aec-123">更新团队</span><span class="sxs-lookup"><span data-stu-id="87aec-123">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="87aec-124">team</span><span class="sxs-lookup"><span data-stu-id="87aec-124">team</span></span>](team.md) |<span data-ttu-id="87aec-125">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="87aec-125">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="87aec-126">删除团队</span><span class="sxs-lookup"><span data-stu-id="87aec-126">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="87aec-127">无</span><span class="sxs-lookup"><span data-stu-id="87aec-127">None</span></span> |<span data-ttu-id="87aec-128">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="87aec-128">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="87aec-129">克隆团队</span><span class="sxs-lookup"><span data-stu-id="87aec-129">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="87aec-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="87aec-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="87aec-131">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="87aec-131">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="87aec-132">存档团队</span><span class="sxs-lookup"><span data-stu-id="87aec-132">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="87aec-133">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="87aec-133">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="87aec-134">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="87aec-134">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="87aec-135">解档团队</span><span class="sxs-lookup"><span data-stu-id="87aec-135">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="87aec-136">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="87aec-136">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="87aec-137">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="87aec-137">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="87aec-138">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="87aec-138">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="87aec-139">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87aec-139">[team](team.md) collection</span></span> | <span data-ttu-id="87aec-140">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="87aec-140">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="87aec-141">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="87aec-141">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="87aec-142">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87aec-142">[group](group.md) collection</span></span> | <span data-ttu-id="87aec-143">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="87aec-143">List all groups that have teams.</span></span> |
|[<span data-ttu-id="87aec-144">获取团队照片</span><span class="sxs-lookup"><span data-stu-id="87aec-144">Get team photo</span></span>](../api/team-get-photo.md) | <span data-ttu-id="87aec-145">二进制数据</span><span class="sxs-lookup"><span data-stu-id="87aec-145">Binary data</span></span> | <span data-ttu-id="87aec-146">获取团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="87aec-146">Get the photo (picture) for a team.</span></span> |
|[<span data-ttu-id="87aec-147">更新团队照片</span><span class="sxs-lookup"><span data-stu-id="87aec-147">Update team photo</span></span>](../api/team-update-photo.md) | <span data-ttu-id="87aec-148">无</span><span class="sxs-lookup"><span data-stu-id="87aec-148">None</span></span> | <span data-ttu-id="87aec-149">更新团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="87aec-149">Update the photo (picture) for a team.</span></span> |

## <a name="properties"></a><span data-ttu-id="87aec-150">属性</span><span class="sxs-lookup"><span data-stu-id="87aec-150">Properties</span></span>

| <span data-ttu-id="87aec-151">属性</span><span class="sxs-lookup"><span data-stu-id="87aec-151">Property</span></span> | <span data-ttu-id="87aec-152">类型</span><span class="sxs-lookup"><span data-stu-id="87aec-152">Type</span></span> | <span data-ttu-id="87aec-153">说明</span><span class="sxs-lookup"><span data-stu-id="87aec-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="87aec-154">displayName</span><span class="sxs-lookup"><span data-stu-id="87aec-154">displayName</span></span>|<span data-ttu-id="87aec-155">string</span><span class="sxs-lookup"><span data-stu-id="87aec-155">string</span></span>| <span data-ttu-id="87aec-156">团队的名称。</span><span class="sxs-lookup"><span data-stu-id="87aec-156">The name of the team.</span></span> |
|<span data-ttu-id="87aec-157">description</span><span class="sxs-lookup"><span data-stu-id="87aec-157">description</span></span>|<span data-ttu-id="87aec-158">string</span><span class="sxs-lookup"><span data-stu-id="87aec-158">string</span></span>| <span data-ttu-id="87aec-159">组的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="87aec-159">An optional description for the team.</span></span> |
|<span data-ttu-id="87aec-160">classification</span><span class="sxs-lookup"><span data-stu-id="87aec-160">classification</span></span>|<span data-ttu-id="87aec-161">string</span><span class="sxs-lookup"><span data-stu-id="87aec-161">string</span></span>| <span data-ttu-id="87aec-162">标签（可选）。</span><span class="sxs-lookup"><span data-stu-id="87aec-162">An optional label.</span></span> <span data-ttu-id="87aec-163">通常说明团队的数据或业务敏感性。</span><span class="sxs-lookup"><span data-stu-id="87aec-163">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="87aec-164">必须与租户目录中的一个预配置集匹配。</span><span class="sxs-lookup"><span data-stu-id="87aec-164">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="87aec-165">specialization</span><span class="sxs-lookup"><span data-stu-id="87aec-165">specialization</span></span>|[<span data-ttu-id="87aec-166">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="87aec-166">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="87aec-167">可选。</span><span class="sxs-lookup"><span data-stu-id="87aec-167">Optional.</span></span> <span data-ttu-id="87aec-168">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="87aec-168">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="87aec-169">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="87aec-169">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="87aec-170">visibility</span><span class="sxs-lookup"><span data-stu-id="87aec-170">visibility</span></span>|[<span data-ttu-id="87aec-171">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="87aec-171">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="87aec-172">组和团队的可见性。</span><span class="sxs-lookup"><span data-stu-id="87aec-172">The visibility of a the group and team.</span></span> <span data-ttu-id="87aec-173">默认值为 Public。</span><span class="sxs-lookup"><span data-stu-id="87aec-173">Defaults to Public.</span></span> |
|<span data-ttu-id="87aec-174">funSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-174">funSettings</span></span>|[<span data-ttu-id="87aec-175">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-175">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="87aec-176">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="87aec-176">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="87aec-177">guestSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-177">guestSettings</span></span>|[<span data-ttu-id="87aec-178">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-178">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="87aec-179">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="87aec-179">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="87aec-180">internalId</span><span class="sxs-lookup"><span data-stu-id="87aec-180">internalId</span></span> | <span data-ttu-id="87aec-181">字符串</span><span class="sxs-lookup"><span data-stu-id="87aec-181">string</span></span> | <span data-ttu-id="87aec-182">已在一些位置（如审核日志/[Office 365 管理活动 API](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="87aec-182">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="87aec-183">isArchived</span><span class="sxs-lookup"><span data-stu-id="87aec-183">isArchived</span></span>|<span data-ttu-id="87aec-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="87aec-184">Boolean</span></span>|<span data-ttu-id="87aec-185">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="87aec-185">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="87aec-186">memberSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-186">memberSettings</span></span>|[<span data-ttu-id="87aec-187">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-187">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="87aec-188">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="87aec-188">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="87aec-189">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-189">messagingSettings</span></span>|[<span data-ttu-id="87aec-190">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-190">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="87aec-191">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="87aec-191">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="87aec-192">discoverySettings</span><span class="sxs-lookup"><span data-stu-id="87aec-192">discoverySettings</span></span>|[<span data-ttu-id="87aec-193">teamDiscoverySettings</span><span class="sxs-lookup"><span data-stu-id="87aec-193">teamDiscoverySettings</span></span>](teamdiscoverysettings.md) |<span data-ttu-id="87aec-194">用于让他人配置团队可发现性的设置。</span><span class="sxs-lookup"><span data-stu-id="87aec-194">Settings to configure team discoverability by others.</span></span>|
|<span data-ttu-id="87aec-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="87aec-195">webUrl</span></span>|<span data-ttu-id="87aec-196">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="87aec-196">string (readonly)</span></span> | <span data-ttu-id="87aec-197">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="87aec-197">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="87aec-198">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="87aec-198">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="87aec-199">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="87aec-199">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="87aec-200">classSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-200">classSettings</span></span>|[<span data-ttu-id="87aec-201">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="87aec-201">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="87aec-202">配置班级设置。</span><span class="sxs-lookup"><span data-stu-id="87aec-202">Configure settings of a class.</span></span> <span data-ttu-id="87aec-203">仅当团队代表班级时可用。</span><span class="sxs-lookup"><span data-stu-id="87aec-203">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87aec-204">关系</span><span class="sxs-lookup"><span data-stu-id="87aec-204">Relationships</span></span>

| <span data-ttu-id="87aec-205">关系</span><span class="sxs-lookup"><span data-stu-id="87aec-205">Relationship</span></span> | <span data-ttu-id="87aec-206">类型</span><span class="sxs-lookup"><span data-stu-id="87aec-206">Type</span></span> | <span data-ttu-id="87aec-207">说明</span><span class="sxs-lookup"><span data-stu-id="87aec-207">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="87aec-208">channels</span><span class="sxs-lookup"><span data-stu-id="87aec-208">channels</span></span>|<span data-ttu-id="87aec-209">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87aec-209">[channel](channel.md) collection</span></span>|<span data-ttu-id="87aec-210">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="87aec-210">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="87aec-211">installedApps</span><span class="sxs-lookup"><span data-stu-id="87aec-211">installedApps</span></span>|<span data-ttu-id="87aec-212">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87aec-212">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="87aec-213">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="87aec-213">The apps installed in this team.</span></span>|
|<span data-ttu-id="87aec-214">owners</span><span class="sxs-lookup"><span data-stu-id="87aec-214">owners</span></span>|[<span data-ttu-id="87aec-215">user</span><span class="sxs-lookup"><span data-stu-id="87aec-215">user</span></span>](user.md)| <span data-ttu-id="87aec-216">此团队的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="87aec-216">The list of this team's owners.</span></span> <span data-ttu-id="87aec-217">目前，在使用应用程序权限创建团队时，必须指定一个所有者。</span><span class="sxs-lookup"><span data-stu-id="87aec-217">Currently, when creating a team using application permissions, exactly one owner must be specified.</span></span> <span data-ttu-id="87aec-218">当使用用户委派的权限时，不能指定任何所有者（当前用户是所有者）。</span><span class="sxs-lookup"><span data-stu-id="87aec-218">When using user delegated permissions, no owner can be specified (the current user is the owner).</span></span> <span data-ttu-id="87aec-219">必须将所有者指定为对象 ID (GUID)，而不是 UPN。</span><span class="sxs-lookup"><span data-stu-id="87aec-219">Owner must be specified as an object ID (GUID), not a UPN.</span></span> |
|<span data-ttu-id="87aec-220">operations</span><span class="sxs-lookup"><span data-stu-id="87aec-220">operations</span></span>|<span data-ttu-id="87aec-221">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87aec-221">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="87aec-222">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="87aec-222">The async operations that ran or are running on this team.</span></span> | 
|[<span data-ttu-id="87aec-223">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="87aec-223">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="87aec-224">频道</span><span class="sxs-lookup"><span data-stu-id="87aec-224">channel</span></span>](channel.md)| <span data-ttu-id="87aec-225">团队的常规频道。</span><span class="sxs-lookup"><span data-stu-id="87aec-225">The general channel for the team.</span></span> | 
|<span data-ttu-id="87aec-226">schedule</span><span class="sxs-lookup"><span data-stu-id="87aec-226">schedule</span></span>|[<span data-ttu-id="87aec-227">日程安排</span><span class="sxs-lookup"><span data-stu-id="87aec-227">schedule</span></span>](schedule.md)| <span data-ttu-id="87aec-228">此团队的排班安排。</span><span class="sxs-lookup"><span data-stu-id="87aec-228">The schedule of shifts for this team.</span></span>|
|<span data-ttu-id="87aec-229">template</span><span class="sxs-lookup"><span data-stu-id="87aec-229">template</span></span>|[<span data-ttu-id="87aec-230">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="87aec-230">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="87aec-231">创建此团队时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="87aec-231">The template this team was created from.</span></span> <span data-ttu-id="87aec-232">请参阅[可用模板](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="87aec-232">See [available templates](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87aec-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87aec-233">JSON representation</span></span>

<span data-ttu-id="87aec-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87aec-234">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="87aec-235">**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。</span><span class="sxs-lookup"><span data-stu-id="87aec-235">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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
  "discoverySettings": {"@odata.type": "microsoft.graph.teamDiscoverySettings"},
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "displayName": "string",
  "description": "string",
  "classification": "string",
  "specialization": "string",
  "visibility": "string",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="87aec-236">另请参阅</span><span class="sxs-lookup"><span data-stu-id="87aec-236">See also</span></span>

- [<span data-ttu-id="87aec-237">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="87aec-237">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="87aec-238">将 Microsoft Graph API 与 Microsoft Teams 结合使用</span><span class="sxs-lookup"><span data-stu-id="87aec-238">Use the Microsoft Graph API to work with Microsoft Teams</span></span>](teams-api-overview.md)
