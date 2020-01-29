---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b9255dfc6b20f2fe2028c173a7704941249a15fb
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559031"
---
# <a name="channel-resource-type"></a><span data-ttu-id="715bc-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="715bc-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="715bc-104">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="715bc-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="715bc-105">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="715bc-105">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="715bc-106">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="715bc-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="715bc-107">方法</span><span class="sxs-lookup"><span data-stu-id="715bc-107">Methods</span></span>

| <span data-ttu-id="715bc-108">方法</span><span class="sxs-lookup"><span data-stu-id="715bc-108">Method</span></span>       | <span data-ttu-id="715bc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="715bc-109">Return Type</span></span>  |<span data-ttu-id="715bc-110">说明</span><span class="sxs-lookup"><span data-stu-id="715bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="715bc-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="715bc-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="715bc-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="715bc-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="715bc-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="715bc-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="715bc-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="715bc-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="715bc-115">频道</span><span class="sxs-lookup"><span data-stu-id="715bc-115">channel</span></span>](channel.md) | <span data-ttu-id="715bc-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="715bc-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="715bc-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="715bc-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="715bc-118">频道</span><span class="sxs-lookup"><span data-stu-id="715bc-118">channel</span></span>](channel.md) | <span data-ttu-id="715bc-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="715bc-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="715bc-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="715bc-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="715bc-121">频道</span><span class="sxs-lookup"><span data-stu-id="715bc-121">channel</span></span>](channel.md) | <span data-ttu-id="715bc-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="715bc-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="715bc-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="715bc-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="715bc-124">无</span><span class="sxs-lookup"><span data-stu-id="715bc-124">None</span></span> | <span data-ttu-id="715bc-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="715bc-125">Delete a channel.</span></span>|
|[<span data-ttu-id="715bc-126">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="715bc-126">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="715bc-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="715bc-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="715bc-128">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="715bc-128">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="715bc-129">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="715bc-129">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="715bc-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="715bc-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="715bc-131">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="715bc-131">Get messages in a channel</span></span> |
|[<span data-ttu-id="715bc-132">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="715bc-132">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="715bc-133">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="715bc-133">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="715bc-134">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="715bc-134">List the members of a channel.</span></span> |
|[<span data-ttu-id="715bc-135">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="715bc-135">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="715bc-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="715bc-136">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="715bc-137">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="715bc-137">Get a member of a channel.</span></span> |
|[<span data-ttu-id="715bc-138">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="715bc-138">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="715bc-139">conversationMember</span><span class="sxs-lookup"><span data-stu-id="715bc-139">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="715bc-140">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="715bc-140">Add a member to a channel.</span></span> <span data-ttu-id="715bc-141">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="715bc-141">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="715bc-142">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="715bc-142">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="715bc-143">conversationMember</span><span class="sxs-lookup"><span data-stu-id="715bc-143">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="715bc-144">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="715bc-144">Update a member of a channel.</span></span> <span data-ttu-id="715bc-145">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="715bc-145">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="715bc-146">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="715bc-146">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="715bc-147">conversationMember</span><span class="sxs-lookup"><span data-stu-id="715bc-147">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="715bc-148">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="715bc-148">Delete a member of a channel.</span></span> <span data-ttu-id="715bc-149">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="715bc-149">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="715bc-150">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="715bc-150">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="715bc-151">chatMessage</span><span class="sxs-lookup"><span data-stu-id="715bc-151">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="715bc-152">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="715bc-152">Send a message to a channel.</span></span> |
|[<span data-ttu-id="715bc-153">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="715bc-153">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="715bc-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="715bc-154">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="715bc-155">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="715bc-155">Reply to a message in a channel.</span></span>|
|[<span data-ttu-id="715bc-156">获取文件文件夹</span><span class="sxs-lookup"><span data-stu-id="715bc-156">Get files folder</span></span>](../api/driveitem-get.md)| [<span data-ttu-id="715bc-157">driveItem</span><span class="sxs-lookup"><span data-stu-id="715bc-157">driveItem</span></span>](driveitem.md) | <span data-ttu-id="715bc-158">检索用于存储频道文件的 SharePoint 文件夹的详细信息。</span><span class="sxs-lookup"><span data-stu-id="715bc-158">Retrieves the details of the SharePoint folder where the files for the channel are stored.</span></span> |

## <a name="properties"></a><span data-ttu-id="715bc-159">属性</span><span class="sxs-lookup"><span data-stu-id="715bc-159">Properties</span></span>

| <span data-ttu-id="715bc-160">属性</span><span class="sxs-lookup"><span data-stu-id="715bc-160">Property</span></span>   | <span data-ttu-id="715bc-161">类型</span><span class="sxs-lookup"><span data-stu-id="715bc-161">Type</span></span> |<span data-ttu-id="715bc-162">说明</span><span class="sxs-lookup"><span data-stu-id="715bc-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="715bc-163">说明</span><span class="sxs-lookup"><span data-stu-id="715bc-163">description</span></span>|<span data-ttu-id="715bc-164">String</span><span class="sxs-lookup"><span data-stu-id="715bc-164">String</span></span>|<span data-ttu-id="715bc-165">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="715bc-165">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="715bc-166">displayName</span><span class="sxs-lookup"><span data-stu-id="715bc-166">displayName</span></span>|<span data-ttu-id="715bc-167">String</span><span class="sxs-lookup"><span data-stu-id="715bc-167">String</span></span>|<span data-ttu-id="715bc-168">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="715bc-168">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="715bc-169">id</span><span class="sxs-lookup"><span data-stu-id="715bc-169">id</span></span>|<span data-ttu-id="715bc-170">String</span><span class="sxs-lookup"><span data-stu-id="715bc-170">String</span></span>|<span data-ttu-id="715bc-171">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="715bc-171">The channel's unique identifier.</span></span> <span data-ttu-id="715bc-172">只读。</span><span class="sxs-lookup"><span data-stu-id="715bc-172">Read-only.</span></span>|
|<span data-ttu-id="715bc-173">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="715bc-173">isFavoriteByDefault</span></span>|<span data-ttu-id="715bc-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="715bc-174">Boolean</span></span>|<span data-ttu-id="715bc-175">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="715bc-175">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="715bc-176">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="715bc-176">Default: `false`.</span></span>|
|<span data-ttu-id="715bc-177">email</span><span class="sxs-lookup"><span data-stu-id="715bc-177">email</span></span>|<span data-ttu-id="715bc-178">String</span><span class="sxs-lookup"><span data-stu-id="715bc-178">String</span></span>| <span data-ttu-id="715bc-179">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="715bc-179">The email address for sending messages to the channel.</span></span> <span data-ttu-id="715bc-180">只读。</span><span class="sxs-lookup"><span data-stu-id="715bc-180">Read-only.</span></span>|
|<span data-ttu-id="715bc-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="715bc-181">webUrl</span></span>|<span data-ttu-id="715bc-182">String</span><span class="sxs-lookup"><span data-stu-id="715bc-182">String</span></span>|<span data-ttu-id="715bc-183">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="715bc-183">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="715bc-184">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="715bc-184">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="715bc-185">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="715bc-185">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="715bc-186">只读。</span><span class="sxs-lookup"><span data-stu-id="715bc-186">Read-only.</span></span>|
|<span data-ttu-id="715bc-187">membershipType</span><span class="sxs-lookup"><span data-stu-id="715bc-187">membershipType</span></span>|[<span data-ttu-id="715bc-188">channelMembershipType</span><span class="sxs-lookup"><span data-stu-id="715bc-188">channelMembershipType</span></span>](../resources/enums.md#channelmembershiptype-values)|<span data-ttu-id="715bc-189">频道的类型。</span><span class="sxs-lookup"><span data-stu-id="715bc-189">The type of the channel.</span></span> <span data-ttu-id="715bc-190">可在创建期间设置，但不可更改。</span><span class="sxs-lookup"><span data-stu-id="715bc-190">Can be set during creation and cannot be changed.</span></span> <span data-ttu-id="715bc-191">默认：标准。</span><span class="sxs-lookup"><span data-stu-id="715bc-191">Default: standard.</span></span>|

## <a name="relationships"></a><span data-ttu-id="715bc-192">关系</span><span class="sxs-lookup"><span data-stu-id="715bc-192">Relationships</span></span>

| <span data-ttu-id="715bc-193">关系</span><span class="sxs-lookup"><span data-stu-id="715bc-193">Relationship</span></span> | <span data-ttu-id="715bc-194">类型</span><span class="sxs-lookup"><span data-stu-id="715bc-194">Type</span></span> |<span data-ttu-id="715bc-195">说明</span><span class="sxs-lookup"><span data-stu-id="715bc-195">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="715bc-196">messages</span><span class="sxs-lookup"><span data-stu-id="715bc-196">messages</span></span>|<span data-ttu-id="715bc-197">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="715bc-197">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="715bc-198">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="715bc-198">A collection of all the messages in the channel.</span></span> <span data-ttu-id="715bc-199">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="715bc-199">A navigation property.</span></span> <span data-ttu-id="715bc-200">可为空。</span><span class="sxs-lookup"><span data-stu-id="715bc-200">Nullable.</span></span> <span data-ttu-id="715bc-201">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="715bc-201">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="715bc-202">选项卡</span><span class="sxs-lookup"><span data-stu-id="715bc-202">tabs</span></span>|<span data-ttu-id="715bc-203">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="715bc-203">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="715bc-204">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="715bc-204">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="715bc-205">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="715bc-205">A navigation property.</span></span>|
|<span data-ttu-id="715bc-206">成员</span><span class="sxs-lookup"><span data-stu-id="715bc-206">members</span></span>|<span data-ttu-id="715bc-207">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="715bc-207">[conversationMember](conversationmember.md) collection</span></span>|<span data-ttu-id="715bc-208">与频道关联的成员资格记录的集合。</span><span class="sxs-lookup"><span data-stu-id="715bc-208">A collection of membership records associated with the channel.</span></span>|
|<span data-ttu-id="715bc-209">filesFolder</span><span class="sxs-lookup"><span data-stu-id="715bc-209">filesFolder</span></span>|[<span data-ttu-id="715bc-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="715bc-210">driveItem</span></span>](driveitem.md)|<span data-ttu-id="715bc-211">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="715bc-211">Metadata for the location where the channel's files are stored.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="715bc-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="715bc-212">JSON representation</span></span>

<span data-ttu-id="715bc-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="715bc-213">The following is a JSON representation of the resource.</span></span>

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
