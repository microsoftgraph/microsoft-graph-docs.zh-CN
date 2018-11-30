---
title: 团队资源类型
description: '团队中的 Microsoft 团队是通道的集合。 '
ms.openlocfilehash: 5ebb4dbc2c5913d69b69bdb244d8a7cfc83cec8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045579"
---
# <a name="team-resource-type"></a><span data-ttu-id="0800b-103">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="0800b-103">team resource type</span></span>

> <span data-ttu-id="0800b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0800b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0800b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0800b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0800b-106">团队中的 Microsoft 团队是[通道](channel.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="0800b-106">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="0800b-107">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="0800b-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="0800b-108">每个团队是与[组](../resources/group.md)关联。</span><span class="sxs-lookup"><span data-stu-id="0800b-108">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="0800b-109">组具有相同的 ID 团队-例如，/groups/ {id} / 球队是 /teams/ {id} 相同。</span><span class="sxs-lookup"><span data-stu-id="0800b-109">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="0800b-110">有关使用组和团队中的成员的详细信息，请参阅[使用 Microsoft Graph REST API 以使用 Microsoft 团队](teams-api-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="0800b-110">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0800b-111">方法</span><span class="sxs-lookup"><span data-stu-id="0800b-111">Methods</span></span>

| <span data-ttu-id="0800b-112">方法</span><span class="sxs-lookup"><span data-stu-id="0800b-112">Method</span></span>       | <span data-ttu-id="0800b-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="0800b-113">Return Type</span></span>  |<span data-ttu-id="0800b-114">说明</span><span class="sxs-lookup"><span data-stu-id="0800b-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0800b-115">创建工作组</span><span class="sxs-lookup"><span data-stu-id="0800b-115">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="0800b-116">团队</span><span class="sxs-lookup"><span data-stu-id="0800b-116">team</span></span>](team.md) | <span data-ttu-id="0800b-117">创建一个新的团队，或添加到现有组的团队。</span><span class="sxs-lookup"><span data-stu-id="0800b-117">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="0800b-118">获取工作组</span><span class="sxs-lookup"><span data-stu-id="0800b-118">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="0800b-119">团队</span><span class="sxs-lookup"><span data-stu-id="0800b-119">team</span></span>](team.md) | <span data-ttu-id="0800b-120">检索的属性和指定团队的关系。</span><span class="sxs-lookup"><span data-stu-id="0800b-120">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="0800b-121">更新团队</span><span class="sxs-lookup"><span data-stu-id="0800b-121">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="0800b-122">团队</span><span class="sxs-lookup"><span data-stu-id="0800b-122">team</span></span>](team.md) |<span data-ttu-id="0800b-123">更新指定的团队的属性。</span><span class="sxs-lookup"><span data-stu-id="0800b-123">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="0800b-124">删除团队</span><span class="sxs-lookup"><span data-stu-id="0800b-124">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="0800b-125">无</span><span class="sxs-lookup"><span data-stu-id="0800b-125">None</span></span> |<span data-ttu-id="0800b-126">删除团队和其关联的组。</span><span class="sxs-lookup"><span data-stu-id="0800b-126">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="0800b-127">克隆团队</span><span class="sxs-lookup"><span data-stu-id="0800b-127">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="0800b-128">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="0800b-128">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="0800b-129">复制团队和其关联的组。</span><span class="sxs-lookup"><span data-stu-id="0800b-129">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="0800b-130">存档团队</span><span class="sxs-lookup"><span data-stu-id="0800b-130">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="0800b-131">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="0800b-131">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="0800b-132">将团队放在只读状态。</span><span class="sxs-lookup"><span data-stu-id="0800b-132">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="0800b-133">Unarchive 团队</span><span class="sxs-lookup"><span data-stu-id="0800b-133">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="0800b-134">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="0800b-134">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="0800b-135">还原到读写状态团队。</span><span class="sxs-lookup"><span data-stu-id="0800b-135">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="0800b-136">列出您的团队</span><span class="sxs-lookup"><span data-stu-id="0800b-136">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="0800b-137">[团队](team.md)集合</span><span class="sxs-lookup"><span data-stu-id="0800b-137">[team](team.md) collection</span></span> | <span data-ttu-id="0800b-138">列出您是成员的团队。</span><span class="sxs-lookup"><span data-stu-id="0800b-138">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="0800b-139">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="0800b-139">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="0800b-140">[组](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0800b-140">[group](group.md) collection</span></span> | <span data-ttu-id="0800b-141">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="0800b-141">List all groups that have teams.</span></span> |
|[<span data-ttu-id="0800b-142">将应用程序发布到您的组织</span><span class="sxs-lookup"><span data-stu-id="0800b-142">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="0800b-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0800b-143">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="0800b-144">创建团队应用程序仅对您的组织可见。</span><span class="sxs-lookup"><span data-stu-id="0800b-144">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="0800b-145">将应用程序添加到团队</span><span class="sxs-lookup"><span data-stu-id="0800b-145">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="0800b-146">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="0800b-146">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="0800b-147">将 （安装） 添加到团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="0800b-147">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="0800b-148">选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="0800b-148">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="0800b-149">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0800b-149">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="0800b-150">将 （安装） 添加到团队的通道选项卡。</span><span class="sxs-lookup"><span data-stu-id="0800b-150">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="0800b-151">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="0800b-151">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="0800b-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0800b-152">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="0800b-153">在通道中收到消息</span><span class="sxs-lookup"><span data-stu-id="0800b-153">Get messages in a channel</span></span>](../api/channel-list-messages.md) |

## <a name="properties"></a><span data-ttu-id="0800b-154">属性</span><span class="sxs-lookup"><span data-stu-id="0800b-154">Properties</span></span>

| <span data-ttu-id="0800b-155">属性</span><span class="sxs-lookup"><span data-stu-id="0800b-155">Property</span></span> | <span data-ttu-id="0800b-156">类型</span><span class="sxs-lookup"><span data-stu-id="0800b-156">Type</span></span>   | <span data-ttu-id="0800b-157">说明</span><span class="sxs-lookup"><span data-stu-id="0800b-157">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0800b-158">funSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-158">funSettings</span></span>|[<span data-ttu-id="0800b-159">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-159">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="0800b-160">要配置的团队中的使用 Giphy、 memes 和标签的设置。</span><span class="sxs-lookup"><span data-stu-id="0800b-160">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="0800b-161">guestSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-161">guestSettings</span></span>|[<span data-ttu-id="0800b-162">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-162">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="0800b-163">要配置的是否来宾可以创建、 更新或删除通道团队中的设置。</span><span class="sxs-lookup"><span data-stu-id="0800b-163">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="0800b-164">isArchived</span><span class="sxs-lookup"><span data-stu-id="0800b-164">isArchived</span></span>|<span data-ttu-id="0800b-165">布尔</span><span class="sxs-lookup"><span data-stu-id="0800b-165">Boolean</span></span>|<span data-ttu-id="0800b-166">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="0800b-166">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="0800b-167">memberSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-167">memberSettings</span></span>|[<span data-ttu-id="0800b-168">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-168">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="0800b-169">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。</span><span class="sxs-lookup"><span data-stu-id="0800b-169">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="0800b-170">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-170">messagingSettings</span></span>|[<span data-ttu-id="0800b-171">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="0800b-171">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="0800b-172">要配置的消息设置和团队中的提及。</span><span class="sxs-lookup"><span data-stu-id="0800b-172">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="0800b-173">WebUrl</span><span class="sxs-lookup"><span data-stu-id="0800b-173">webUrl</span></span>|<span data-ttu-id="0800b-174">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="0800b-174">string (readonly)</span></span> | <span data-ttu-id="0800b-175">将转到 Microsoft 团队客户端中的团队超链接。</span><span class="sxs-lookup"><span data-stu-id="0800b-175">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="0800b-176">这是当您右键单击在客户端中的 Microsoft 团队团队，然后选择**获取团队链接**获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="0800b-176">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="0800b-177">此 URL 应是视为不透明 blob，并且未分列。</span><span class="sxs-lookup"><span data-stu-id="0800b-177">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0800b-178">Relationships</span><span class="sxs-lookup"><span data-stu-id="0800b-178">Relationships</span></span>

| <span data-ttu-id="0800b-179">关系</span><span class="sxs-lookup"><span data-stu-id="0800b-179">Relationship</span></span> | <span data-ttu-id="0800b-180">类型</span><span class="sxs-lookup"><span data-stu-id="0800b-180">Type</span></span>   | <span data-ttu-id="0800b-181">说明</span><span class="sxs-lookup"><span data-stu-id="0800b-181">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0800b-182">apps</span><span class="sxs-lookup"><span data-stu-id="0800b-182">apps</span></span>|<span data-ttu-id="0800b-183">[teamsApp](teamsapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="0800b-183">[teamsApp](teamsapp.md) collection</span></span>| <span data-ttu-id="0800b-184">（已过时）此团队中安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="0800b-184">(Obsolete) The apps installed in this team.</span></span>|
|<span data-ttu-id="0800b-185">通道</span><span class="sxs-lookup"><span data-stu-id="0800b-185">channels</span></span>|<span data-ttu-id="0800b-186">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="0800b-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="0800b-187">通道邮件与团队关联的集合。</span><span class="sxs-lookup"><span data-stu-id="0800b-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="0800b-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="0800b-188">installedApps</span></span>|<span data-ttu-id="0800b-189">[teamsAppInstallation](teamsappinstallation.md)集合</span><span class="sxs-lookup"><span data-stu-id="0800b-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="0800b-190">此团队中安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="0800b-190">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0800b-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0800b-191">JSON representation</span></span>

<span data-ttu-id="0800b-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0800b-192">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0800b-193">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0800b-193">See Also</span></span>
- [<span data-ttu-id="0800b-194">与团队创建组</span><span class="sxs-lookup"><span data-stu-id="0800b-194">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="0800b-195">团队 API 概述</span><span class="sxs-lookup"><span data-stu-id="0800b-195">Teams API Overview</span></span>](teams-api-overview.md)
