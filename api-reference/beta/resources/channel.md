---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8b284cdfef42e9eb3319fc51c17febcf02eba1a1
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709430"
---
# <a name="channel-resource-type"></a><span data-ttu-id="83297-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="83297-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83297-104">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="83297-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="83297-105">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="83297-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="83297-106">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="83297-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="83297-107">方法</span><span class="sxs-lookup"><span data-stu-id="83297-107">Methods</span></span>

| <span data-ttu-id="83297-108">方法</span><span class="sxs-lookup"><span data-stu-id="83297-108">Method</span></span>       | <span data-ttu-id="83297-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="83297-109">Return Type</span></span>  |<span data-ttu-id="83297-110">说明</span><span class="sxs-lookup"><span data-stu-id="83297-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83297-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="83297-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="83297-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="83297-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="83297-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="83297-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="83297-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="83297-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="83297-115">频道</span><span class="sxs-lookup"><span data-stu-id="83297-115">channel</span></span>](channel.md) | <span data-ttu-id="83297-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="83297-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="83297-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="83297-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="83297-118">频道</span><span class="sxs-lookup"><span data-stu-id="83297-118">channel</span></span>](channel.md) | <span data-ttu-id="83297-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83297-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="83297-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="83297-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="83297-121">频道</span><span class="sxs-lookup"><span data-stu-id="83297-121">channel</span></span>](channel.md) | <span data-ttu-id="83297-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="83297-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="83297-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="83297-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="83297-124">无</span><span class="sxs-lookup"><span data-stu-id="83297-124">None</span></span> | <span data-ttu-id="83297-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="83297-125">Delete a channel.</span></span>|
|[<span data-ttu-id="83297-126">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="83297-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="83297-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="83297-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="83297-128">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="83297-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="83297-129">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="83297-129">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="83297-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="83297-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="83297-131">向频道发送消息。</span><span class="sxs-lookup"><span data-stu-id="83297-131">Send a message to a channel</span></span> |
|[<span data-ttu-id="83297-132">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="83297-132">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="83297-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="83297-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="83297-134">在频道中回复消息。</span><span class="sxs-lookup"><span data-stu-id="83297-134">Reply to a message in a channel</span></span>|
|[<span data-ttu-id="83297-135">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="83297-135">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="83297-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="83297-136">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="83297-137">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="83297-137">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="83297-138">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="83297-138">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="83297-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="83297-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="83297-140">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="83297-140">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="83297-141">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="83297-141">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="83297-142">teamsTab</span><span class="sxs-lookup"><span data-stu-id="83297-142">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="83297-143">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="83297-143">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="83297-144">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="83297-144">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="83297-145">无</span><span class="sxs-lookup"><span data-stu-id="83297-145">None</span></span> | <span data-ttu-id="83297-146">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="83297-146">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="83297-147">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="83297-147">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="83297-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="83297-148">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="83297-149">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="83297-149">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="83297-150">属性</span><span class="sxs-lookup"><span data-stu-id="83297-150">Properties</span></span>
| <span data-ttu-id="83297-151">属性</span><span class="sxs-lookup"><span data-stu-id="83297-151">Property</span></span>     | <span data-ttu-id="83297-152">类型</span><span class="sxs-lookup"><span data-stu-id="83297-152">Type</span></span>   |<span data-ttu-id="83297-153">说明</span><span class="sxs-lookup"><span data-stu-id="83297-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83297-154">说明</span><span class="sxs-lookup"><span data-stu-id="83297-154">description</span></span>|<span data-ttu-id="83297-155">String</span><span class="sxs-lookup"><span data-stu-id="83297-155">String</span></span>|<span data-ttu-id="83297-156">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="83297-156">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="83297-157">displayName</span><span class="sxs-lookup"><span data-stu-id="83297-157">displayName</span></span>|<span data-ttu-id="83297-158">String</span><span class="sxs-lookup"><span data-stu-id="83297-158">String</span></span>|<span data-ttu-id="83297-159">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="83297-159">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="83297-160">id</span><span class="sxs-lookup"><span data-stu-id="83297-160">id</span></span>|<span data-ttu-id="83297-161">String</span><span class="sxs-lookup"><span data-stu-id="83297-161">String</span></span>|<span data-ttu-id="83297-162">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="83297-162">The channels's unique identifier.</span></span> <span data-ttu-id="83297-163">只读。</span><span class="sxs-lookup"><span data-stu-id="83297-163">Read-only.</span></span>|
|<span data-ttu-id="83297-164">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="83297-164">isFavoriteByDefault</span></span>|<span data-ttu-id="83297-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="83297-165">Boolean</span></span>|<span data-ttu-id="83297-166">频道是否对团队所有成员标记为“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="83297-166">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="83297-167">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="83297-167">Default: `false`.</span></span>|
|<span data-ttu-id="83297-168">email</span><span class="sxs-lookup"><span data-stu-id="83297-168">email</span></span>|<span data-ttu-id="83297-169">String</span><span class="sxs-lookup"><span data-stu-id="83297-169">String</span></span>| <span data-ttu-id="83297-170">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="83297-170">The email address for sending messages to the channel.</span></span> <span data-ttu-id="83297-171">只读。</span><span class="sxs-lookup"><span data-stu-id="83297-171">Read-only.</span></span>|
|<span data-ttu-id="83297-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="83297-172">webUrl</span></span>|<span data-ttu-id="83297-173">String</span><span class="sxs-lookup"><span data-stu-id="83297-173">String</span></span>|<span data-ttu-id="83297-174">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="83297-174">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="83297-175">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="83297-175">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="83297-176">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="83297-176">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="83297-177">只读。</span><span class="sxs-lookup"><span data-stu-id="83297-177">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="83297-178">关系</span><span class="sxs-lookup"><span data-stu-id="83297-178">Relationships</span></span>
| <span data-ttu-id="83297-179">关系</span><span class="sxs-lookup"><span data-stu-id="83297-179">Relationship</span></span> | <span data-ttu-id="83297-180">类型</span><span class="sxs-lookup"><span data-stu-id="83297-180">Type</span></span>   |<span data-ttu-id="83297-181">说明</span><span class="sxs-lookup"><span data-stu-id="83297-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83297-182">messages</span><span class="sxs-lookup"><span data-stu-id="83297-182">messages</span></span>|<span data-ttu-id="83297-183">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83297-183">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="83297-184">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="83297-184">A collection of all the messages in the channel.</span></span> <span data-ttu-id="83297-185">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="83297-185">A navigation property.</span></span> <span data-ttu-id="83297-186">可为空。</span><span class="sxs-lookup"><span data-stu-id="83297-186">Nullable.</span></span> <span data-ttu-id="83297-187">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="83297-187">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="83297-188">选项卡</span><span class="sxs-lookup"><span data-stu-id="83297-188">tabs</span></span>|<span data-ttu-id="83297-189">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83297-189">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="83297-190">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="83297-190">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="83297-191">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="83297-191">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="83297-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83297-192">JSON representation</span></span>

<span data-ttu-id="83297-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83297-193">Here is a JSON representation of the resource</span></span>

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
