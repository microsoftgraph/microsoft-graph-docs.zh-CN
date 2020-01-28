---
title: 团队资源类型
description: 'Microsoft Teams 中的团队是频道的集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 584e7016e74d7aeef8093af8e62e216a8f2870aa
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559052"
---
# <a name="team-resource-type"></a><span data-ttu-id="42e25-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="42e25-103">team resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42e25-104">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="42e25-104">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span> <span data-ttu-id="42e25-105">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="42e25-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="42e25-106">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="42e25-106">Every team is associated with a [group](../resources/group.md).</span></span> <span data-ttu-id="42e25-107">该组具有与团队相同的 ID，例如 `/groups/{id}/team` 与 `/teams/{id}` 相同。</span><span class="sxs-lookup"><span data-stu-id="42e25-107">The group has the same ID as the team - for example, `/groups/{id}/team` is the same as `/teams/{id}`.</span></span> <span data-ttu-id="42e25-108">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="42e25-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="42e25-109">方法</span><span class="sxs-lookup"><span data-stu-id="42e25-109">Methods</span></span>

| <span data-ttu-id="42e25-110">方法</span><span class="sxs-lookup"><span data-stu-id="42e25-110">Method</span></span>       | <span data-ttu-id="42e25-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="42e25-111">Return Type</span></span>  |<span data-ttu-id="42e25-112">说明</span><span class="sxs-lookup"><span data-stu-id="42e25-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42e25-113">创建团队</span><span class="sxs-lookup"><span data-stu-id="42e25-113">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="42e25-114">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="42e25-114">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="42e25-115">从头开始创建团队。</span><span class="sxs-lookup"><span data-stu-id="42e25-115">Create a team from scratch.</span></span> |
|[<span data-ttu-id="42e25-116">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="42e25-116">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="42e25-117">team</span><span class="sxs-lookup"><span data-stu-id="42e25-117">team</span></span>](team.md) | <span data-ttu-id="42e25-118">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="42e25-118">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="42e25-119">获取团队</span><span class="sxs-lookup"><span data-stu-id="42e25-119">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="42e25-120">team</span><span class="sxs-lookup"><span data-stu-id="42e25-120">team</span></span>](team.md) | <span data-ttu-id="42e25-121">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42e25-121">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="42e25-122">更新团队</span><span class="sxs-lookup"><span data-stu-id="42e25-122">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="42e25-123">team</span><span class="sxs-lookup"><span data-stu-id="42e25-123">team</span></span>](team.md) |<span data-ttu-id="42e25-124">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="42e25-124">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="42e25-125">删除团队</span><span class="sxs-lookup"><span data-stu-id="42e25-125">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="42e25-126">无</span><span class="sxs-lookup"><span data-stu-id="42e25-126">None</span></span> |<span data-ttu-id="42e25-127">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="42e25-127">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="42e25-128">克隆团队</span><span class="sxs-lookup"><span data-stu-id="42e25-128">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="42e25-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="42e25-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="42e25-130">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="42e25-130">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="42e25-131">存档团队</span><span class="sxs-lookup"><span data-stu-id="42e25-131">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="42e25-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="42e25-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="42e25-133">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="42e25-133">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="42e25-134">解档团队</span><span class="sxs-lookup"><span data-stu-id="42e25-134">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="42e25-135">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="42e25-135">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="42e25-136">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="42e25-136">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="42e25-137">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="42e25-137">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="42e25-138">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42e25-138">[team](team.md) collection</span></span> | <span data-ttu-id="42e25-139">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="42e25-139">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="42e25-140">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="42e25-140">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="42e25-141">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42e25-141">[group](group.md) collection</span></span> | <span data-ttu-id="42e25-142">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="42e25-142">List all groups that have teams.</span></span> |
|[<span data-ttu-id="42e25-143">获取团队照片</span><span class="sxs-lookup"><span data-stu-id="42e25-143">Get team photo</span></span>](../api/team-get-photo.md) | <span data-ttu-id="42e25-144">二进制数据</span><span class="sxs-lookup"><span data-stu-id="42e25-144">Binary data</span></span> | <span data-ttu-id="42e25-145">获取团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="42e25-145">Get the photo (picture) for a team.</span></span> |
|[<span data-ttu-id="42e25-146">更新团队照片</span><span class="sxs-lookup"><span data-stu-id="42e25-146">Update team photo</span></span>](../api/team-update-photo.md) | <span data-ttu-id="42e25-147">无</span><span class="sxs-lookup"><span data-stu-id="42e25-147">None</span></span> | <span data-ttu-id="42e25-148">更新团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="42e25-148">Update the photo (picture) for a team.</span></span> |

## <a name="properties"></a><span data-ttu-id="42e25-149">属性</span><span class="sxs-lookup"><span data-stu-id="42e25-149">Properties</span></span>

