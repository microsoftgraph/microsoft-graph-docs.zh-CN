---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cdcb7f10d068372c167f65a7868672a7cb669107
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677125"
---
# <a name="channel-resource-type"></a><span data-ttu-id="25812-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="25812-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25812-104">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="25812-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="25812-105">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="25812-105">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="25812-106">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="25812-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="25812-107">方法</span><span class="sxs-lookup"><span data-stu-id="25812-107">Methods</span></span>

| <span data-ttu-id="25812-108">方法</span><span class="sxs-lookup"><span data-stu-id="25812-108">Method</span></span>       | <span data-ttu-id="25812-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="25812-109">Return Type</span></span>  |<span data-ttu-id="25812-110">说明</span><span class="sxs-lookup"><span data-stu-id="25812-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25812-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="25812-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="25812-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="25812-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="25812-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="25812-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="25812-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="25812-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="25812-115">频道</span><span class="sxs-lookup"><span data-stu-id="25812-115">channel</span></span>](channel.md) | <span data-ttu-id="25812-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="25812-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="25812-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="25812-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="25812-118">频道</span><span class="sxs-lookup"><span data-stu-id="25812-118">channel</span></span>](channel.md) | <span data-ttu-id="25812-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25812-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="25812-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="25812-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="25812-121">频道</span><span class="sxs-lookup"><span data-stu-id="25812-121">channel</span></span>](channel.md) | <span data-ttu-id="25812-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="25812-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="25812-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="25812-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="25812-124">无</span><span class="sxs-lookup"><span data-stu-id="25812-124">None</span></span> | <span data-ttu-id="25812-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="25812-125">Delete a channel.</span></span>|
|[<span data-ttu-id="25812-126">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="25812-126">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="25812-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25812-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="25812-128">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="25812-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="25812-129">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="25812-129">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="25812-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25812-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="25812-131">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="25812-131">Get messages in a channel</span></span> |
|[<span data-ttu-id="25812-132">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="25812-132">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="25812-133">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25812-133">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="25812-134">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="25812-134">List the members of a channel.</span></span> |
|[<span data-ttu-id="25812-135">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="25812-135">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="25812-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25812-136">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="25812-137">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="25812-137">Get a member of a channel.</span></span> |
|[<span data-ttu-id="25812-138">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="25812-138">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="25812-139">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25812-139">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="25812-140">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="25812-140">Add a member to a class.</span></span> <span data-ttu-id="25812-141">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="25812-141">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="25812-142">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="25812-142">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="25812-143">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25812-143">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="25812-144">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="25812-144">Update a member of a channel.</span></span> <span data-ttu-id="25812-145">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="25812-145">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="25812-146">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="25812-146">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="25812-147">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25812-147">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="25812-148">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="25812-148">Delete a member of a channel.</span></span> <span data-ttu-id="25812-149">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="25812-149">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="25812-150">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="25812-150">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="25812-151">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25812-151">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="25812-152">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="25812-152">Send a message to a channel</span></span> |
|[<span data-ttu-id="25812-153">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="25812-153">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="25812-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="25812-154">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="25812-155">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="25812-155">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="25812-156">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="25812-156">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="25812-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25812-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25812-158">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="25812-158">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="25812-159">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="25812-159">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="25812-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25812-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25812-161">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="25812-161">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="25812-162">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="25812-162">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="25812-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25812-163">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25812-164">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="25812-164">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="25812-165">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="25812-165">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="25812-166">无</span><span class="sxs-lookup"><span data-stu-id="25812-166">None</span></span> | <span data-ttu-id="25812-167">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="25812-167">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="25812-168">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="25812-168">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="25812-169">teamsTab</span><span class="sxs-lookup"><span data-stu-id="25812-169">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="25812-170">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="25812-170">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="25812-171">属性</span><span class="sxs-lookup"><span data-stu-id="25812-171">Properties</span></span>

| <span data-ttu-id="25812-172">属性</span><span class="sxs-lookup"><span data-stu-id="25812-172">Property</span></span>   | <span data-ttu-id="25812-173">类型</span><span class="sxs-lookup"><span data-stu-id="25812-173">Type</span></span> |<span data-ttu-id="25812-174">说明</span><span class="sxs-lookup"><span data-stu-id="25812-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25812-175">说明</span><span class="sxs-lookup"><span data-stu-id="25812-175">description</span></span>|<span data-ttu-id="25812-176">String</span><span class="sxs-lookup"><span data-stu-id="25812-176">String</span></span>|<span data-ttu-id="25812-177">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="25812-177">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="25812-178">displayName</span><span class="sxs-lookup"><span data-stu-id="25812-178">displayName</span></span>|<span data-ttu-id="25812-179">String</span><span class="sxs-lookup"><span data-stu-id="25812-179">String</span></span>|<span data-ttu-id="25812-180">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="25812-180">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="25812-181">id</span><span class="sxs-lookup"><span data-stu-id="25812-181">id</span></span>|<span data-ttu-id="25812-182">String</span><span class="sxs-lookup"><span data-stu-id="25812-182">String</span></span>|<span data-ttu-id="25812-183">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="25812-183">The channels's unique identifier.</span></span> <span data-ttu-id="25812-184">只读。</span><span class="sxs-lookup"><span data-stu-id="25812-184">Read-only.</span></span>|
|<span data-ttu-id="25812-185">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="25812-185">isFavoriteByDefault</span></span>|<span data-ttu-id="25812-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="25812-186">Boolean</span></span>|<span data-ttu-id="25812-187">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="25812-187">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="25812-188">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="25812-188">Default: `false`.</span></span>|
|<span data-ttu-id="25812-189">email</span><span class="sxs-lookup"><span data-stu-id="25812-189">email</span></span>|<span data-ttu-id="25812-190">String</span><span class="sxs-lookup"><span data-stu-id="25812-190">String</span></span>| <span data-ttu-id="25812-191">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="25812-191">The email address for sending messages to the channel.</span></span> <span data-ttu-id="25812-192">只读。</span><span class="sxs-lookup"><span data-stu-id="25812-192">Read-only.</span></span>|
|<span data-ttu-id="25812-193">webUrl</span><span class="sxs-lookup"><span data-stu-id="25812-193">webUrl</span></span>|<span data-ttu-id="25812-194">String</span><span class="sxs-lookup"><span data-stu-id="25812-194">String</span></span>|<span data-ttu-id="25812-195">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="25812-195">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="25812-196">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="25812-196">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="25812-197">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="25812-197">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="25812-198">只读。</span><span class="sxs-lookup"><span data-stu-id="25812-198">Read-only.</span></span>|
|<span data-ttu-id="25812-199">membershipType</span><span class="sxs-lookup"><span data-stu-id="25812-199">membershipType</span></span>|[<span data-ttu-id="25812-200">channelMembershipType</span><span class="sxs-lookup"><span data-stu-id="25812-200">channelMembershipType</span></span>](../resources/enums.md#channelmembershiptype-values)|<span data-ttu-id="25812-201">频道的类型。</span><span class="sxs-lookup"><span data-stu-id="25812-201">The ID of the channel.</span></span> <span data-ttu-id="25812-202">可在创建期间设置，但不可更改。</span><span class="sxs-lookup"><span data-stu-id="25812-202">Can be set during creation and cannot be changed.</span></span> <span data-ttu-id="25812-203">默认：标准。</span><span class="sxs-lookup"><span data-stu-id="25812-203">Default: standard.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25812-204">关系</span><span class="sxs-lookup"><span data-stu-id="25812-204">Relationships</span></span>

| <span data-ttu-id="25812-205">关系</span><span class="sxs-lookup"><span data-stu-id="25812-205">Relationship</span></span> | <span data-ttu-id="25812-206">类型</span><span class="sxs-lookup"><span data-stu-id="25812-206">Type</span></span> |<span data-ttu-id="25812-207">说明</span><span class="sxs-lookup"><span data-stu-id="25812-207">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25812-208">messages</span><span class="sxs-lookup"><span data-stu-id="25812-208">messages</span></span>|<span data-ttu-id="25812-209">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25812-209">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="25812-210">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="25812-210">A collection of all the messages in the channel.</span></span> <span data-ttu-id="25812-211">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="25812-211">A navigation property.</span></span> <span data-ttu-id="25812-212">可为空。</span><span class="sxs-lookup"><span data-stu-id="25812-212">Nullable.</span></span> <span data-ttu-id="25812-213">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="25812-213">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="25812-214">选项卡</span><span class="sxs-lookup"><span data-stu-id="25812-214">tabs</span></span>|<span data-ttu-id="25812-215">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25812-215">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="25812-216">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="25812-216">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="25812-217">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="25812-217">A navigation property.</span></span>|
|<span data-ttu-id="25812-218">成员</span><span class="sxs-lookup"><span data-stu-id="25812-218">members</span></span>|<span data-ttu-id="25812-219">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25812-219">[conversationMember](conversationmember.md) collection</span></span>|<span data-ttu-id="25812-220">与频道关联的成员资格记录的集合。</span><span class="sxs-lookup"><span data-stu-id="25812-220">A collection of membership records associated with the channel.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25812-221">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25812-221">JSON representation</span></span>

<span data-ttu-id="25812-222">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25812-222">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "membershipType": "channelMembershipType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
