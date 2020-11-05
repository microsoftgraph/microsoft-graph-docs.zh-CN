---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: baf38d4ced45f5616a8db1bf51fe2d3ba17e940f
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849177"
---
# <a name="channel-resource-type"></a><span data-ttu-id="0a8e1-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="0a8e1-103">channel resource type</span></span>

<span data-ttu-id="0a8e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a8e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a8e1-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="0a8e1-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="0a8e1-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="0a8e1-108">方法</span><span class="sxs-lookup"><span data-stu-id="0a8e1-108">Methods</span></span>

| <span data-ttu-id="0a8e1-109">方法</span><span class="sxs-lookup"><span data-stu-id="0a8e1-109">Method</span></span>       | <span data-ttu-id="0a8e1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0a8e1-110">Return Type</span></span>  |<span data-ttu-id="0a8e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="0a8e1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a8e1-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="0a8e1-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="0a8e1-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="0a8e1-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="0a8e1-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="0a8e1-116">频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-116">channel</span></span>](channel.md) | <span data-ttu-id="0a8e1-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="0a8e1-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="0a8e1-119">频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-119">channel</span></span>](channel.md) | <span data-ttu-id="0a8e1-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="0a8e1-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="0a8e1-122">频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-122">channel</span></span>](channel.md) | <span data-ttu-id="0a8e1-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="0a8e1-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="0a8e1-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="0a8e1-125">无</span><span class="sxs-lookup"><span data-stu-id="0a8e1-125">None</span></span> | <span data-ttu-id="0a8e1-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-126">Delete a channel.</span></span>|
|[<span data-ttu-id="0a8e1-127">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="0a8e1-127">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="0a8e1-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0a8e1-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0a8e1-129">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-129">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="0a8e1-130">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="0a8e1-130">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="0a8e1-131">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0a8e1-131">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0a8e1-132">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="0a8e1-132">Get messages in a channel</span></span> |
|[<span data-ttu-id="0a8e1-133">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="0a8e1-133">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="0a8e1-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0a8e1-134">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="0a8e1-135">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-135">List the members of a channel.</span></span> |
|[<span data-ttu-id="0a8e1-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="0a8e1-136">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="0a8e1-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0a8e1-137">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="0a8e1-138">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-138">Get a member of a channel.</span></span> |
|[<span data-ttu-id="0a8e1-139">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="0a8e1-139">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="0a8e1-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0a8e1-140">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="0a8e1-141">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-141">Add a member to a channel.</span></span> <span data-ttu-id="0a8e1-142">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-142">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="0a8e1-143">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="0a8e1-143">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="0a8e1-144">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0a8e1-144">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="0a8e1-145">更新聊天成员。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-145">Update a member of a channel.</span></span> <span data-ttu-id="0a8e1-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="0a8e1-147">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="0a8e1-147">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="0a8e1-148">conversationMember</span><span class="sxs-lookup"><span data-stu-id="0a8e1-148">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="0a8e1-149">删除频道的成员。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-149">Delete a member of a channel.</span></span> <span data-ttu-id="0a8e1-150">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-150">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="0a8e1-151">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="0a8e1-151">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="0a8e1-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0a8e1-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0a8e1-153">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-153">Send a message to a channel.</span></span> |
|[<span data-ttu-id="0a8e1-154">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="0a8e1-154">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="0a8e1-155">chatMessage</span><span class="sxs-lookup"><span data-stu-id="0a8e1-155">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0a8e1-156">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-156">Reply to a message in a channel.</span></span>|
|[<span data-ttu-id="0a8e1-157">获取文件文件夹</span><span class="sxs-lookup"><span data-stu-id="0a8e1-157">Get files folder</span></span>](../api/driveitem-get.md)| [<span data-ttu-id="0a8e1-158">driveItem</span><span class="sxs-lookup"><span data-stu-id="0a8e1-158">driveItem</span></span>](driveitem.md) | <span data-ttu-id="0a8e1-159">检索用于存储频道文件的 SharePoint 文件夹的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-159">Retrieves the details of the SharePoint folder where the files for the channel are stored.</span></span> |
|[<span data-ttu-id="0a8e1-160">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="0a8e1-160">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="0a8e1-161">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0a8e1-161">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0a8e1-162">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-162">Lists tabs pinned to a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a8e1-163">属性</span><span class="sxs-lookup"><span data-stu-id="0a8e1-163">Properties</span></span>

| <span data-ttu-id="0a8e1-164">属性</span><span class="sxs-lookup"><span data-stu-id="0a8e1-164">Property</span></span>   | <span data-ttu-id="0a8e1-165">类型</span><span class="sxs-lookup"><span data-stu-id="0a8e1-165">Type</span></span> |<span data-ttu-id="0a8e1-166">说明</span><span class="sxs-lookup"><span data-stu-id="0a8e1-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a8e1-167">说明</span><span class="sxs-lookup"><span data-stu-id="0a8e1-167">description</span></span>|<span data-ttu-id="0a8e1-168">String</span><span class="sxs-lookup"><span data-stu-id="0a8e1-168">String</span></span>|<span data-ttu-id="0a8e1-169">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-169">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="0a8e1-170">displayName</span><span class="sxs-lookup"><span data-stu-id="0a8e1-170">displayName</span></span>|<span data-ttu-id="0a8e1-171">String</span><span class="sxs-lookup"><span data-stu-id="0a8e1-171">String</span></span>|<span data-ttu-id="0a8e1-172">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-172">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="0a8e1-173">id</span><span class="sxs-lookup"><span data-stu-id="0a8e1-173">id</span></span>|<span data-ttu-id="0a8e1-174">String</span><span class="sxs-lookup"><span data-stu-id="0a8e1-174">String</span></span>|<span data-ttu-id="0a8e1-175">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-175">The channel's unique identifier.</span></span> <span data-ttu-id="0a8e1-176">只读。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-176">Read-only.</span></span>|
|<span data-ttu-id="0a8e1-177">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="0a8e1-177">isFavoriteByDefault</span></span>|<span data-ttu-id="0a8e1-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a8e1-178">Boolean</span></span>|<span data-ttu-id="0a8e1-179">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-179">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="0a8e1-180">仅可使用“[创建团队](../api/team-post.md)”以编程方式设置。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-180">Can only be set programmatically with [Create team](../api/team-post.md).</span></span> <span data-ttu-id="0a8e1-181">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-181">Default: `false`.</span></span>|
|<span data-ttu-id="0a8e1-182">email</span><span class="sxs-lookup"><span data-stu-id="0a8e1-182">email</span></span>|<span data-ttu-id="0a8e1-183">String</span><span class="sxs-lookup"><span data-stu-id="0a8e1-183">String</span></span>| <span data-ttu-id="0a8e1-184">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-184">The email address for sending messages to the channel.</span></span> <span data-ttu-id="0a8e1-185">只读。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-185">Read-only.</span></span>|
|<span data-ttu-id="0a8e1-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="0a8e1-186">webUrl</span></span>|<span data-ttu-id="0a8e1-187">String</span><span class="sxs-lookup"><span data-stu-id="0a8e1-187">String</span></span>|<span data-ttu-id="0a8e1-188">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-188">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="0a8e1-189">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-189">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="0a8e1-190">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-190">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="0a8e1-191">只读。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-191">Read-only.</span></span>|
|<span data-ttu-id="0a8e1-192">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8e1-192">createdDateTime</span></span>|<span data-ttu-id="0a8e1-193">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8e1-193">dateTimeOffset</span></span>|<span data-ttu-id="0a8e1-194">只读。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-194">Read only.</span></span> <span data-ttu-id="0a8e1-195">创建频道的时间戳。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-195">Timestamp at which the channel was created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a8e1-196">关系</span><span class="sxs-lookup"><span data-stu-id="0a8e1-196">Relationships</span></span>

| <span data-ttu-id="0a8e1-197">关系</span><span class="sxs-lookup"><span data-stu-id="0a8e1-197">Relationship</span></span> | <span data-ttu-id="0a8e1-198">类型</span><span class="sxs-lookup"><span data-stu-id="0a8e1-198">Type</span></span> |<span data-ttu-id="0a8e1-199">说明</span><span class="sxs-lookup"><span data-stu-id="0a8e1-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a8e1-200">messages</span><span class="sxs-lookup"><span data-stu-id="0a8e1-200">messages</span></span>|<span data-ttu-id="0a8e1-201">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0a8e1-201">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="0a8e1-202">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-202">A collection of all the messages in the channel.</span></span> <span data-ttu-id="0a8e1-203">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-203">A navigation property.</span></span> <span data-ttu-id="0a8e1-204">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-204">Nullable.</span></span>|
|<span data-ttu-id="0a8e1-205">选项卡</span><span class="sxs-lookup"><span data-stu-id="0a8e1-205">tabs</span></span>|<span data-ttu-id="0a8e1-206">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0a8e1-206">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="0a8e1-207">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-207">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="0a8e1-208">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-208">A navigation property.</span></span>|
|[<span data-ttu-id="0a8e1-209">filesFolder</span><span class="sxs-lookup"><span data-stu-id="0a8e1-209">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="0a8e1-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="0a8e1-210">driveItem</span></span>](driveitem.md)|<span data-ttu-id="0a8e1-211">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-211">Metadata for the location where the channel's files are stored.</span></span>|
|<span data-ttu-id="0a8e1-212">operations</span><span class="sxs-lookup"><span data-stu-id="0a8e1-212">operations</span></span>|<span data-ttu-id="0a8e1-213">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0a8e1-213">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="0a8e1-214">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-214">The async operations that ran or are running on this team.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a8e1-215">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a8e1-215">JSON representation</span></span>

<span data-ttu-id="0a8e1-216">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a8e1-216">The following is a JSON representation of the resource.</span></span>

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
  "createdDateTime": "string (timestamp)"
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