| <span data-ttu-id="42e25-150">属性</span><span class="sxs-lookup"><span data-stu-id="42e25-150">Property</span></span> | <span data-ttu-id="42e25-151">类型</span><span class="sxs-lookup"><span data-stu-id="42e25-151">Type</span></span> | <span data-ttu-id="42e25-152">说明</span><span class="sxs-lookup"><span data-stu-id="42e25-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="42e25-153">displayName</span><span class="sxs-lookup"><span data-stu-id="42e25-153">displayName</span></span>|<span data-ttu-id="42e25-154">string</span><span class="sxs-lookup"><span data-stu-id="42e25-154">string</span></span>| <span data-ttu-id="42e25-155">团队的名称。</span><span class="sxs-lookup"><span data-stu-id="42e25-155">The name of the team.</span></span> |
|<span data-ttu-id="42e25-156">description</span><span class="sxs-lookup"><span data-stu-id="42e25-156">description</span></span>|<span data-ttu-id="42e25-157">string</span><span class="sxs-lookup"><span data-stu-id="42e25-157">string</span></span>| <span data-ttu-id="42e25-158">组的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="42e25-158">An optional description for the team.</span></span> |
|<span data-ttu-id="42e25-159">classification</span><span class="sxs-lookup"><span data-stu-id="42e25-159">classification</span></span>|<span data-ttu-id="42e25-160">string</span><span class="sxs-lookup"><span data-stu-id="42e25-160">string</span></span>| <span data-ttu-id="42e25-161">标签（可选）。</span><span class="sxs-lookup"><span data-stu-id="42e25-161">An optional label.</span></span> <span data-ttu-id="42e25-162">通常说明团队的数据或业务敏感性。</span><span class="sxs-lookup"><span data-stu-id="42e25-162">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="42e25-163">必须与租户目录中的一个预配置集匹配。</span><span class="sxs-lookup"><span data-stu-id="42e25-163">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="42e25-164">specialization</span><span class="sxs-lookup"><span data-stu-id="42e25-164">specialization</span></span>|[<span data-ttu-id="42e25-165">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="42e25-165">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="42e25-166">可选。</span><span class="sxs-lookup"><span data-stu-id="42e25-166">Optional.</span></span> <span data-ttu-id="42e25-167">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="42e25-167">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="42e25-168">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="42e25-168">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="42e25-169">visibility</span><span class="sxs-lookup"><span data-stu-id="42e25-169">visibility</span></span>|[<span data-ttu-id="42e25-170">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="42e25-170">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="42e25-171">组和团队的可见性。</span><span class="sxs-lookup"><span data-stu-id="42e25-171">The visibility of a the group and team.</span></span> <span data-ttu-id="42e25-172">默认值为 Public。</span><span class="sxs-lookup"><span data-stu-id="42e25-172">Defaults to Public.</span></span> |
|<span data-ttu-id="42e25-173">funSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-173">funSettings</span></span>|[<span data-ttu-id="42e25-174">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-174">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="42e25-175">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="42e25-175">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="42e25-176">guestSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-176">guestSettings</span></span>|[<span data-ttu-id="42e25-177">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-177">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="42e25-178">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="42e25-178">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="42e25-179">internalId</span><span class="sxs-lookup"><span data-stu-id="42e25-179">internalId</span></span> | <span data-ttu-id="42e25-180">字符串</span><span class="sxs-lookup"><span data-stu-id="42e25-180">string</span></span> | <span data-ttu-id="42e25-181">已在一些位置（如审核日志/[Office 365 管理活动 API](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="42e25-181">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="42e25-182">isArchived</span><span class="sxs-lookup"><span data-stu-id="42e25-182">isArchived</span></span>|<span data-ttu-id="42e25-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="42e25-183">Boolean</span></span>|<span data-ttu-id="42e25-184">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="42e25-184">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="42e25-185">memberSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-185">memberSettings</span></span>|[<span data-ttu-id="42e25-186">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-186">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="42e25-187">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="42e25-187">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="42e25-188">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-188">messagingSettings</span></span>|[<span data-ttu-id="42e25-189">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-189">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="42e25-190">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="42e25-190">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="42e25-191">discoverySettings</span><span class="sxs-lookup"><span data-stu-id="42e25-191">discoverySettings</span></span>|[<span data-ttu-id="42e25-192">teamDiscoverySettings</span><span class="sxs-lookup"><span data-stu-id="42e25-192">teamDiscoverySettings</span></span>](teamdiscoverysettings.md) |<span data-ttu-id="42e25-193">用于让他人配置团队可发现性的设置。</span><span class="sxs-lookup"><span data-stu-id="42e25-193">Settings to configure team discoverability by others.</span></span>|
|<span data-ttu-id="42e25-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="42e25-194">webUrl</span></span>|<span data-ttu-id="42e25-195">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="42e25-195">string (readonly)</span></span> | <span data-ttu-id="42e25-196">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="42e25-196">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="42e25-197">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="42e25-197">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="42e25-198">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="42e25-198">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="42e25-199">classSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-199">classSettings</span></span>|[<span data-ttu-id="42e25-200">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="42e25-200">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="42e25-201">配置班级设置。</span><span class="sxs-lookup"><span data-stu-id="42e25-201">Configure settings of a class.</span></span> <span data-ttu-id="42e25-202">仅当团队代表班级时可用。</span><span class="sxs-lookup"><span data-stu-id="42e25-202">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42e25-203">关系</span><span class="sxs-lookup"><span data-stu-id="42e25-203">Relationships</span></span>

| <span data-ttu-id="42e25-204">关系</span><span class="sxs-lookup"><span data-stu-id="42e25-204">Relationship</span></span> | <span data-ttu-id="42e25-205">类型</span><span class="sxs-lookup"><span data-stu-id="42e25-205">Type</span></span> | <span data-ttu-id="42e25-206">说明</span><span class="sxs-lookup"><span data-stu-id="42e25-206">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="42e25-207">channels</span><span class="sxs-lookup"><span data-stu-id="42e25-207">channels</span></span>|<span data-ttu-id="42e25-208">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42e25-208">[channel](channel.md) collection</span></span>|<span data-ttu-id="42e25-209">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="42e25-209">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="42e25-210">installedApps</span><span class="sxs-lookup"><span data-stu-id="42e25-210">installedApps</span></span>|<span data-ttu-id="42e25-211">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42e25-211">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="42e25-212">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="42e25-212">The apps installed in this team.</span></span>|
|<span data-ttu-id="42e25-213">owners</span><span class="sxs-lookup"><span data-stu-id="42e25-213">owners</span></span>|[<span data-ttu-id="42e25-214">user</span><span class="sxs-lookup"><span data-stu-id="42e25-214">user</span></span>](user.md)| <span data-ttu-id="42e25-215">此团队的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="42e25-215">The list of this team's owners.</span></span> <span data-ttu-id="42e25-216">目前，在使用应用程序权限创建团队时，必须指定一个所有者。</span><span class="sxs-lookup"><span data-stu-id="42e25-216">Currently, when creating a team using application permissions, exactly one owner must be specified.</span></span> <span data-ttu-id="42e25-217">当使用用户委派的权限时，不能指定任何所有者（当前用户是所有者）。</span><span class="sxs-lookup"><span data-stu-id="42e25-217">When using user delegated permissions, no owner can be specified (the current user is the owner).</span></span> <span data-ttu-id="42e25-218">必须将所有者指定为对象 ID (GUID)，而不是 UPN。</span><span class="sxs-lookup"><span data-stu-id="42e25-218">Owner must be specified as an object ID (GUID), not a UPN.</span></span> |
|<span data-ttu-id="42e25-219">operations</span><span class="sxs-lookup"><span data-stu-id="42e25-219">operations</span></span>|<span data-ttu-id="42e25-220">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42e25-220">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="42e25-221">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="42e25-221">The async operations that ran or are running on this team.</span></span> | 
|<span data-ttu-id="42e25-222">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="42e25-222">primaryChannel</span></span>|[<span data-ttu-id="42e25-223">频道</span><span class="sxs-lookup"><span data-stu-id="42e25-223">channel</span></span>](channel.md)| <span data-ttu-id="42e25-224">团队的常规频道。</span><span class="sxs-lookup"><span data-stu-id="42e25-224">The general channel for the team.</span></span> | 
|<span data-ttu-id="42e25-225">schedule</span><span class="sxs-lookup"><span data-stu-id="42e25-225">schedule</span></span>|[<span data-ttu-id="42e25-226">日程安排</span><span class="sxs-lookup"><span data-stu-id="42e25-226">schedule</span></span>](schedule.md)| <span data-ttu-id="42e25-227">此团队的排班安排。</span><span class="sxs-lookup"><span data-stu-id="42e25-227">The schedule of shifts for this team.</span></span>|
|<span data-ttu-id="42e25-228">template</span><span class="sxs-lookup"><span data-stu-id="42e25-228">template</span></span>|[<span data-ttu-id="42e25-229">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="42e25-229">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="42e25-230">创建此团队时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="42e25-230">The template this team was created from.</span></span> <span data-ttu-id="42e25-231">请参阅[可用模板](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="42e25-231">See [available templates](https://docs.microsoft.com/MicrosoftTeams/get-started-with-teams-templates).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42e25-232">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42e25-232">JSON representation</span></span>

<span data-ttu-id="42e25-233">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42e25-233">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="42e25-234">**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。</span><span class="sxs-lookup"><span data-stu-id="42e25-234">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="42e25-235">另请参阅</span><span class="sxs-lookup"><span data-stu-id="42e25-235">See Also</span></span>

- [<span data-ttu-id="42e25-236">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="42e25-236">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="42e25-237">Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="42e25-237">Teams API Overview</span></span>](teams-api-overview.md)
