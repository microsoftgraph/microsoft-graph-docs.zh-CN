---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1b77afb1560ed451683838a617123db013b71cd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338759"
---
# <a name="channel-resource-type"></a><span data-ttu-id="4f4f9-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="4f4f9-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f4f9-104">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="4f4f9-105">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="4f4f9-106">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="4f4f9-107">方法</span><span class="sxs-lookup"><span data-stu-id="4f4f9-107">Methods</span></span>

| <span data-ttu-id="4f4f9-108">方法</span><span class="sxs-lookup"><span data-stu-id="4f4f9-108">Method</span></span>       | <span data-ttu-id="4f4f9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f4f9-109">Return Type</span></span>  |<span data-ttu-id="4f4f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="4f4f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f4f9-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="4f4f9-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f4f9-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="4f4f9-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="4f4f9-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="4f4f9-115">频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-115">channel</span></span>](channel.md) | <span data-ttu-id="4f4f9-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="4f4f9-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="4f4f9-118">频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-118">channel</span></span>](channel.md) | <span data-ttu-id="4f4f9-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="4f4f9-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="4f4f9-121">频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-121">channel</span></span>](channel.md) | <span data-ttu-id="4f4f9-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="4f4f9-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="4f4f9-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="4f4f9-124">无</span><span class="sxs-lookup"><span data-stu-id="4f4f9-124">None</span></span> | <span data-ttu-id="4f4f9-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-125">Delete a channel.</span></span>|
|[<span data-ttu-id="4f4f9-126">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="4f4f9-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="4f4f9-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4f4f9-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4f4f9-128">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="4f4f9-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="4f4f9-129">发送渠道消息</span><span class="sxs-lookup"><span data-stu-id="4f4f9-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="4f4f9-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4f4f9-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="4f4f9-131">向渠道发送消息</span><span class="sxs-lookup"><span data-stu-id="4f4f9-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |
|[<span data-ttu-id="4f4f9-132">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="4f4f9-132">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="4f4f9-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4f4f9-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4f4f9-134">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-134">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="4f4f9-135">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="4f4f9-135">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="4f4f9-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4f4f9-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4f4f9-137">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-137">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="4f4f9-138">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="4f4f9-138">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4f4f9-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4f4f9-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4f4f9-140">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-140">Adds (installs) a tab to a team's channel.</span></span>|
|[<span data-ttu-id="4f4f9-141">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="4f4f9-141">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="4f4f9-142">无</span><span class="sxs-lookup"><span data-stu-id="4f4f9-142">None</span></span> | <span data-ttu-id="4f4f9-143">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-143">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="4f4f9-144">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="4f4f9-144">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="4f4f9-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4f4f9-145">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4f4f9-146">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-146">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="4f4f9-147">属性</span><span class="sxs-lookup"><span data-stu-id="4f4f9-147">Properties</span></span>
| <span data-ttu-id="4f4f9-148">属性</span><span class="sxs-lookup"><span data-stu-id="4f4f9-148">Property</span></span>     | <span data-ttu-id="4f4f9-149">类型</span><span class="sxs-lookup"><span data-stu-id="4f4f9-149">Type</span></span>   |<span data-ttu-id="4f4f9-150">说明</span><span class="sxs-lookup"><span data-stu-id="4f4f9-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f4f9-151">说明</span><span class="sxs-lookup"><span data-stu-id="4f4f9-151">description</span></span>|<span data-ttu-id="4f4f9-152">String</span><span class="sxs-lookup"><span data-stu-id="4f4f9-152">String</span></span>|<span data-ttu-id="4f4f9-153">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-153">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="4f4f9-154">displayName</span><span class="sxs-lookup"><span data-stu-id="4f4f9-154">displayName</span></span>|<span data-ttu-id="4f4f9-155">String</span><span class="sxs-lookup"><span data-stu-id="4f4f9-155">String</span></span>|<span data-ttu-id="4f4f9-156">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-156">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="4f4f9-157">id</span><span class="sxs-lookup"><span data-stu-id="4f4f9-157">id</span></span>|<span data-ttu-id="4f4f9-158">String</span><span class="sxs-lookup"><span data-stu-id="4f4f9-158">String</span></span>|<span data-ttu-id="4f4f9-159">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-159">The channels's unique identifier.</span></span> <span data-ttu-id="4f4f9-160">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-160">Read-only.</span></span>|
|<span data-ttu-id="4f4f9-161">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="4f4f9-161">isFavoriteByDefault</span></span>|<span data-ttu-id="4f4f9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4f9-162">Boolean</span></span>|<span data-ttu-id="4f4f9-163">频道是否对团队所有成员标记为“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-163">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="4f4f9-164">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-164">Default: `false`.</span></span>|
|<span data-ttu-id="4f4f9-165">email</span><span class="sxs-lookup"><span data-stu-id="4f4f9-165">email</span></span>|<span data-ttu-id="4f4f9-166">String</span><span class="sxs-lookup"><span data-stu-id="4f4f9-166">String</span></span>| <span data-ttu-id="4f4f9-167">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-167">The email address for sending messages to the channel.</span></span> <span data-ttu-id="4f4f9-168">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-168">Read-only.</span></span>|
|<span data-ttu-id="4f4f9-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="4f4f9-169">webUrl</span></span>|<span data-ttu-id="4f4f9-170">String</span><span class="sxs-lookup"><span data-stu-id="4f4f9-170">String</span></span>|<span data-ttu-id="4f4f9-171">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-171">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="4f4f9-172">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-172">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="4f4f9-173">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-173">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="4f4f9-174">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-174">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4f4f9-175">关系</span><span class="sxs-lookup"><span data-stu-id="4f4f9-175">Relationships</span></span>
| <span data-ttu-id="4f4f9-176">关系</span><span class="sxs-lookup"><span data-stu-id="4f4f9-176">Relationship</span></span> | <span data-ttu-id="4f4f9-177">类型</span><span class="sxs-lookup"><span data-stu-id="4f4f9-177">Type</span></span>   |<span data-ttu-id="4f4f9-178">说明</span><span class="sxs-lookup"><span data-stu-id="4f4f9-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f4f9-179">messages</span><span class="sxs-lookup"><span data-stu-id="4f4f9-179">messages</span></span>|<span data-ttu-id="4f4f9-180">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f4f9-180">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="4f4f9-181">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-181">A collection of all the messages in the channel.</span></span> <span data-ttu-id="4f4f9-182">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-182">A navigation property.</span></span> <span data-ttu-id="4f4f9-183">可为空。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-183">Nullable.</span></span> <span data-ttu-id="4f4f9-184">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-184">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="4f4f9-185">选项卡</span><span class="sxs-lookup"><span data-stu-id="4f4f9-185">tabs</span></span>|<span data-ttu-id="4f4f9-186">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f4f9-186">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="4f4f9-187">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-187">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="4f4f9-188">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-188">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4f4f9-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f4f9-189">JSON representation</span></span>

<span data-ttu-id="4f4f9-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f4f9-190">Here is a JSON representation of the resource</span></span>

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
  "webUrl": "string"
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
