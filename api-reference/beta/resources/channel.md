---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8c6239cc91eb10ecec5d2e037ffa9364e55646e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633676"
---
# <a name="channel-resource-type"></a><span data-ttu-id="4c604-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="4c604-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c604-104">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="4c604-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="4c604-105">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="4c604-105">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="4c604-106">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="4c604-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="4c604-107">方法</span><span class="sxs-lookup"><span data-stu-id="4c604-107">Methods</span></span>

| <span data-ttu-id="4c604-108">方法</span><span class="sxs-lookup"><span data-stu-id="4c604-108">Method</span></span>       | <span data-ttu-id="4c604-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4c604-109">Return Type</span></span>  |<span data-ttu-id="4c604-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c604-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c604-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="4c604-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="4c604-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="4c604-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="4c604-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="4c604-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="4c604-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="4c604-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="4c604-115">频道</span><span class="sxs-lookup"><span data-stu-id="4c604-115">channel</span></span>](channel.md) | <span data-ttu-id="4c604-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="4c604-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="4c604-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="4c604-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="4c604-118">频道</span><span class="sxs-lookup"><span data-stu-id="4c604-118">channel</span></span>](channel.md) | <span data-ttu-id="4c604-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c604-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="4c604-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="4c604-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="4c604-121">频道</span><span class="sxs-lookup"><span data-stu-id="4c604-121">channel</span></span>](channel.md) | <span data-ttu-id="4c604-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="4c604-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="4c604-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="4c604-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="4c604-124">无</span><span class="sxs-lookup"><span data-stu-id="4c604-124">None</span></span> | <span data-ttu-id="4c604-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="4c604-125">Delete a channel.</span></span>|
|[<span data-ttu-id="4c604-126">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="4c604-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="4c604-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4c604-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4c604-128">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="4c604-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="4c604-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="4c604-129">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="4c604-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c604-130">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="4c604-131">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="4c604-131">List the members of a channel.</span></span> |
|[<span data-ttu-id="4c604-132">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="4c604-132">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="4c604-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4c604-133">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4c604-134">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="4c604-134">Get a member of a channel.</span></span> |
|[<span data-ttu-id="4c604-135">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="4c604-135">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="4c604-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4c604-136">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4c604-137">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="4c604-137">Add a member to a class.</span></span> <span data-ttu-id="4c604-138">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="4c604-138">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="4c604-139">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="4c604-139">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="4c604-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4c604-140">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4c604-141">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="4c604-141">Update a member of a channel.</span></span> <span data-ttu-id="4c604-142">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="4c604-142">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="4c604-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="4c604-143">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="4c604-144">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4c604-144">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="4c604-145">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="4c604-145">Delete a member of a channel.</span></span> <span data-ttu-id="4c604-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="4c604-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="4c604-147">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="4c604-147">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="4c604-148">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4c604-148">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4c604-149">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="4c604-149">Send a message to a channel</span></span> |
|[<span data-ttu-id="4c604-150">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="4c604-150">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="4c604-151">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4c604-151">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4c604-152">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="4c604-152">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="4c604-153">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="4c604-153">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="4c604-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4c604-154">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4c604-155">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="4c604-155">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="4c604-156">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="4c604-156">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="4c604-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4c604-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4c604-158">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="4c604-158">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="4c604-159">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="4c604-159">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4c604-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4c604-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4c604-161">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="4c604-161">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="4c604-162">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="4c604-162">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="4c604-163">无</span><span class="sxs-lookup"><span data-stu-id="4c604-163">None</span></span> | <span data-ttu-id="4c604-164">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="4c604-164">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="4c604-165">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="4c604-165">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="4c604-166">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4c604-166">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4c604-167">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="4c604-167">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c604-168">属性</span><span class="sxs-lookup"><span data-stu-id="4c604-168">Properties</span></span>

| <span data-ttu-id="4c604-169">属性</span><span class="sxs-lookup"><span data-stu-id="4c604-169">Property</span></span>    | <span data-ttu-id="4c604-170">类型</span><span class="sxs-lookup"><span data-stu-id="4c604-170">Type</span></span> |<span data-ttu-id="4c604-171">说明</span><span class="sxs-lookup"><span data-stu-id="4c604-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c604-172">说明</span><span class="sxs-lookup"><span data-stu-id="4c604-172">description</span></span>|<span data-ttu-id="4c604-173">String</span><span class="sxs-lookup"><span data-stu-id="4c604-173">String</span></span>|<span data-ttu-id="4c604-174">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="4c604-174">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="4c604-175">displayName</span><span class="sxs-lookup"><span data-stu-id="4c604-175">displayName</span></span>|<span data-ttu-id="4c604-176">String</span><span class="sxs-lookup"><span data-stu-id="4c604-176">String</span></span>|<span data-ttu-id="4c604-177">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="4c604-177">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="4c604-178">id</span><span class="sxs-lookup"><span data-stu-id="4c604-178">id</span></span>|<span data-ttu-id="4c604-179">String</span><span class="sxs-lookup"><span data-stu-id="4c604-179">String</span></span>|<span data-ttu-id="4c604-180">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4c604-180">The channels's unique identifier.</span></span> <span data-ttu-id="4c604-181">只读。</span><span class="sxs-lookup"><span data-stu-id="4c604-181">Read-only.</span></span>|
|<span data-ttu-id="4c604-182">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="4c604-182">isFavoriteByDefault</span></span>|<span data-ttu-id="4c604-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c604-183">Boolean</span></span>|<span data-ttu-id="4c604-184">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="4c604-184">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="4c604-185">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="4c604-185">Default: `false`.</span></span>|
|<span data-ttu-id="4c604-186">email</span><span class="sxs-lookup"><span data-stu-id="4c604-186">email</span></span>|<span data-ttu-id="4c604-187">String</span><span class="sxs-lookup"><span data-stu-id="4c604-187">String</span></span>| <span data-ttu-id="4c604-188">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4c604-188">The email address for sending messages to the channel.</span></span> <span data-ttu-id="4c604-189">只读。</span><span class="sxs-lookup"><span data-stu-id="4c604-189">Read-only.</span></span>|
|<span data-ttu-id="4c604-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="4c604-190">webUrl</span></span>|<span data-ttu-id="4c604-191">String</span><span class="sxs-lookup"><span data-stu-id="4c604-191">String</span></span>|<span data-ttu-id="4c604-192">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="4c604-192">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="4c604-193">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="4c604-193">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="4c604-194">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="4c604-194">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="4c604-195">只读。</span><span class="sxs-lookup"><span data-stu-id="4c604-195">Read-only.</span></span>|
|<span data-ttu-id="4c604-196">membershipType</span><span class="sxs-lookup"><span data-stu-id="4c604-196">membershipType</span></span>|[<span data-ttu-id="4c604-197">channelMembershipType</span><span class="sxs-lookup"><span data-stu-id="4c604-197">channelMembershipType</span></span>](../resources/enums.md#channelmembershiptype-values)|<span data-ttu-id="4c604-198">频道的类型。</span><span class="sxs-lookup"><span data-stu-id="4c604-198">The ID of the channel.</span></span> <span data-ttu-id="4c604-199">可在创建期间设置，但不可更改。</span><span class="sxs-lookup"><span data-stu-id="4c604-199">Can be set during creation and cannot be changed.</span></span> <span data-ttu-id="4c604-200">默认：标准。</span><span class="sxs-lookup"><span data-stu-id="4c604-200">Default: standard.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c604-201">关系</span><span class="sxs-lookup"><span data-stu-id="4c604-201">Relationships</span></span>

| <span data-ttu-id="4c604-202">关系</span><span class="sxs-lookup"><span data-stu-id="4c604-202">Relationship</span></span> | <span data-ttu-id="4c604-203">类型</span><span class="sxs-lookup"><span data-stu-id="4c604-203">Type</span></span>   |<span data-ttu-id="4c604-204">说明</span><span class="sxs-lookup"><span data-stu-id="4c604-204">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c604-205">messages</span><span class="sxs-lookup"><span data-stu-id="4c604-205">messages</span></span>|<span data-ttu-id="4c604-206">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c604-206">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="4c604-207">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="4c604-207">A collection of all the messages in the channel.</span></span> <span data-ttu-id="4c604-208">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="4c604-208">A navigation property.</span></span> <span data-ttu-id="4c604-209">可为空。</span><span class="sxs-lookup"><span data-stu-id="4c604-209">Nullable.</span></span> <span data-ttu-id="4c604-210">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="4c604-210">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="4c604-211">选项卡</span><span class="sxs-lookup"><span data-stu-id="4c604-211">tabs</span></span>|<span data-ttu-id="4c604-212">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c604-212">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="4c604-213">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="4c604-213">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="4c604-214">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="4c604-214">A navigation property.</span></span>|
|<span data-ttu-id="4c604-215">成员</span><span class="sxs-lookup"><span data-stu-id="4c604-215">members</span></span>|<span data-ttu-id="4c604-216">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c604-216">[conversationMember](conversationmember.md) collection</span></span>|<span data-ttu-id="4c604-217">与频道关联的成员资格记录的集合。</span><span class="sxs-lookup"><span data-stu-id="4c604-217">A collection of membership records associated with the channel.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c604-218">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c604-218">JSON representation</span></span>

<span data-ttu-id="4c604-219">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c604-219">The following is a JSON representation of the resource.</span></span>

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
