# <a name="team-resource-type"></a><span data-ttu-id="8d8d2-101">团队资源类型</span><span class="sxs-lookup"><span data-stu-id="8d8d2-101">team resource type</span></span>



<span data-ttu-id="8d8d2-102">团队中的 Microsoft 团队是[通道](channel.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-102">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="8d8d2-103">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="8d8d2-104">每个团队是与[组](../resources/group.md)关联。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-104">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="8d8d2-105">组具有相同的 ID 团队-例如，/groups/ {id} / 球队是 /teams/ {id} 相同。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-105">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="8d8d2-106">有关使用组和团队中的成员的详细信息，请参阅[使用 Microsoft Graph REST API 以使用 Microsoft 团队](teams_api_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-106">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams_api_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8d8d2-107">方法</span><span class="sxs-lookup"><span data-stu-id="8d8d2-107">Methods</span></span>

| <span data-ttu-id="8d8d2-108">方法</span><span class="sxs-lookup"><span data-stu-id="8d8d2-108">Method</span></span>       | <span data-ttu-id="8d8d2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d8d2-109">Return Type</span></span>  |<span data-ttu-id="8d8d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d8d2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d8d2-111">创建工作组</span><span class="sxs-lookup"><span data-stu-id="8d8d2-111">Create team</span></span>](../api/team_put_teams.md) | [<span data-ttu-id="8d8d2-112">团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-112">team</span></span>](team.md) | <span data-ttu-id="8d8d2-113">创建一个新的团队，或添加到现有组的团队。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-113">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="8d8d2-114">获取工作组</span><span class="sxs-lookup"><span data-stu-id="8d8d2-114">Get team</span></span>](../api/team_get.md) | [<span data-ttu-id="8d8d2-115">团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-115">team</span></span>](team.md) | <span data-ttu-id="8d8d2-116">检索的属性和指定团队的关系。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-116">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="8d8d2-117">更新团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-117">Update team</span></span>](../api/team_update.md) | [<span data-ttu-id="8d8d2-118">团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-118">team</span></span>](team.md) |<span data-ttu-id="8d8d2-119">更新指定的团队的属性。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-119">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="8d8d2-120">删除团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-120">Delete team</span></span>](../../v1.0/api/group_delete.md) | <span data-ttu-id="8d8d2-121">无</span><span class="sxs-lookup"><span data-stu-id="8d8d2-121">None</span></span> |<span data-ttu-id="8d8d2-122">删除团队和其关联的组。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-122">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="8d8d2-123">克隆团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-123">Clone team</span></span>](../api/team_clone.md) | [<span data-ttu-id="8d8d2-124">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8d8d2-124">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8d8d2-125">复制团队和其关联的组。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-125">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="8d8d2-126">存档团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-126">Archive team</span></span>](../api/team_archive.md) | [<span data-ttu-id="8d8d2-127">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8d8d2-127">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8d8d2-128">将团队放在只读状态。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-128">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="8d8d2-129">Unarchive 团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-129">Unarchive team</span></span>](../api/team_unarchive.md) | [<span data-ttu-id="8d8d2-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="8d8d2-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="8d8d2-131">还原到读写状态团队。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-131">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="8d8d2-132">列出您的团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-132">List your teams</span></span>](../api/user_list_joinedteams.md) | <span data-ttu-id="8d8d2-133">[团队](team.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d8d2-133">[team](team.md) collection</span></span> | <span data-ttu-id="8d8d2-134">列出您是成员的团队。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-134">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="8d8d2-135">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-135">List all teams</span></span>](../../../concepts/teams_list_all_teams.md) | <span data-ttu-id="8d8d2-136">[组](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d8d2-136">[group](group.md) collection</span></span> | <span data-ttu-id="8d8d2-137">列出具有团队的所有组。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-137">List all groups that have teams.</span></span> |
|[<span data-ttu-id="8d8d2-138">将应用程序发布到您的组织</span><span class="sxs-lookup"><span data-stu-id="8d8d2-138">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="8d8d2-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d8d2-139">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="8d8d2-140">创建团队应用程序仅对您的组织可见。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-140">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="8d8d2-141">将应用程序添加到团队</span><span class="sxs-lookup"><span data-stu-id="8d8d2-141">Add app to team</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="8d8d2-142">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="8d8d2-142">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="8d8d2-143">将 （安装） 添加到团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-143">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="8d8d2-144">选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="8d8d2-144">Add tab to channel</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="8d8d2-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8d8d2-145">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="8d8d2-146">将 （安装） 添加到团队的通道选项卡。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-146">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d8d2-147">属性</span><span class="sxs-lookup"><span data-stu-id="8d8d2-147">Properties</span></span>

| <span data-ttu-id="8d8d2-148">属性</span><span class="sxs-lookup"><span data-stu-id="8d8d2-148">Property</span></span> | <span data-ttu-id="8d8d2-149">类型</span><span class="sxs-lookup"><span data-stu-id="8d8d2-149">Type</span></span>   | <span data-ttu-id="8d8d2-150">说明</span><span class="sxs-lookup"><span data-stu-id="8d8d2-150">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8d8d2-151">funSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-151">funSettings</span></span>|[<span data-ttu-id="8d8d2-152">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-152">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="8d8d2-153">要配置的团队中的使用 Giphy、 memes 和标签的设置。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-153">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="8d8d2-154">guestSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-154">guestSettings</span></span>|[<span data-ttu-id="8d8d2-155">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-155">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="8d8d2-156">要配置的是否来宾可以创建、 更新或删除通道团队中的设置。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-156">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="8d8d2-157">isArchived</span><span class="sxs-lookup"><span data-stu-id="8d8d2-157">isArchived</span></span>|<span data-ttu-id="8d8d2-158">布尔</span><span class="sxs-lookup"><span data-stu-id="8d8d2-158">Boolean</span></span>|<span data-ttu-id="8d8d2-159">此团队是否处于只读模式。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-159">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="8d8d2-160">memberSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-160">memberSettings</span></span>|[<span data-ttu-id="8d8d2-161">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-161">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="8d8d2-162">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-162">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="8d8d2-163">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-163">messagingSettings</span></span>|[<span data-ttu-id="8d8d2-164">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="8d8d2-164">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="8d8d2-165">要配置的消息设置和团队中的提及。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-165">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="8d8d2-166">WebUrl</span><span class="sxs-lookup"><span data-stu-id="8d8d2-166">webUrl</span></span>|<span data-ttu-id="8d8d2-167">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="8d8d2-167">string (readonly)</span></span> | <span data-ttu-id="8d8d2-168">将转到 Microsoft 团队客户端中的团队超链接。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-168">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="8d8d2-169">这是当您右键单击在客户端中的 Microsoft 团队团队，然后选择**获取团队链接**获取的 URL。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-169">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="8d8d2-170">此 URL 应是视为不透明 blob，并且未分列。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-170">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d8d2-171">Relationships</span><span class="sxs-lookup"><span data-stu-id="8d8d2-171">Relationships</span></span>

| <span data-ttu-id="8d8d2-172">关系</span><span class="sxs-lookup"><span data-stu-id="8d8d2-172">Relationship</span></span> | <span data-ttu-id="8d8d2-173">类型</span><span class="sxs-lookup"><span data-stu-id="8d8d2-173">Type</span></span>   | <span data-ttu-id="8d8d2-174">说明</span><span class="sxs-lookup"><span data-stu-id="8d8d2-174">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8d8d2-175">通道</span><span class="sxs-lookup"><span data-stu-id="8d8d2-175">channels</span></span>|<span data-ttu-id="8d8d2-176">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d8d2-176">[channel](channel.md) collection</span></span>|<span data-ttu-id="8d8d2-177">通道邮件与团队关联的集合。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-177">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="8d8d2-178">installedApps</span><span class="sxs-lookup"><span data-stu-id="8d8d2-178">installedApps</span></span>|<span data-ttu-id="8d8d2-179">[teamsAppInstallation](teamsappinstallation.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d8d2-179">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="8d8d2-180">此团队中安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-180">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d8d2-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d8d2-181">JSON representation</span></span>

<span data-ttu-id="8d8d2-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d8d2-182">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8d8d2-183">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8d8d2-183">See Also</span></span>
- [<span data-ttu-id="8d8d2-184">与团队创建组</span><span class="sxs-lookup"><span data-stu-id="8d8d2-184">Creating a group with a team</span></span>](../../../concepts/teams-create-group-and-team.md)
- [<span data-ttu-id="8d8d2-185">使用团队 Api</span><span class="sxs-lookup"><span data-stu-id="8d8d2-185">Using Teams APIs</span></span>](teams_api_overview.md)
