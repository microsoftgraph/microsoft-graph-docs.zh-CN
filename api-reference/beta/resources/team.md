---
title: 团队资源类型
description: 'Microsoft Teams 中的团队是频道的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6ed8b298336563d2b07ce2d6a83b90c9400fe53f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643774"
---
# <a name="team-resource-type"></a><span data-ttu-id="22bb8-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="22bb8-103">team resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22bb8-104">Microsoft Teams 中的团队是[频道](channel.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="22bb8-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="22bb8-105">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="22bb8-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="22bb8-106">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="22bb8-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="22bb8-107">该组具有与团队相同的 ID，例如 /groups/{id}/team 与 /teams/{id} 相同。</span><span class="sxs-lookup"><span data-stu-id="22bb8-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="22bb8-108">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="22bb8-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="22bb8-109">方法</span><span class="sxs-lookup"><span data-stu-id="22bb8-109">Methods</span></span>

| <span data-ttu-id="22bb8-110">方法</span><span class="sxs-lookup"><span data-stu-id="22bb8-110">Method</span></span>       | <span data-ttu-id="22bb8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="22bb8-111">Return Type</span></span>  |<span data-ttu-id="22bb8-112">说明</span><span class="sxs-lookup"><span data-stu-id="22bb8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22bb8-113">创建团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-113">Create team</span></span>](../api/team-post.md) | [<span data-ttu-id="22bb8-114">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="22bb8-114">teamsAsyncOperation</span></span>](teamsasyncoperation.md) | <span data-ttu-id="22bb8-115">从头开始创建团队。</span><span class="sxs-lookup"><span data-stu-id="22bb8-115">Create a team from scratch.</span></span> |
|[<span data-ttu-id="22bb8-116">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-116">Create team from group</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="22bb8-117">team</span><span class="sxs-lookup"><span data-stu-id="22bb8-117">team</span></span>](team.md) | <span data-ttu-id="22bb8-118">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="22bb8-118">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="22bb8-119">获取团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-119">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="22bb8-120">team</span><span class="sxs-lookup"><span data-stu-id="22bb8-120">team</span></span>](team.md) | <span data-ttu-id="22bb8-121">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22bb8-121">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="22bb8-122">更新团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-122">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="22bb8-123">team</span><span class="sxs-lookup"><span data-stu-id="22bb8-123">team</span></span>](team.md) |<span data-ttu-id="22bb8-124">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="22bb8-124">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="22bb8-125">删除团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-125">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="22bb8-126">无</span><span class="sxs-lookup"><span data-stu-id="22bb8-126">None</span></span> |<span data-ttu-id="22bb8-127">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="22bb8-127">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="22bb8-128">克隆团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-128">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="22bb8-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="22bb8-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="22bb8-130">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="22bb8-130">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="22bb8-131">存档团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-131">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="22bb8-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="22bb8-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="22bb8-133">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="22bb8-133">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="22bb8-134">解档团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-134">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="22bb8-135">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="22bb8-135">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="22bb8-136">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="22bb8-136">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="22bb8-137">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-137">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="22bb8-138">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bb8-138">[team](team.md) collection</span></span> | <span data-ttu-id="22bb8-139">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="22bb8-139">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="22bb8-140">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-140">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="22bb8-141">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bb8-141">[group](group.md) collection</span></span> | <span data-ttu-id="22bb8-142">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="22bb8-142">List all groups that have teams.</span></span> |
|[<span data-ttu-id="22bb8-143">将应用发布到你的组织</span><span class="sxs-lookup"><span data-stu-id="22bb8-143">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="22bb8-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="22bb8-144">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="22bb8-145">创建仅对你的组织可见的 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="22bb8-145">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="22bb8-146">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="22bb8-146">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="22bb8-147">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="22bb8-147">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="22bb8-148">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="22bb8-148">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="22bb8-149">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="22bb8-149">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="22bb8-150">teamsTab</span><span class="sxs-lookup"><span data-stu-id="22bb8-150">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="22bb8-151">将选项卡添加（安装）到团队的频道。</span><span class="sxs-lookup"><span data-stu-id="22bb8-151">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="22bb8-152">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="22bb8-152">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="22bb8-153">chatMessage</span><span class="sxs-lookup"><span data-stu-id="22bb8-153">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="22bb8-154">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="22bb8-154">Get messages in a channel</span></span>](../api/channel-list-messages.md) |

## <a name="properties"></a><span data-ttu-id="22bb8-155">属性</span><span class="sxs-lookup"><span data-stu-id="22bb8-155">Properties</span></span>

| <span data-ttu-id="22bb8-156">属性</span><span class="sxs-lookup"><span data-stu-id="22bb8-156">Property</span></span> | <span data-ttu-id="22bb8-157">类型</span><span class="sxs-lookup"><span data-stu-id="22bb8-157">Type</span></span>   | <span data-ttu-id="22bb8-158">说明</span><span class="sxs-lookup"><span data-stu-id="22bb8-158">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="22bb8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="22bb8-159">displayName</span></span>|<span data-ttu-id="22bb8-160">string</span><span class="sxs-lookup"><span data-stu-id="22bb8-160">string</span></span>| <span data-ttu-id="22bb8-161">团队的名称。</span><span class="sxs-lookup"><span data-stu-id="22bb8-161">The name of the team.</span></span> |
|<span data-ttu-id="22bb8-162">description</span><span class="sxs-lookup"><span data-stu-id="22bb8-162">description</span></span>|<span data-ttu-id="22bb8-163">string</span><span class="sxs-lookup"><span data-stu-id="22bb8-163">string</span></span>| <span data-ttu-id="22bb8-164">组的说明（可选）。</span><span class="sxs-lookup"><span data-stu-id="22bb8-164">An optional description for the team.</span></span> |
|<span data-ttu-id="22bb8-165">classification</span><span class="sxs-lookup"><span data-stu-id="22bb8-165">classification</span></span>|<span data-ttu-id="22bb8-166">string</span><span class="sxs-lookup"><span data-stu-id="22bb8-166">string</span></span>| <span data-ttu-id="22bb8-167">标签（可选）。</span><span class="sxs-lookup"><span data-stu-id="22bb8-167">An optional label.</span></span> <span data-ttu-id="22bb8-168">通常说明团队的数据或业务敏感性。</span><span class="sxs-lookup"><span data-stu-id="22bb8-168">Typically describes the data or business sensitivity of the team.</span></span> <span data-ttu-id="22bb8-169">必须与租户目录中的一个预配置集匹配。</span><span class="sxs-lookup"><span data-stu-id="22bb8-169">Must match one of a pre-configured set in the tenant's directory.</span></span> |
|<span data-ttu-id="22bb8-170">specialization</span><span class="sxs-lookup"><span data-stu-id="22bb8-170">specialization</span></span>|[<span data-ttu-id="22bb8-171">teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="22bb8-171">teamSpecialization</span></span>](teamspecialization.md)| <span data-ttu-id="22bb8-172">可选。</span><span class="sxs-lookup"><span data-stu-id="22bb8-172">Optional.</span></span> <span data-ttu-id="22bb8-173">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="22bb8-173">Indicates whether the team is intended for a particular use case.</span></span>  <span data-ttu-id="22bb8-174">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="22bb8-174">Each team specialization has access to unique behaviors and experiences targeted to its use case.</span></span> |
|<span data-ttu-id="22bb8-175">visibility</span><span class="sxs-lookup"><span data-stu-id="22bb8-175">visibility</span></span>|[<span data-ttu-id="22bb8-176">teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="22bb8-176">teamVisibilityType</span></span>](teamvisibilitytype.md)| <span data-ttu-id="22bb8-177">组和团队的可见性。</span><span class="sxs-lookup"><span data-stu-id="22bb8-177">The visibility of a the group and team.</span></span> <span data-ttu-id="22bb8-178">默认值为 Public。</span><span class="sxs-lookup"><span data-stu-id="22bb8-178">Defaults to Public.</span></span> |
|<span data-ttu-id="22bb8-179">funSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-179">funSettings</span></span>|[<span data-ttu-id="22bb8-180">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-180">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="22bb8-181">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="22bb8-181">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="22bb8-182">guestSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-182">guestSettings</span></span>|[<span data-ttu-id="22bb8-183">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-183">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="22bb8-184">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="22bb8-184">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="22bb8-185">isArchived</span><span class="sxs-lookup"><span data-stu-id="22bb8-185">isArchived</span></span>|<span data-ttu-id="22bb8-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="22bb8-186">Boolean</span></span>|<span data-ttu-id="22bb8-187">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="22bb8-187">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="22bb8-188">memberSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-188">memberSettings</span></span>|[<span data-ttu-id="22bb8-189">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-189">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="22bb8-190">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="22bb8-190">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="22bb8-191">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-191">messagingSettings</span></span>|[<span data-ttu-id="22bb8-192">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="22bb8-192">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="22bb8-193">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="22bb8-193">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="22bb8-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="22bb8-194">webUrl</span></span>|<span data-ttu-id="22bb8-195">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="22bb8-195">string (readonly)</span></span> | <span data-ttu-id="22bb8-196">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="22bb8-196">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="22bb8-197">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="22bb8-197">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="22bb8-198">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="22bb8-198">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="22bb8-199">关系</span><span class="sxs-lookup"><span data-stu-id="22bb8-199">Relationships</span></span>

| <span data-ttu-id="22bb8-200">关系</span><span class="sxs-lookup"><span data-stu-id="22bb8-200">Relationship</span></span> | <span data-ttu-id="22bb8-201">类型</span><span class="sxs-lookup"><span data-stu-id="22bb8-201">Type</span></span>   | <span data-ttu-id="22bb8-202">说明</span><span class="sxs-lookup"><span data-stu-id="22bb8-202">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="22bb8-203">apps</span><span class="sxs-lookup"><span data-stu-id="22bb8-203">apps</span></span>|<span data-ttu-id="22bb8-204">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bb8-204">[teamsApp](teamsapp.md) collection</span></span>| <span data-ttu-id="22bb8-205">（已过时）此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="22bb8-205">(Obsolete) The apps installed in this team.</span></span>|
|<span data-ttu-id="22bb8-206">channels</span><span class="sxs-lookup"><span data-stu-id="22bb8-206">channels</span></span>|<span data-ttu-id="22bb8-207">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bb8-207">[channel](channel.md) collection</span></span>|<span data-ttu-id="22bb8-208">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="22bb8-208">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="22bb8-209">installedApps</span><span class="sxs-lookup"><span data-stu-id="22bb8-209">installedApps</span></span>|<span data-ttu-id="22bb8-210">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bb8-210">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="22bb8-211">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="22bb8-211">The apps installed in this team.</span></span>|
|<span data-ttu-id="22bb8-212">owners</span><span class="sxs-lookup"><span data-stu-id="22bb8-212">owners</span></span>|[<span data-ttu-id="22bb8-213">user</span><span class="sxs-lookup"><span data-stu-id="22bb8-213">user</span></span>](user.md)| <span data-ttu-id="22bb8-214">此团队的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="22bb8-214">The list of this team's owners.</span></span> |
|<span data-ttu-id="22bb8-215">operations</span><span class="sxs-lookup"><span data-stu-id="22bb8-215">operations</span></span>|<span data-ttu-id="22bb8-216">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bb8-216">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="22bb8-217">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="22bb8-217">The async operations that ran or are running on this team.</span></span> | 
|<span data-ttu-id="22bb8-218">template</span><span class="sxs-lookup"><span data-stu-id="22bb8-218">template</span></span>|[<span data-ttu-id="22bb8-219">teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="22bb8-219">teamsTemplate</span></span>](teamstemplate.md)| <span data-ttu-id="22bb8-220">创建此团队时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="22bb8-220">The template this team was created from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="22bb8-221">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22bb8-221">JSON representation</span></span>

<span data-ttu-id="22bb8-222">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22bb8-222">The following is a JSON representation of the resource.</span></span>

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
  "isArchived": false,
  "webUrl": "https://...longUrl..."
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
  "suppressions": [
    "Error: /api-reference/beta/resources/team.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="22bb8-223">另请参阅</span><span class="sxs-lookup"><span data-stu-id="22bb8-223">See Also</span></span>
- [<span data-ttu-id="22bb8-224">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="22bb8-224">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="22bb8-225">Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="22bb8-225">Teams API Overview</span></span>](teams-api-overview.md)
