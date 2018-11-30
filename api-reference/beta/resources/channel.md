---
title: 通道资源类型
description: '频道是 chatMessages 团队中的集合。 '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048622"
---
# <a name="channel-resource-type"></a><span data-ttu-id="67a36-103">通道资源类型</span><span class="sxs-lookup"><span data-stu-id="67a36-103">channel resource type</span></span>

> <span data-ttu-id="67a36-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="67a36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67a36-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67a36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67a36-106">频道是[chatMessages](chatmessage.md) [团队](../resources/team.md)中的集合。</span><span class="sxs-lookup"><span data-stu-id="67a36-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="67a36-107">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="67a36-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="67a36-108">示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。</span><span class="sxs-lookup"><span data-stu-id="67a36-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="67a36-109">方法</span><span class="sxs-lookup"><span data-stu-id="67a36-109">Methods</span></span>

| <span data-ttu-id="67a36-110">方法</span><span class="sxs-lookup"><span data-stu-id="67a36-110">Method</span></span>       | <span data-ttu-id="67a36-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="67a36-111">Return Type</span></span>  |<span data-ttu-id="67a36-112">说明</span><span class="sxs-lookup"><span data-stu-id="67a36-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="67a36-113">列表通道</span><span class="sxs-lookup"><span data-stu-id="67a36-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="67a36-114">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="67a36-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="67a36-115">此团队中获取通道的列表。</span><span class="sxs-lookup"><span data-stu-id="67a36-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="67a36-116">创建通道</span><span class="sxs-lookup"><span data-stu-id="67a36-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="67a36-117">通道</span><span class="sxs-lookup"><span data-stu-id="67a36-117">channel</span></span>](channel.md) | <span data-ttu-id="67a36-118">创建新的通道通过包括的显示名称和说明。</span><span class="sxs-lookup"><span data-stu-id="67a36-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="67a36-119">获取通道</span><span class="sxs-lookup"><span data-stu-id="67a36-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="67a36-120">通道</span><span class="sxs-lookup"><span data-stu-id="67a36-120">channel</span></span>](channel.md) | <span data-ttu-id="67a36-121">读取属性和该频道的关系。</span><span class="sxs-lookup"><span data-stu-id="67a36-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="67a36-122">更新通道</span><span class="sxs-lookup"><span data-stu-id="67a36-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="67a36-123">通道</span><span class="sxs-lookup"><span data-stu-id="67a36-123">channel</span></span>](channel.md) | <span data-ttu-id="67a36-124">更新该频道的属性。</span><span class="sxs-lookup"><span data-stu-id="67a36-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="67a36-125">删除通道</span><span class="sxs-lookup"><span data-stu-id="67a36-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="67a36-126">无</span><span class="sxs-lookup"><span data-stu-id="67a36-126">None</span></span> | <span data-ttu-id="67a36-127">删除通道。</span><span class="sxs-lookup"><span data-stu-id="67a36-127">Delete a channel.</span></span>|
|[<span data-ttu-id="67a36-128">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="67a36-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="67a36-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="67a36-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="67a36-130">在通道中收到消息</span><span class="sxs-lookup"><span data-stu-id="67a36-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="67a36-131">创建聊天线程</span><span class="sxs-lookup"><span data-stu-id="67a36-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="67a36-132">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="67a36-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="67a36-133">创建在指定的频道的聊天线程。</span><span class="sxs-lookup"><span data-stu-id="67a36-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="67a36-134">属性</span><span class="sxs-lookup"><span data-stu-id="67a36-134">Properties</span></span>
| <span data-ttu-id="67a36-135">属性</span><span class="sxs-lookup"><span data-stu-id="67a36-135">Property</span></span>     | <span data-ttu-id="67a36-136">类型</span><span class="sxs-lookup"><span data-stu-id="67a36-136">Type</span></span>   |<span data-ttu-id="67a36-137">说明</span><span class="sxs-lookup"><span data-stu-id="67a36-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67a36-138">说明</span><span class="sxs-lookup"><span data-stu-id="67a36-138">description</span></span>|<span data-ttu-id="67a36-139">字符串</span><span class="sxs-lookup"><span data-stu-id="67a36-139">String</span></span>|<span data-ttu-id="67a36-140">通道的可选文字说明。</span><span class="sxs-lookup"><span data-stu-id="67a36-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="67a36-141">displayName</span><span class="sxs-lookup"><span data-stu-id="67a36-141">displayName</span></span>|<span data-ttu-id="67a36-142">字符串</span><span class="sxs-lookup"><span data-stu-id="67a36-142">String</span></span>|<span data-ttu-id="67a36-143">通道名称将显示于 Microsoft 团队中的用户。</span><span class="sxs-lookup"><span data-stu-id="67a36-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="67a36-144">id</span><span class="sxs-lookup"><span data-stu-id="67a36-144">id</span></span>|<span data-ttu-id="67a36-145">字符串</span><span class="sxs-lookup"><span data-stu-id="67a36-145">String</span></span>|<span data-ttu-id="67a36-146">通道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67a36-146">The channels's unique identifier.</span></span> <span data-ttu-id="67a36-147">只读。</span><span class="sxs-lookup"><span data-stu-id="67a36-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67a36-148">Relationships</span><span class="sxs-lookup"><span data-stu-id="67a36-148">Relationships</span></span>
| <span data-ttu-id="67a36-149">关系</span><span class="sxs-lookup"><span data-stu-id="67a36-149">Relationship</span></span> | <span data-ttu-id="67a36-150">类型</span><span class="sxs-lookup"><span data-stu-id="67a36-150">Type</span></span>   |<span data-ttu-id="67a36-151">说明</span><span class="sxs-lookup"><span data-stu-id="67a36-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67a36-152">messages</span><span class="sxs-lookup"><span data-stu-id="67a36-152">messages</span></span>|<span data-ttu-id="67a36-153">[chatMessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="67a36-153">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="67a36-154">在进入频道的所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="67a36-154">A collection of all the messages in the channel.</span></span> <span data-ttu-id="67a36-155">导航属性。</span><span class="sxs-lookup"><span data-stu-id="67a36-155">A navigation property.</span></span> <span data-ttu-id="67a36-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="67a36-156">Nullable.</span></span> <span data-ttu-id="67a36-157">目前此 API 仅支持读取，但将最终太支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="67a36-157">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="67a36-158">chatThreads</span><span class="sxs-lookup"><span data-stu-id="67a36-158">chatThreads</span></span>|<span data-ttu-id="67a36-159">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="67a36-159">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="67a36-160">（这被淘汰以消息属性应用） chatThreads 支持创建新邮件，但未阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="67a36-160">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="67a36-161">ChatThreads 是导航属性，并且是可以为 Null。</span><span class="sxs-lookup"><span data-stu-id="67a36-161">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="67a36-162">选项卡</span><span class="sxs-lookup"><span data-stu-id="67a36-162">tabs</span></span>|<span data-ttu-id="67a36-163">[teamsTab](../resources/teamstab.md)集合</span><span class="sxs-lookup"><span data-stu-id="67a36-163">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="67a36-164">在进入频道的所有选项卡的集合。</span><span class="sxs-lookup"><span data-stu-id="67a36-164">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="67a36-165">导航属性。</span><span class="sxs-lookup"><span data-stu-id="67a36-165">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="67a36-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67a36-166">JSON representation</span></span>

<span data-ttu-id="67a36-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67a36-167">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
