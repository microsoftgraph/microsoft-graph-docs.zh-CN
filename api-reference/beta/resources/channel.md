---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 243c3ea1e203ceaca4b31cb82dca77c873af7cb0
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272694"
---
# <a name="channel-resource-type"></a><span data-ttu-id="a09f5-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="a09f5-103">channel resource type</span></span>

<span data-ttu-id="a09f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a09f5-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="a09f5-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="a09f5-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="a09f5-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="a09f5-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="a09f5-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="a09f5-108">方法</span><span class="sxs-lookup"><span data-stu-id="a09f5-108">Methods</span></span>

| <span data-ttu-id="a09f5-109">方法</span><span class="sxs-lookup"><span data-stu-id="a09f5-109">Method</span></span>       | <span data-ttu-id="a09f5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a09f5-110">Return Type</span></span>  |<span data-ttu-id="a09f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="a09f5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a09f5-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="a09f5-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="a09f5-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="a09f5-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="a09f5-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="a09f5-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="a09f5-116">频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-116">channel</span></span>](channel.md) | <span data-ttu-id="a09f5-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="a09f5-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="a09f5-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="a09f5-119">频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-119">channel</span></span>](channel.md) | <span data-ttu-id="a09f5-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a09f5-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="a09f5-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="a09f5-122">频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-122">channel</span></span>](channel.md) | <span data-ttu-id="a09f5-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="a09f5-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="a09f5-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="a09f5-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="a09f5-125">无</span><span class="sxs-lookup"><span data-stu-id="a09f5-125">None</span></span> | <span data-ttu-id="a09f5-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="a09f5-126">Delete a channel.</span></span>|
|[<span data-ttu-id="a09f5-127">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="a09f5-127">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="a09f5-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a09f5-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a09f5-129">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="a09f5-129">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="a09f5-130">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="a09f5-130">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="a09f5-131">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a09f5-131">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a09f5-132">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="a09f5-132">Get messages in a channel</span></span> |
|[<span data-ttu-id="a09f5-133">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="a09f5-133">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="a09f5-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a09f5-134">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="a09f5-135">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="a09f5-135">List the members of a channel.</span></span> |
|[<span data-ttu-id="a09f5-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="a09f5-136">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="a09f5-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a09f5-137">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="a09f5-138">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="a09f5-138">Get a member of a channel.</span></span> |
|[<span data-ttu-id="a09f5-139">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="a09f5-139">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="a09f5-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a09f5-140">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="a09f5-141">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="a09f5-141">Add a member to a channel.</span></span> <span data-ttu-id="a09f5-142">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="a09f5-142">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="a09f5-143">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="a09f5-143">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="a09f5-144">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a09f5-144">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="a09f5-145">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="a09f5-145">Update a member of a channel.</span></span> <span data-ttu-id="a09f5-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="a09f5-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="a09f5-147">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="a09f5-147">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="a09f5-148">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a09f5-148">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="a09f5-149">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="a09f5-149">Delete a member of a channel.</span></span> <span data-ttu-id="a09f5-150">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="a09f5-150">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="a09f5-151">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="a09f5-151">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="a09f5-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a09f5-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a09f5-153">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="a09f5-153">Send a message to a channel.</span></span> |
|[<span data-ttu-id="a09f5-154">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="a09f5-154">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="a09f5-155">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a09f5-155">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="a09f5-156">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="a09f5-156">Reply to a message in a channel.</span></span>|
|[<span data-ttu-id="a09f5-157">获取文件文件夹</span><span class="sxs-lookup"><span data-stu-id="a09f5-157">Get files folder</span></span>](../api/driveitem-get.md)| [<span data-ttu-id="a09f5-158">driveItem</span><span class="sxs-lookup"><span data-stu-id="a09f5-158">driveItem</span></span>](driveitem.md) | <span data-ttu-id="a09f5-159">检索用于存储频道文件的 SharePoint 文件夹的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a09f5-159">Retrieves the details of the SharePoint folder where the files for the channel are stored.</span></span> |

## <a name="properties"></a><span data-ttu-id="a09f5-160">属性</span><span class="sxs-lookup"><span data-stu-id="a09f5-160">Properties</span></span>

| <span data-ttu-id="a09f5-161">属性</span><span class="sxs-lookup"><span data-stu-id="a09f5-161">Property</span></span>   | <span data-ttu-id="a09f5-162">类型</span><span class="sxs-lookup"><span data-stu-id="a09f5-162">Type</span></span> |<span data-ttu-id="a09f5-163">说明</span><span class="sxs-lookup"><span data-stu-id="a09f5-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a09f5-164">说明</span><span class="sxs-lookup"><span data-stu-id="a09f5-164">description</span></span>|<span data-ttu-id="a09f5-165">String</span><span class="sxs-lookup"><span data-stu-id="a09f5-165">String</span></span>|<span data-ttu-id="a09f5-166">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="a09f5-166">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="a09f5-167">displayName</span><span class="sxs-lookup"><span data-stu-id="a09f5-167">displayName</span></span>|<span data-ttu-id="a09f5-168">String</span><span class="sxs-lookup"><span data-stu-id="a09f5-168">String</span></span>|<span data-ttu-id="a09f5-169">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="a09f5-169">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="a09f5-170">id</span><span class="sxs-lookup"><span data-stu-id="a09f5-170">id</span></span>|<span data-ttu-id="a09f5-171">String</span><span class="sxs-lookup"><span data-stu-id="a09f5-171">String</span></span>|<span data-ttu-id="a09f5-172">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a09f5-172">The channel's unique identifier.</span></span> <span data-ttu-id="a09f5-173">只读。</span><span class="sxs-lookup"><span data-stu-id="a09f5-173">Read-only.</span></span>|
|<span data-ttu-id="a09f5-174">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="a09f5-174">isFavoriteByDefault</span></span>|<span data-ttu-id="a09f5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a09f5-175">Boolean</span></span>|<span data-ttu-id="a09f5-176">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="a09f5-176">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="a09f5-177">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="a09f5-177">Default: `false`.</span></span>|
|<span data-ttu-id="a09f5-178">email</span><span class="sxs-lookup"><span data-stu-id="a09f5-178">email</span></span>|<span data-ttu-id="a09f5-179">String</span><span class="sxs-lookup"><span data-stu-id="a09f5-179">String</span></span>| <span data-ttu-id="a09f5-180">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a09f5-180">The email address for sending messages to the channel.</span></span> <span data-ttu-id="a09f5-181">只读。</span><span class="sxs-lookup"><span data-stu-id="a09f5-181">Read-only.</span></span>|
|<span data-ttu-id="a09f5-182">webUrl</span><span class="sxs-lookup"><span data-stu-id="a09f5-182">webUrl</span></span>|<span data-ttu-id="a09f5-183">String</span><span class="sxs-lookup"><span data-stu-id="a09f5-183">String</span></span>|<span data-ttu-id="a09f5-184">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="a09f5-184">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="a09f5-185">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="a09f5-185">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="a09f5-186">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="a09f5-186">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="a09f5-187">只读。</span><span class="sxs-lookup"><span data-stu-id="a09f5-187">Read-only.</span></span>|
|<span data-ttu-id="a09f5-188">membershipType</span><span class="sxs-lookup"><span data-stu-id="a09f5-188">membershipType</span></span>|[<span data-ttu-id="a09f5-189">channelMembershipType</span><span class="sxs-lookup"><span data-stu-id="a09f5-189">channelMembershipType</span></span>](../resources/enums.md#channelmembershiptype-values)|<span data-ttu-id="a09f5-190">频道的类型。</span><span class="sxs-lookup"><span data-stu-id="a09f5-190">The type of the channel.</span></span> <span data-ttu-id="a09f5-191">可在创建期间设置，但不可更改。</span><span class="sxs-lookup"><span data-stu-id="a09f5-191">Can be set during creation and cannot be changed.</span></span> <span data-ttu-id="a09f5-192">默认：标准。</span><span class="sxs-lookup"><span data-stu-id="a09f5-192">Default: standard.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a09f5-193">关系</span><span class="sxs-lookup"><span data-stu-id="a09f5-193">Relationships</span></span>

| <span data-ttu-id="a09f5-194">关系</span><span class="sxs-lookup"><span data-stu-id="a09f5-194">Relationship</span></span> | <span data-ttu-id="a09f5-195">类型</span><span class="sxs-lookup"><span data-stu-id="a09f5-195">Type</span></span> |<span data-ttu-id="a09f5-196">说明</span><span class="sxs-lookup"><span data-stu-id="a09f5-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a09f5-197">messages</span><span class="sxs-lookup"><span data-stu-id="a09f5-197">messages</span></span>|<span data-ttu-id="a09f5-198">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a09f5-198">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="a09f5-199">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="a09f5-199">A collection of all the messages in the channel.</span></span> <span data-ttu-id="a09f5-200">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="a09f5-200">A navigation property.</span></span> <span data-ttu-id="a09f5-201">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a09f5-201">Nullable.</span></span>|
|<span data-ttu-id="a09f5-202">选项卡</span><span class="sxs-lookup"><span data-stu-id="a09f5-202">tabs</span></span>|<span data-ttu-id="a09f5-203">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a09f5-203">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="a09f5-204">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="a09f5-204">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="a09f5-205">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="a09f5-205">A navigation property.</span></span>|
|<span data-ttu-id="a09f5-206">成员</span><span class="sxs-lookup"><span data-stu-id="a09f5-206">members</span></span>|<span data-ttu-id="a09f5-207">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a09f5-207">[conversationMember](conversationmember.md) collection</span></span>|<span data-ttu-id="a09f5-208">与频道关联的成员资格记录的集合。</span><span class="sxs-lookup"><span data-stu-id="a09f5-208">A collection of membership records associated with the channel.</span></span>|
|<span data-ttu-id="a09f5-209">filesFolder</span><span class="sxs-lookup"><span data-stu-id="a09f5-209">filesFolder</span></span>|[<span data-ttu-id="a09f5-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="a09f5-210">driveItem</span></span>](driveitem.md)|<span data-ttu-id="a09f5-211">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="a09f5-211">Metadata for the location where the channel's files are stored.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a09f5-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a09f5-212">JSON representation</span></span>

<span data-ttu-id="a09f5-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a09f5-213">The following is a JSON representation of the resource.</span></span>

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
