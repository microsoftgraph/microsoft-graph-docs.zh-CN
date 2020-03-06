---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 491352231980e841ebe215c9c0680dc1c672b36c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507745"
---
# <a name="channel-resource-type"></a><span data-ttu-id="55b09-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="55b09-103">channel resource type</span></span>

<span data-ttu-id="55b09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55b09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55b09-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="55b09-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="55b09-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="55b09-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="55b09-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="55b09-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="55b09-108">方法</span><span class="sxs-lookup"><span data-stu-id="55b09-108">Methods</span></span>

| <span data-ttu-id="55b09-109">方法</span><span class="sxs-lookup"><span data-stu-id="55b09-109">Method</span></span>       | <span data-ttu-id="55b09-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="55b09-110">Return Type</span></span>  |<span data-ttu-id="55b09-111">说明</span><span class="sxs-lookup"><span data-stu-id="55b09-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55b09-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="55b09-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="55b09-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="55b09-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="55b09-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="55b09-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="55b09-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="55b09-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="55b09-116">频道</span><span class="sxs-lookup"><span data-stu-id="55b09-116">channel</span></span>](channel.md) | <span data-ttu-id="55b09-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="55b09-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="55b09-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="55b09-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="55b09-119">频道</span><span class="sxs-lookup"><span data-stu-id="55b09-119">channel</span></span>](channel.md) | <span data-ttu-id="55b09-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55b09-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="55b09-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="55b09-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="55b09-122">频道</span><span class="sxs-lookup"><span data-stu-id="55b09-122">channel</span></span>](channel.md) | <span data-ttu-id="55b09-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="55b09-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="55b09-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="55b09-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="55b09-125">无</span><span class="sxs-lookup"><span data-stu-id="55b09-125">None</span></span> | <span data-ttu-id="55b09-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="55b09-126">Delete a channel.</span></span>|
|[<span data-ttu-id="55b09-127">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="55b09-127">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="55b09-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55b09-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55b09-129">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="55b09-129">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="55b09-130">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="55b09-130">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="55b09-131">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55b09-131">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55b09-132">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="55b09-132">Get messages in a channel</span></span> |
|[<span data-ttu-id="55b09-133">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="55b09-133">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="55b09-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55b09-134">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="55b09-135">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="55b09-135">List the members of a channel.</span></span> |
|[<span data-ttu-id="55b09-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="55b09-136">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="55b09-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="55b09-137">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="55b09-138">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="55b09-138">Get a member of a channel.</span></span> |
|[<span data-ttu-id="55b09-139">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="55b09-139">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="55b09-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="55b09-140">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="55b09-141">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="55b09-141">Add a member to a channel.</span></span> <span data-ttu-id="55b09-142">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="55b09-142">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="55b09-143">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="55b09-143">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="55b09-144">conversationMember</span><span class="sxs-lookup"><span data-stu-id="55b09-144">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="55b09-145">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="55b09-145">Update a member of a channel.</span></span> <span data-ttu-id="55b09-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="55b09-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="55b09-147">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="55b09-147">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="55b09-148">conversationMember</span><span class="sxs-lookup"><span data-stu-id="55b09-148">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="55b09-149">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="55b09-149">Delete a member of a channel.</span></span> <span data-ttu-id="55b09-150">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="55b09-150">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="55b09-151">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="55b09-151">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="55b09-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55b09-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55b09-153">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="55b09-153">Send a message to a channel.</span></span> |
|[<span data-ttu-id="55b09-154">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="55b09-154">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="55b09-155">chatMessage</span><span class="sxs-lookup"><span data-stu-id="55b09-155">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="55b09-156">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="55b09-156">Reply to a message in a channel.</span></span>|
|[<span data-ttu-id="55b09-157">获取文件文件夹</span><span class="sxs-lookup"><span data-stu-id="55b09-157">Get files folder</span></span>](../api/driveitem-get.md)| [<span data-ttu-id="55b09-158">driveItem</span><span class="sxs-lookup"><span data-stu-id="55b09-158">driveItem</span></span>](driveitem.md) | <span data-ttu-id="55b09-159">检索用于存储频道文件的 SharePoint 文件夹的详细信息。</span><span class="sxs-lookup"><span data-stu-id="55b09-159">Retrieves the details of the SharePoint folder where the files for the channel are stored.</span></span> |

## <a name="properties"></a><span data-ttu-id="55b09-160">属性</span><span class="sxs-lookup"><span data-stu-id="55b09-160">Properties</span></span>

| <span data-ttu-id="55b09-161">属性</span><span class="sxs-lookup"><span data-stu-id="55b09-161">Property</span></span>   | <span data-ttu-id="55b09-162">类型</span><span class="sxs-lookup"><span data-stu-id="55b09-162">Type</span></span> |<span data-ttu-id="55b09-163">说明</span><span class="sxs-lookup"><span data-stu-id="55b09-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55b09-164">说明</span><span class="sxs-lookup"><span data-stu-id="55b09-164">description</span></span>|<span data-ttu-id="55b09-165">String</span><span class="sxs-lookup"><span data-stu-id="55b09-165">String</span></span>|<span data-ttu-id="55b09-166">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="55b09-166">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="55b09-167">displayName</span><span class="sxs-lookup"><span data-stu-id="55b09-167">displayName</span></span>|<span data-ttu-id="55b09-168">String</span><span class="sxs-lookup"><span data-stu-id="55b09-168">String</span></span>|<span data-ttu-id="55b09-169">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="55b09-169">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="55b09-170">id</span><span class="sxs-lookup"><span data-stu-id="55b09-170">id</span></span>|<span data-ttu-id="55b09-171">String</span><span class="sxs-lookup"><span data-stu-id="55b09-171">String</span></span>|<span data-ttu-id="55b09-172">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="55b09-172">The channel's unique identifier.</span></span> <span data-ttu-id="55b09-173">只读。</span><span class="sxs-lookup"><span data-stu-id="55b09-173">Read-only.</span></span>|
|<span data-ttu-id="55b09-174">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="55b09-174">isFavoriteByDefault</span></span>|<span data-ttu-id="55b09-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="55b09-175">Boolean</span></span>|<span data-ttu-id="55b09-176">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="55b09-176">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="55b09-177">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="55b09-177">Default: `false`.</span></span>|
|<span data-ttu-id="55b09-178">email</span><span class="sxs-lookup"><span data-stu-id="55b09-178">email</span></span>|<span data-ttu-id="55b09-179">String</span><span class="sxs-lookup"><span data-stu-id="55b09-179">String</span></span>| <span data-ttu-id="55b09-180">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="55b09-180">The email address for sending messages to the channel.</span></span> <span data-ttu-id="55b09-181">只读。</span><span class="sxs-lookup"><span data-stu-id="55b09-181">Read-only.</span></span>|
|<span data-ttu-id="55b09-182">webUrl</span><span class="sxs-lookup"><span data-stu-id="55b09-182">webUrl</span></span>|<span data-ttu-id="55b09-183">String</span><span class="sxs-lookup"><span data-stu-id="55b09-183">String</span></span>|<span data-ttu-id="55b09-184">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="55b09-184">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="55b09-185">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="55b09-185">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="55b09-186">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="55b09-186">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="55b09-187">只读。</span><span class="sxs-lookup"><span data-stu-id="55b09-187">Read-only.</span></span>|
|<span data-ttu-id="55b09-188">membershipType</span><span class="sxs-lookup"><span data-stu-id="55b09-188">membershipType</span></span>|[<span data-ttu-id="55b09-189">channelMembershipType</span><span class="sxs-lookup"><span data-stu-id="55b09-189">channelMembershipType</span></span>](../resources/enums.md#channelmembershiptype-values)|<span data-ttu-id="55b09-190">频道的类型。</span><span class="sxs-lookup"><span data-stu-id="55b09-190">The type of the channel.</span></span> <span data-ttu-id="55b09-191">可在创建期间设置，但不可更改。</span><span class="sxs-lookup"><span data-stu-id="55b09-191">Can be set during creation and cannot be changed.</span></span> <span data-ttu-id="55b09-192">默认：标准。</span><span class="sxs-lookup"><span data-stu-id="55b09-192">Default: standard.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55b09-193">关系</span><span class="sxs-lookup"><span data-stu-id="55b09-193">Relationships</span></span>

| <span data-ttu-id="55b09-194">关系</span><span class="sxs-lookup"><span data-stu-id="55b09-194">Relationship</span></span> | <span data-ttu-id="55b09-195">类型</span><span class="sxs-lookup"><span data-stu-id="55b09-195">Type</span></span> |<span data-ttu-id="55b09-196">说明</span><span class="sxs-lookup"><span data-stu-id="55b09-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55b09-197">messages</span><span class="sxs-lookup"><span data-stu-id="55b09-197">messages</span></span>|<span data-ttu-id="55b09-198">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55b09-198">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="55b09-199">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="55b09-199">A collection of all the messages in the channel.</span></span> <span data-ttu-id="55b09-200">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="55b09-200">A navigation property.</span></span> <span data-ttu-id="55b09-201">可为空。</span><span class="sxs-lookup"><span data-stu-id="55b09-201">Nullable.</span></span> <span data-ttu-id="55b09-202">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="55b09-202">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="55b09-203">选项卡</span><span class="sxs-lookup"><span data-stu-id="55b09-203">tabs</span></span>|<span data-ttu-id="55b09-204">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55b09-204">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="55b09-205">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="55b09-205">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="55b09-206">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="55b09-206">A navigation property.</span></span>|
|<span data-ttu-id="55b09-207">成员</span><span class="sxs-lookup"><span data-stu-id="55b09-207">members</span></span>|<span data-ttu-id="55b09-208">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55b09-208">[conversationMember](conversationmember.md) collection</span></span>|<span data-ttu-id="55b09-209">与频道关联的成员资格记录的集合。</span><span class="sxs-lookup"><span data-stu-id="55b09-209">A collection of membership records associated with the channel.</span></span>|
|<span data-ttu-id="55b09-210">filesFolder</span><span class="sxs-lookup"><span data-stu-id="55b09-210">filesFolder</span></span>|[<span data-ttu-id="55b09-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="55b09-211">driveItem</span></span>](driveitem.md)|<span data-ttu-id="55b09-212">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="55b09-212">Metadata for the location where the channel's files are stored.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55b09-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55b09-213">JSON representation</span></span>

<span data-ttu-id="55b09-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55b09-214">The following is a JSON representation of the resource.</span></span>

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
