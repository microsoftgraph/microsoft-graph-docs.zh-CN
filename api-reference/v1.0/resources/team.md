---
title: 团队资源类型
description: 'Microsoft Teams 中的团队是频道的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7c3dd42c25ce8c48722ab857f61e0c6a9a275581
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964134"
---
# <a name="team-resource-type"></a><span data-ttu-id="b8968-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="b8968-103">team resource type</span></span>



<span data-ttu-id="b8968-104">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b8968-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="b8968-105">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="b8968-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="b8968-106">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="b8968-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="b8968-107">该组具有与团队相同的 ID，例如 /groups/{id}/team 与 /teams/{id} 相同。</span><span class="sxs-lookup"><span data-stu-id="b8968-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="b8968-108">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="b8968-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b8968-109">方法</span><span class="sxs-lookup"><span data-stu-id="b8968-109">Methods</span></span>

| <span data-ttu-id="b8968-110">方法</span><span class="sxs-lookup"><span data-stu-id="b8968-110">Method</span></span>       | <span data-ttu-id="b8968-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8968-111">Return Type</span></span>  |<span data-ttu-id="b8968-112">说明</span><span class="sxs-lookup"><span data-stu-id="b8968-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8968-113">创建团队</span><span class="sxs-lookup"><span data-stu-id="b8968-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="b8968-114">团队</span><span class="sxs-lookup"><span data-stu-id="b8968-114">team</span></span>](team.md) | <span data-ttu-id="b8968-115">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="b8968-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="b8968-116">获取团队</span><span class="sxs-lookup"><span data-stu-id="b8968-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="b8968-117">team</span><span class="sxs-lookup"><span data-stu-id="b8968-117">team</span></span>](team.md) | <span data-ttu-id="b8968-118">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8968-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="b8968-119">更新团队</span><span class="sxs-lookup"><span data-stu-id="b8968-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="b8968-120">team</span><span class="sxs-lookup"><span data-stu-id="b8968-120">team</span></span>](team.md) |<span data-ttu-id="b8968-121">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="b8968-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="b8968-122">删除团队</span><span class="sxs-lookup"><span data-stu-id="b8968-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="b8968-123">无</span><span class="sxs-lookup"><span data-stu-id="b8968-123">None</span></span> |<span data-ttu-id="b8968-124">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="b8968-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="b8968-125">克隆团队</span><span class="sxs-lookup"><span data-stu-id="b8968-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="b8968-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="b8968-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="b8968-127">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="b8968-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="b8968-128">存档团队</span><span class="sxs-lookup"><span data-stu-id="b8968-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="b8968-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="b8968-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="b8968-130">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="b8968-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="b8968-131">解档团队</span><span class="sxs-lookup"><span data-stu-id="b8968-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="b8968-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="b8968-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="b8968-133">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="b8968-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="b8968-134">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="b8968-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="b8968-135">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8968-135">[team](team.md) collection</span></span> | <span data-ttu-id="b8968-136">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="b8968-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="b8968-137">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="b8968-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="b8968-138">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8968-138">[group](group.md) collection</span></span> | <span data-ttu-id="b8968-139">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="b8968-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="b8968-140">将应用发布到你的组织</span><span class="sxs-lookup"><span data-stu-id="b8968-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="b8968-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b8968-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="b8968-142">创建仅对你的组织可见的 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="b8968-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="b8968-143">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="b8968-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="b8968-144">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b8968-144">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="b8968-145">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="b8968-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="b8968-146">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="b8968-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="b8968-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b8968-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="b8968-148">将选项卡添加（安装）到团队的频道。</span><span class="sxs-lookup"><span data-stu-id="b8968-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8968-149">属性</span><span class="sxs-lookup"><span data-stu-id="b8968-149">Properties</span></span>

| <span data-ttu-id="b8968-150">属性</span><span class="sxs-lookup"><span data-stu-id="b8968-150">Property</span></span> | <span data-ttu-id="b8968-151">类型</span><span class="sxs-lookup"><span data-stu-id="b8968-151">Type</span></span>   | <span data-ttu-id="b8968-152">说明</span><span class="sxs-lookup"><span data-stu-id="b8968-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b8968-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-153">funSettings</span></span>|[<span data-ttu-id="b8968-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="b8968-155">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="b8968-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="b8968-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-156">guestSettings</span></span>|[<span data-ttu-id="b8968-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="b8968-158">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="b8968-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="b8968-159">internalId</span><span class="sxs-lookup"><span data-stu-id="b8968-159">internalId</span></span> | <span data-ttu-id="b8968-160">字符串</span><span class="sxs-lookup"><span data-stu-id="b8968-160">string</span></span> | <span data-ttu-id="b8968-161">已在一些位置（如审核日志/[Office 365 管理活动 API](https://docs.microsoft.com/zh-CN/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b8968-161">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](https://docs.microsoft.com/zh-CN/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="b8968-162">isArchived</span><span class="sxs-lookup"><span data-stu-id="b8968-162">isArchived</span></span>|<span data-ttu-id="b8968-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8968-163">Boolean</span></span>|<span data-ttu-id="b8968-164">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="b8968-164">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="b8968-165">memberSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-165">memberSettings</span></span>|[<span data-ttu-id="b8968-166">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-166">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="b8968-167">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="b8968-167">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="b8968-168">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-168">messagingSettings</span></span>|[<span data-ttu-id="b8968-169">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="b8968-169">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="b8968-170">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="b8968-170">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="b8968-171">webUrl</span><span class="sxs-lookup"><span data-stu-id="b8968-171">webUrl</span></span>|<span data-ttu-id="b8968-172">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="b8968-172">string (readonly)</span></span> | <span data-ttu-id="b8968-173">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="b8968-173">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="b8968-174">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="b8968-174">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="b8968-175">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="b8968-175">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b8968-176">关系</span><span class="sxs-lookup"><span data-stu-id="b8968-176">Relationships</span></span>

| <span data-ttu-id="b8968-177">关系</span><span class="sxs-lookup"><span data-stu-id="b8968-177">Relationship</span></span> | <span data-ttu-id="b8968-178">类型</span><span class="sxs-lookup"><span data-stu-id="b8968-178">Type</span></span>   | <span data-ttu-id="b8968-179">说明</span><span class="sxs-lookup"><span data-stu-id="b8968-179">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b8968-180">channels</span><span class="sxs-lookup"><span data-stu-id="b8968-180">channels</span></span>|<span data-ttu-id="b8968-181">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8968-181">[channel](channel.md) collection</span></span>|<span data-ttu-id="b8968-182">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="b8968-182">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="b8968-183">installedApps</span><span class="sxs-lookup"><span data-stu-id="b8968-183">installedApps</span></span>|<span data-ttu-id="b8968-184">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8968-184">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="b8968-185">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="b8968-185">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8968-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8968-186">JSON representation</span></span>

<span data-ttu-id="b8968-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8968-187">The following is a JSON representation of the resource.</span></span>

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
  "internalId": "19:...big.number...@thread.skype",
  "isArchived": false,
  "webUrl": "https://...longUrl..."
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

## <a name="see-also"></a><span data-ttu-id="b8968-188">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b8968-188">See Also</span></span>
- [<span data-ttu-id="b8968-189">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="b8968-189">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="b8968-190">使用 Teams API</span><span class="sxs-lookup"><span data-stu-id="b8968-190">Using Teams APIs</span></span>](teams-api-overview.md)
