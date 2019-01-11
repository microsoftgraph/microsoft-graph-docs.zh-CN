---
title: 团队资源类型
description: '团队中的 Microsoft 团队是通道的集合。 '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 85694e18771ac17873f97cedf68d074ee550f787
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878545"
---
# <a name="team-resource-type"></a><span data-ttu-id="dba8a-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="dba8a-103">team resource type</span></span>



<span data-ttu-id="dba8a-104">团队中的 Microsoft 团队是[通道](channel.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="dba8a-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="dba8a-105">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="dba8a-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="dba8a-106">每个团队是与[组](../resources/group.md)关联。</span><span class="sxs-lookup"><span data-stu-id="dba8a-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="dba8a-107">组具有相同的 ID 团队-例如，/groups/ {id} / 球队是 /teams/ {id} 相同。</span><span class="sxs-lookup"><span data-stu-id="dba8a-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="dba8a-108">有关使用组和团队中的成员的详细信息，请参阅[使用 Microsoft Graph REST API 以使用 Microsoft 团队](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="dba8a-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dba8a-109">方法</span><span class="sxs-lookup"><span data-stu-id="dba8a-109">Methods</span></span>

| <span data-ttu-id="dba8a-110">方法</span><span class="sxs-lookup"><span data-stu-id="dba8a-110">Method</span></span>       | <span data-ttu-id="dba8a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="dba8a-111">Return Type</span></span>  |<span data-ttu-id="dba8a-112">说明</span><span class="sxs-lookup"><span data-stu-id="dba8a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dba8a-113">创建工作组</span><span class="sxs-lookup"><span data-stu-id="dba8a-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="dba8a-114">团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-114">team</span></span>](team.md) | <span data-ttu-id="dba8a-115">创建一个新的团队，或添加到现有组的团队。</span><span class="sxs-lookup"><span data-stu-id="dba8a-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="dba8a-116">获取工作组</span><span class="sxs-lookup"><span data-stu-id="dba8a-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="dba8a-117">团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-117">team</span></span>](team.md) | <span data-ttu-id="dba8a-118">检索的属性和指定团队的关系。</span><span class="sxs-lookup"><span data-stu-id="dba8a-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="dba8a-119">更新团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="dba8a-120">团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-120">team</span></span>](team.md) |<span data-ttu-id="dba8a-121">更新指定的团队的属性。</span><span class="sxs-lookup"><span data-stu-id="dba8a-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="dba8a-122">删除团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="dba8a-123">无</span><span class="sxs-lookup"><span data-stu-id="dba8a-123">None</span></span> |<span data-ttu-id="dba8a-124">删除团队和其关联的组。</span><span class="sxs-lookup"><span data-stu-id="dba8a-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="dba8a-125">克隆团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="dba8a-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="dba8a-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="dba8a-127">复制团队和其关联的组。</span><span class="sxs-lookup"><span data-stu-id="dba8a-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="dba8a-128">存档团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="dba8a-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="dba8a-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="dba8a-130">将团队放在只读状态。</span><span class="sxs-lookup"><span data-stu-id="dba8a-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="dba8a-131">Unarchive 团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="dba8a-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="dba8a-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="dba8a-133">还原到读写状态团队。</span><span class="sxs-lookup"><span data-stu-id="dba8a-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="dba8a-134">列出您的团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="dba8a-135">[团队](team.md)集合</span><span class="sxs-lookup"><span data-stu-id="dba8a-135">[team](team.md) collection</span></span> | <span data-ttu-id="dba8a-136">列出您是成员的团队。</span><span class="sxs-lookup"><span data-stu-id="dba8a-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="dba8a-137">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="dba8a-138">[组](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dba8a-138">[group](group.md) collection</span></span> | <span data-ttu-id="dba8a-139">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="dba8a-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="dba8a-140">将应用程序发布到您的组织</span><span class="sxs-lookup"><span data-stu-id="dba8a-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="dba8a-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dba8a-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="dba8a-142">创建团队应用程序仅对您的组织可见。</span><span class="sxs-lookup"><span data-stu-id="dba8a-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="dba8a-143">将应用程序添加到团队</span><span class="sxs-lookup"><span data-stu-id="dba8a-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="dba8a-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="dba8a-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="dba8a-145">将 （安装） 添加到团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="dba8a-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="dba8a-146">选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="dba8a-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="dba8a-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dba8a-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="dba8a-148">将 （安装） 添加到团队的通道选项卡。</span><span class="sxs-lookup"><span data-stu-id="dba8a-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="dba8a-149">属性</span><span class="sxs-lookup"><span data-stu-id="dba8a-149">Properties</span></span>

| <span data-ttu-id="dba8a-150">属性</span><span class="sxs-lookup"><span data-stu-id="dba8a-150">Property</span></span> | <span data-ttu-id="dba8a-151">类型</span><span class="sxs-lookup"><span data-stu-id="dba8a-151">Type</span></span>   | <span data-ttu-id="dba8a-152">Description</span><span class="sxs-lookup"><span data-stu-id="dba8a-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dba8a-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-153">funSettings</span></span>|[<span data-ttu-id="dba8a-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="dba8a-155">要配置的团队中的使用 Giphy、 memes 和标签的设置。</span><span class="sxs-lookup"><span data-stu-id="dba8a-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="dba8a-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-156">guestSettings</span></span>|[<span data-ttu-id="dba8a-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="dba8a-158">要配置的是否来宾可以创建、 更新或删除通道团队中的设置。</span><span class="sxs-lookup"><span data-stu-id="dba8a-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="dba8a-159">isArchived</span><span class="sxs-lookup"><span data-stu-id="dba8a-159">isArchived</span></span>|<span data-ttu-id="dba8a-160">布尔</span><span class="sxs-lookup"><span data-stu-id="dba8a-160">Boolean</span></span>|<span data-ttu-id="dba8a-161">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="dba8a-161">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="dba8a-162">memberSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-162">memberSettings</span></span>|[<span data-ttu-id="dba8a-163">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-163">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="dba8a-164">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。</span><span class="sxs-lookup"><span data-stu-id="dba8a-164">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="dba8a-165">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-165">messagingSettings</span></span>|[<span data-ttu-id="dba8a-166">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="dba8a-166">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="dba8a-167">要配置的消息设置和团队中的提及。</span><span class="sxs-lookup"><span data-stu-id="dba8a-167">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="dba8a-168">WebUrl</span><span class="sxs-lookup"><span data-stu-id="dba8a-168">webUrl</span></span>|<span data-ttu-id="dba8a-169">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="dba8a-169">string (readonly)</span></span> | <span data-ttu-id="dba8a-170">将转到 Microsoft 团队客户端中的团队超链接。</span><span class="sxs-lookup"><span data-stu-id="dba8a-170">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="dba8a-171">这是当您右键单击在客户端中的 Microsoft 团队团队，然后选择**获取团队链接**获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="dba8a-171">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="dba8a-172">此 URL 应是视为不透明 blob，并且未分列。</span><span class="sxs-lookup"><span data-stu-id="dba8a-172">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dba8a-173">Relationships</span><span class="sxs-lookup"><span data-stu-id="dba8a-173">Relationships</span></span>

| <span data-ttu-id="dba8a-174">关系</span><span class="sxs-lookup"><span data-stu-id="dba8a-174">Relationship</span></span> | <span data-ttu-id="dba8a-175">类型</span><span class="sxs-lookup"><span data-stu-id="dba8a-175">Type</span></span>   | <span data-ttu-id="dba8a-176">Description</span><span class="sxs-lookup"><span data-stu-id="dba8a-176">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dba8a-177">通道</span><span class="sxs-lookup"><span data-stu-id="dba8a-177">channels</span></span>|<span data-ttu-id="dba8a-178">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="dba8a-178">[channel](channel.md) collection</span></span>|<span data-ttu-id="dba8a-179">通道邮件与团队关联的集合。</span><span class="sxs-lookup"><span data-stu-id="dba8a-179">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="dba8a-180">installedApps</span><span class="sxs-lookup"><span data-stu-id="dba8a-180">installedApps</span></span>|<span data-ttu-id="dba8a-181">[teamsAppInstallation](teamsappinstallation.md)集合</span><span class="sxs-lookup"><span data-stu-id="dba8a-181">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="dba8a-182">此团队中安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="dba8a-182">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dba8a-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dba8a-183">JSON representation</span></span>

<span data-ttu-id="dba8a-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dba8a-184">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="dba8a-185">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dba8a-185">See Also</span></span>
- [<span data-ttu-id="dba8a-186">与团队创建组</span><span class="sxs-lookup"><span data-stu-id="dba8a-186">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="dba8a-187">使用团队 Api</span><span class="sxs-lookup"><span data-stu-id="dba8a-187">Using Teams APIs</span></span>](teams-api-overview.md)
