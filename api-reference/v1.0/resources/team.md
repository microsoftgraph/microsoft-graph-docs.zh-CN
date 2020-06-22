---
title: 团队资源类型
description: 'Microsoft Teams 中的团队是频道的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 460bbfaa522cf4767d7f35992a4371bf870c8948
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793680"
---
# <a name="team-resource-type"></a><span data-ttu-id="c79ca-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="c79ca-103">team resource type</span></span>

<span data-ttu-id="c79ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c79ca-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="c79ca-105">Microsoft Teams 中的团队是 [channel](channel.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c79ca-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="c79ca-106">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="c79ca-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="c79ca-107">每个团队与一个[组](../resources/group.md)相关联。</span><span class="sxs-lookup"><span data-stu-id="c79ca-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="c79ca-108">该组具有与团队相同的 ID，例如 /groups/{id}/team 与 /teams/{id} 相同。</span><span class="sxs-lookup"><span data-stu-id="c79ca-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="c79ca-109">有关使用组和团队内部成员的详细信息，请参阅[使用 Microsoft Graph REST API 来处理 Microsoft Teams](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="c79ca-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c79ca-110">方法</span><span class="sxs-lookup"><span data-stu-id="c79ca-110">Methods</span></span>

| <span data-ttu-id="c79ca-111">方法</span><span class="sxs-lookup"><span data-stu-id="c79ca-111">Method</span></span>       | <span data-ttu-id="c79ca-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c79ca-112">Return Type</span></span>  |<span data-ttu-id="c79ca-113">说明</span><span class="sxs-lookup"><span data-stu-id="c79ca-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c79ca-114">创建团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-114">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="c79ca-115">团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-115">team</span></span>](team.md) | <span data-ttu-id="c79ca-116">创建新的团队，或向现有组添加团队。</span><span class="sxs-lookup"><span data-stu-id="c79ca-116">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="c79ca-117">获取团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-117">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="c79ca-118">team</span><span class="sxs-lookup"><span data-stu-id="c79ca-118">team</span></span>](team.md) | <span data-ttu-id="c79ca-119">检索指定团队的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c79ca-119">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="c79ca-120">更新团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-120">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="c79ca-121">team</span><span class="sxs-lookup"><span data-stu-id="c79ca-121">team</span></span>](team.md) |<span data-ttu-id="c79ca-122">更新指定团队的属性。</span><span class="sxs-lookup"><span data-stu-id="c79ca-122">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="c79ca-123">删除团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-123">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="c79ca-124">无</span><span class="sxs-lookup"><span data-stu-id="c79ca-124">None</span></span> |<span data-ttu-id="c79ca-125">删除团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="c79ca-125">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="c79ca-126">克隆团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-126">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="c79ca-127">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c79ca-127">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="c79ca-128">复制团队及其关联的组。</span><span class="sxs-lookup"><span data-stu-id="c79ca-128">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="c79ca-129">存档团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-129">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="c79ca-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c79ca-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="c79ca-131">将团队置于只读状态。</span><span class="sxs-lookup"><span data-stu-id="c79ca-131">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="c79ca-132">解档团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-132">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="c79ca-133">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c79ca-133">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="c79ca-134">将团队还原到读写状态。</span><span class="sxs-lookup"><span data-stu-id="c79ca-134">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="c79ca-135">列出你的团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-135">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="c79ca-136">[team](team.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c79ca-136">[team](team.md) collection</span></span> | <span data-ttu-id="c79ca-137">列出你属于的团队。</span><span class="sxs-lookup"><span data-stu-id="c79ca-137">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="c79ca-138">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-138">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="c79ca-139">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c79ca-139">[group](group.md) collection</span></span> | <span data-ttu-id="c79ca-140">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="c79ca-140">List all groups that have teams.</span></span> |
|[<span data-ttu-id="c79ca-141">将应用发布到你的组织</span><span class="sxs-lookup"><span data-stu-id="c79ca-141">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="c79ca-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c79ca-142">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="c79ca-143">创建仅对你的组织可见的 Teams 应用。</span><span class="sxs-lookup"><span data-stu-id="c79ca-143">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="c79ca-144">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="c79ca-144">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="c79ca-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c79ca-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="c79ca-146">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="c79ca-146">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="c79ca-147">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="c79ca-147">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="c79ca-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c79ca-148">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="c79ca-149">将选项卡添加（安装）到团队的频道。</span><span class="sxs-lookup"><span data-stu-id="c79ca-149">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c79ca-150">属性</span><span class="sxs-lookup"><span data-stu-id="c79ca-150">Properties</span></span>

| <span data-ttu-id="c79ca-151">属性</span><span class="sxs-lookup"><span data-stu-id="c79ca-151">Property</span></span> | <span data-ttu-id="c79ca-152">类型</span><span class="sxs-lookup"><span data-stu-id="c79ca-152">Type</span></span>   | <span data-ttu-id="c79ca-153">说明</span><span class="sxs-lookup"><span data-stu-id="c79ca-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c79ca-154">funSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-154">funSettings</span></span>|[<span data-ttu-id="c79ca-155">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-155">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="c79ca-156">用于配置团队中 Giphy、成员和贴纸使用情况的设置。</span><span class="sxs-lookup"><span data-stu-id="c79ca-156">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="c79ca-157">guestSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-157">guestSettings</span></span>|[<span data-ttu-id="c79ca-158">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-158">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="c79ca-159">用于配置来宾是否可以在团队中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="c79ca-159">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="c79ca-160">internalId</span><span class="sxs-lookup"><span data-stu-id="c79ca-160">internalId</span></span> | <span data-ttu-id="c79ca-161">字符串</span><span class="sxs-lookup"><span data-stu-id="c79ca-161">string</span></span> | <span data-ttu-id="c79ca-162">已在一些位置（如审核日志/[Office 365 管理活动 API](/office/office-365-management-api/office-365-management-activity-api-reference)）使用的团队唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="c79ca-162">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="c79ca-163">isArchived</span><span class="sxs-lookup"><span data-stu-id="c79ca-163">isArchived</span></span>|<span data-ttu-id="c79ca-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="c79ca-164">Boolean</span></span>|<span data-ttu-id="c79ca-165">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="c79ca-165">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="c79ca-166">memberSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-166">memberSettings</span></span>|[<span data-ttu-id="c79ca-167">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-167">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="c79ca-168">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="c79ca-168">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="c79ca-169">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-169">messagingSettings</span></span>|[<span data-ttu-id="c79ca-170">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-170">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="c79ca-171">用于配置团队中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="c79ca-171">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="c79ca-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="c79ca-172">webUrl</span></span>|<span data-ttu-id="c79ca-173">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="c79ca-173">string (readonly)</span></span> | <span data-ttu-id="c79ca-174">用于转到 Microsoft Teams 客户端中团队的超链接。</span><span class="sxs-lookup"><span data-stu-id="c79ca-174">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="c79ca-175">这是在 Microsoft Teams 客户端中右键单击团队并选择**获取团队链接**时获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="c79ca-175">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="c79ca-176">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="c79ca-176">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="c79ca-177">classSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-177">classSettings</span></span>|[<span data-ttu-id="c79ca-178">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="c79ca-178">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="c79ca-179">配置班级设置。</span><span class="sxs-lookup"><span data-stu-id="c79ca-179">Configure settings of a class.</span></span> <span data-ttu-id="c79ca-180">仅当团队代表班级时可用。</span><span class="sxs-lookup"><span data-stu-id="c79ca-180">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c79ca-181">关系</span><span class="sxs-lookup"><span data-stu-id="c79ca-181">Relationships</span></span>

| <span data-ttu-id="c79ca-182">关系</span><span class="sxs-lookup"><span data-stu-id="c79ca-182">Relationship</span></span> | <span data-ttu-id="c79ca-183">类型</span><span class="sxs-lookup"><span data-stu-id="c79ca-183">Type</span></span>   | <span data-ttu-id="c79ca-184">说明</span><span class="sxs-lookup"><span data-stu-id="c79ca-184">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c79ca-185">channels</span><span class="sxs-lookup"><span data-stu-id="c79ca-185">channels</span></span>|<span data-ttu-id="c79ca-186">[channel](channel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c79ca-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="c79ca-187">与团队相关的频道和消息的集合。</span><span class="sxs-lookup"><span data-stu-id="c79ca-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="c79ca-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="c79ca-188">installedApps</span></span>|<span data-ttu-id="c79ca-189">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c79ca-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="c79ca-190">此团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="c79ca-190">The apps installed in this team.</span></span>|
|[<span data-ttu-id="c79ca-191">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="c79ca-191">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="c79ca-192">频道</span><span class="sxs-lookup"><span data-stu-id="c79ca-192">channel</span></span>](channel.md)| <span data-ttu-id="c79ca-193">团队的常规频道。</span><span class="sxs-lookup"><span data-stu-id="c79ca-193">The general channel for the team.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="c79ca-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c79ca-194">JSON representation</span></span>

<span data-ttu-id="c79ca-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c79ca-195">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="c79ca-196">**注意：** 如果团队属于班级类型，则会在团队上应用 **classSettings** 属性。</span><span class="sxs-lookup"><span data-stu-id="c79ca-196">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c79ca-197">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c79ca-197">See Also</span></span>
- [<span data-ttu-id="c79ca-198">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="c79ca-198">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="c79ca-199">使用 Teams API</span><span class="sxs-lookup"><span data-stu-id="c79ca-199">Using Teams APIs</span></span>](teams-api-overview.md)
