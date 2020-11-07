---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 59a6b111c08b6bfb408b1f28b4db343843ed12ad
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932582"
---
# <a name="channel-resource-type"></a><span data-ttu-id="6aa41-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="6aa41-103">channel resource type</span></span>

<span data-ttu-id="6aa41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aa41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6aa41-p101">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates. Each channel is dedicated to a specific topic, department, or project. Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p101">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates. Each channel is dedicated to a specific topic, department, or project. Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="6aa41-108">方法</span><span class="sxs-lookup"><span data-stu-id="6aa41-108">Methods</span></span>

| <span data-ttu-id="6aa41-109">方法</span><span class="sxs-lookup"><span data-stu-id="6aa41-109">Method</span></span>       | <span data-ttu-id="6aa41-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6aa41-110">Return Type</span></span>  |<span data-ttu-id="6aa41-111">说明</span><span class="sxs-lookup"><span data-stu-id="6aa41-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6aa41-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="6aa41-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="6aa41-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="6aa41-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="6aa41-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="6aa41-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="6aa41-116">频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-116">channel</span></span>](channel.md) | <span data-ttu-id="6aa41-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="6aa41-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="6aa41-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="6aa41-119">频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-119">channel</span></span>](channel.md) | <span data-ttu-id="6aa41-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6aa41-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="6aa41-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="6aa41-122">频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-122">channel</span></span>](channel.md) | <span data-ttu-id="6aa41-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="6aa41-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="6aa41-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="6aa41-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="6aa41-125">无</span><span class="sxs-lookup"><span data-stu-id="6aa41-125">None</span></span> | <span data-ttu-id="6aa41-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="6aa41-126">Delete a channel.</span></span>|
|[<span data-ttu-id="6aa41-127">获取消息 Delta</span><span class="sxs-lookup"><span data-stu-id="6aa41-127">Get message delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="6aa41-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6aa41-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6aa41-129">获取频道中的增量消息。</span><span class="sxs-lookup"><span data-stu-id="6aa41-129">Get incremental messages in a channel.</span></span> |
|[<span data-ttu-id="6aa41-130">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="6aa41-130">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="6aa41-131">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6aa41-131">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6aa41-132">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="6aa41-132">Get messages in a channel</span></span> |
|[<span data-ttu-id="6aa41-133">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="6aa41-133">List channel members</span></span>](../api/conversationmember-list.md)| <span data-ttu-id="6aa41-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6aa41-134">[conversationMember](conversationmember.md) collection</span></span>| <span data-ttu-id="6aa41-135">列出频道的成员。</span><span class="sxs-lookup"><span data-stu-id="6aa41-135">List the members of a channel.</span></span> |
|[<span data-ttu-id="6aa41-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="6aa41-136">Get channel member</span></span>](../api/conversationmember-get.md)| [<span data-ttu-id="6aa41-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6aa41-137">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="6aa41-138">获取频道的成员。</span><span class="sxs-lookup"><span data-stu-id="6aa41-138">Get a member of a channel.</span></span> |
|[<span data-ttu-id="6aa41-139">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="6aa41-139">Add channel member</span></span>](../api/conversationmember-add.md) | [<span data-ttu-id="6aa41-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6aa41-140">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="6aa41-p102">Add a member to a channel. Only supported for `channelType` of `private`.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p102">Add a member to a channel. Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="6aa41-143">更新频道成员</span><span class="sxs-lookup"><span data-stu-id="6aa41-143">Update channel member</span></span>](../api/conversationmember-update.md) | [<span data-ttu-id="6aa41-144">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6aa41-144">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="6aa41-p103">Update a member of a channel. Only supported for `channelType` of `private`.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p103">Update a member of a channel. Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="6aa41-147">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="6aa41-147">Delete channel member</span></span>](../api/conversationmember-delete.md) | [<span data-ttu-id="6aa41-148">conversationMember</span><span class="sxs-lookup"><span data-stu-id="6aa41-148">conversationMember</span></span>](conversationmember.md)| <span data-ttu-id="6aa41-p104">Delete a member of a channel. Only supported for `channelType` of `private`.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p104">Delete a member of a channel. Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="6aa41-151">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="6aa41-151">Create chatMessage in a channel</span></span>](../api/channel-post-message.md) | [<span data-ttu-id="6aa41-152">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6aa41-152">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6aa41-153">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="6aa41-153">Send a message to a channel.</span></span> |
|[<span data-ttu-id="6aa41-154">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="6aa41-154">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="6aa41-155">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6aa41-155">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6aa41-156">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="6aa41-156">Reply to a message in a channel.</span></span>|
|[<span data-ttu-id="6aa41-157">获取文件文件夹</span><span class="sxs-lookup"><span data-stu-id="6aa41-157">Get files folder</span></span>](../api/driveitem-get.md)| [<span data-ttu-id="6aa41-158">driveItem</span><span class="sxs-lookup"><span data-stu-id="6aa41-158">driveItem</span></span>](driveitem.md) | <span data-ttu-id="6aa41-159">检索用于存储频道文件的 SharePoint 文件夹的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6aa41-159">Retrieves the details of the SharePoint folder where the files for the channel are stored.</span></span> |
|[<span data-ttu-id="6aa41-160">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="6aa41-160">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="6aa41-161">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6aa41-161">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6aa41-162">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="6aa41-162">Lists tabs pinned to a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="6aa41-163">属性</span><span class="sxs-lookup"><span data-stu-id="6aa41-163">Properties</span></span>

| <span data-ttu-id="6aa41-164">属性</span><span class="sxs-lookup"><span data-stu-id="6aa41-164">Property</span></span>   | <span data-ttu-id="6aa41-165">类型</span><span class="sxs-lookup"><span data-stu-id="6aa41-165">Type</span></span> |<span data-ttu-id="6aa41-166">说明</span><span class="sxs-lookup"><span data-stu-id="6aa41-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6aa41-167">说明</span><span class="sxs-lookup"><span data-stu-id="6aa41-167">description</span></span>|<span data-ttu-id="6aa41-168">String</span><span class="sxs-lookup"><span data-stu-id="6aa41-168">String</span></span>|<span data-ttu-id="6aa41-169">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="6aa41-169">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="6aa41-170">displayName</span><span class="sxs-lookup"><span data-stu-id="6aa41-170">displayName</span></span>|<span data-ttu-id="6aa41-171">String</span><span class="sxs-lookup"><span data-stu-id="6aa41-171">String</span></span>|<span data-ttu-id="6aa41-172">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="6aa41-172">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="6aa41-173">id</span><span class="sxs-lookup"><span data-stu-id="6aa41-173">id</span></span>|<span data-ttu-id="6aa41-174">String</span><span class="sxs-lookup"><span data-stu-id="6aa41-174">String</span></span>|<span data-ttu-id="6aa41-p105">The channel's unique identifier. Read-only.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p105">The channel's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="6aa41-177">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="6aa41-177">isFavoriteByDefault</span></span>|<span data-ttu-id="6aa41-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aa41-178">Boolean</span></span>|<span data-ttu-id="6aa41-p106">Indicates whether the channel should automatically be marked 'favorite' for all members of the team. Can only be set programmatically with [Create team](../api/team-post.md). Default: `false`.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p106">Indicates whether the channel should automatically be marked 'favorite' for all members of the team. Can only be set programmatically with [Create team](../api/team-post.md). Default: `false`.</span></span>|
|<span data-ttu-id="6aa41-182">email</span><span class="sxs-lookup"><span data-stu-id="6aa41-182">email</span></span>|<span data-ttu-id="6aa41-183">String</span><span class="sxs-lookup"><span data-stu-id="6aa41-183">String</span></span>| <span data-ttu-id="6aa41-p107">The email address for sending messages to the channel. Read-only.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p107">The email address for sending messages to the channel. Read-only.</span></span>|
|<span data-ttu-id="6aa41-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="6aa41-186">webUrl</span></span>|<span data-ttu-id="6aa41-187">String</span><span class="sxs-lookup"><span data-stu-id="6aa41-187">String</span></span>|<span data-ttu-id="6aa41-p108">A hyperlink that will go to the channel in Microsoft Teams. This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel. This URL should be treated as an opaque blob, and not parsed. Read-only.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p108">A hyperlink that will go to the channel in Microsoft Teams. This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel. This URL should be treated as an opaque blob, and not parsed. Read-only.</span></span>|
|<span data-ttu-id="6aa41-192">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6aa41-192">createdDateTime</span></span>|<span data-ttu-id="6aa41-193">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aa41-193">dateTimeOffset</span></span>|<span data-ttu-id="6aa41-p109">Read only. Timestamp at which the channel was created.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p109">Read only. Timestamp at which the channel was created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6aa41-196">关系</span><span class="sxs-lookup"><span data-stu-id="6aa41-196">Relationships</span></span>

| <span data-ttu-id="6aa41-197">关系</span><span class="sxs-lookup"><span data-stu-id="6aa41-197">Relationship</span></span> | <span data-ttu-id="6aa41-198">类型</span><span class="sxs-lookup"><span data-stu-id="6aa41-198">Type</span></span> |<span data-ttu-id="6aa41-199">说明</span><span class="sxs-lookup"><span data-stu-id="6aa41-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6aa41-200">messages</span><span class="sxs-lookup"><span data-stu-id="6aa41-200">messages</span></span>|<span data-ttu-id="6aa41-201">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6aa41-201">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="6aa41-p110">A collection of all the messages in the channel. A navigation property. Nullable.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p110">A collection of all the messages in the channel. A navigation property. Nullable.</span></span>|
|<span data-ttu-id="6aa41-205">选项卡</span><span class="sxs-lookup"><span data-stu-id="6aa41-205">tabs</span></span>|<span data-ttu-id="6aa41-206">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6aa41-206">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="6aa41-p111">A collection of all the tabs in the channel. A navigation property.</span><span class="sxs-lookup"><span data-stu-id="6aa41-p111">A collection of all the tabs in the channel. A navigation property.</span></span>|
|[<span data-ttu-id="6aa41-209">filesFolder</span><span class="sxs-lookup"><span data-stu-id="6aa41-209">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="6aa41-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="6aa41-210">driveItem</span></span>](driveitem.md)|<span data-ttu-id="6aa41-211">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="6aa41-211">Metadata for the location where the channel's files are stored.</span></span>|
|<span data-ttu-id="6aa41-212">operations</span><span class="sxs-lookup"><span data-stu-id="6aa41-212">operations</span></span>|<span data-ttu-id="6aa41-213">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6aa41-213">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="6aa41-214">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="6aa41-214">The async operations that ran or are running on this team.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6aa41-215">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6aa41-215">JSON representation</span></span>

<span data-ttu-id="6aa41-216">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6aa41-216">The following is a JSON representation of the resource.</span></span>

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
