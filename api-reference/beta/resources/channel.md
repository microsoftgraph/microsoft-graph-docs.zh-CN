---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994466"
---
# <a name="channel-resource-type"></a><span data-ttu-id="98ad2-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="98ad2-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98ad2-104">频道是的[团队](../resources/team.md)中的 [chatMessages](chatmessage.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="98ad2-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="98ad2-105">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="98ad2-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="98ad2-106">示例可以是“星期五团队午餐”和“体系结构讨论”频道。</span><span class="sxs-lookup"><span data-stu-id="98ad2-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="98ad2-107">方法</span><span class="sxs-lookup"><span data-stu-id="98ad2-107">Methods</span></span>

| <span data-ttu-id="98ad2-108">方法</span><span class="sxs-lookup"><span data-stu-id="98ad2-108">Method</span></span>       | <span data-ttu-id="98ad2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="98ad2-109">Return Type</span></span>  |<span data-ttu-id="98ad2-110">说明</span><span class="sxs-lookup"><span data-stu-id="98ad2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98ad2-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="98ad2-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="98ad2-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="98ad2-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="98ad2-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="98ad2-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="98ad2-115">频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-115">channel</span></span>](channel.md) | <span data-ttu-id="98ad2-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="98ad2-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="98ad2-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="98ad2-118">频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-118">channel</span></span>](channel.md) | <span data-ttu-id="98ad2-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98ad2-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="98ad2-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="98ad2-121">频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-121">channel</span></span>](channel.md) | <span data-ttu-id="98ad2-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="98ad2-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="98ad2-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="98ad2-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="98ad2-124">无</span><span class="sxs-lookup"><span data-stu-id="98ad2-124">None</span></span> | <span data-ttu-id="98ad2-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="98ad2-125">Delete a channel.</span></span>|
|[<span data-ttu-id="98ad2-126">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="98ad2-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="98ad2-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="98ad2-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="98ad2-128">获取频道中的消息</span><span class="sxs-lookup"><span data-stu-id="98ad2-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="98ad2-129">发送渠道消息</span><span class="sxs-lookup"><span data-stu-id="98ad2-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="98ad2-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="98ad2-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="98ad2-131">向渠道发送消息</span><span class="sxs-lookup"><span data-stu-id="98ad2-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |


## <a name="properties"></a><span data-ttu-id="98ad2-132">属性</span><span class="sxs-lookup"><span data-stu-id="98ad2-132">Properties</span></span>
| <span data-ttu-id="98ad2-133">属性</span><span class="sxs-lookup"><span data-stu-id="98ad2-133">Property</span></span>     | <span data-ttu-id="98ad2-134">类型</span><span class="sxs-lookup"><span data-stu-id="98ad2-134">Type</span></span>   |<span data-ttu-id="98ad2-135">说明</span><span class="sxs-lookup"><span data-stu-id="98ad2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98ad2-136">说明</span><span class="sxs-lookup"><span data-stu-id="98ad2-136">description</span></span>|<span data-ttu-id="98ad2-137">String</span><span class="sxs-lookup"><span data-stu-id="98ad2-137">String</span></span>|<span data-ttu-id="98ad2-138">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="98ad2-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="98ad2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="98ad2-139">displayName</span></span>|<span data-ttu-id="98ad2-140">String</span><span class="sxs-lookup"><span data-stu-id="98ad2-140">String</span></span>|<span data-ttu-id="98ad2-141">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="98ad2-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="98ad2-142">id</span><span class="sxs-lookup"><span data-stu-id="98ad2-142">id</span></span>|<span data-ttu-id="98ad2-143">String</span><span class="sxs-lookup"><span data-stu-id="98ad2-143">String</span></span>|<span data-ttu-id="98ad2-144">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="98ad2-144">The channels's unique identifier.</span></span> <span data-ttu-id="98ad2-145">只读。</span><span class="sxs-lookup"><span data-stu-id="98ad2-145">Read-only.</span></span>|
|<span data-ttu-id="98ad2-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="98ad2-146">isFavoriteByDefault</span></span>|<span data-ttu-id="98ad2-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="98ad2-147">Boolean</span></span>|<span data-ttu-id="98ad2-148">频道是否对团队所有成员标记为“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="98ad2-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="98ad2-149">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="98ad2-149">Default: `false`.</span></span>|
|<span data-ttu-id="98ad2-150">电子邮件</span><span class="sxs-lookup"><span data-stu-id="98ad2-150">email</span></span>|<span data-ttu-id="98ad2-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="98ad2-151">Boolean</span></span>| <span data-ttu-id="98ad2-152">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="98ad2-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="98ad2-153">只读。</span><span class="sxs-lookup"><span data-stu-id="98ad2-153">Read-only.</span></span>|
|<span data-ttu-id="98ad2-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="98ad2-154">webUrl</span></span>|<span data-ttu-id="98ad2-155">String</span><span class="sxs-lookup"><span data-stu-id="98ad2-155">String</span></span>|<span data-ttu-id="98ad2-156">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="98ad2-156">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="98ad2-157">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="98ad2-157">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="98ad2-158">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="98ad2-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="98ad2-159">只读。</span><span class="sxs-lookup"><span data-stu-id="98ad2-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="98ad2-160">关系</span><span class="sxs-lookup"><span data-stu-id="98ad2-160">Relationships</span></span>
| <span data-ttu-id="98ad2-161">关系</span><span class="sxs-lookup"><span data-stu-id="98ad2-161">Relationship</span></span> | <span data-ttu-id="98ad2-162">类型</span><span class="sxs-lookup"><span data-stu-id="98ad2-162">Type</span></span>   |<span data-ttu-id="98ad2-163">说明</span><span class="sxs-lookup"><span data-stu-id="98ad2-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98ad2-164">messages</span><span class="sxs-lookup"><span data-stu-id="98ad2-164">messages</span></span>|<span data-ttu-id="98ad2-165">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98ad2-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="98ad2-166">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="98ad2-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="98ad2-167">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="98ad2-167">A navigation property.</span></span> <span data-ttu-id="98ad2-168">可为空。</span><span class="sxs-lookup"><span data-stu-id="98ad2-168">Nullable.</span></span> <span data-ttu-id="98ad2-169">此 API 目前仅支持读取消息，但最终也会支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="98ad2-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="98ad2-170">选项卡</span><span class="sxs-lookup"><span data-stu-id="98ad2-170">tabs</span></span>|<span data-ttu-id="98ad2-171">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98ad2-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="98ad2-172">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="98ad2-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="98ad2-173">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="98ad2-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="98ad2-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98ad2-174">JSON representation</span></span>

<span data-ttu-id="98ad2-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98ad2-175">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
