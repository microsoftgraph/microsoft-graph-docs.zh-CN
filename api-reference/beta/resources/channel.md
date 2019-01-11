---
title: 通道资源类型
description: '频道是 chatMessages 团队中的集合。 '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 058632c9f56462195db0cd268fd0af262d4292f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842684"
---
# <a name="channel-resource-type"></a><span data-ttu-id="b167d-103">通道资源类型</span><span class="sxs-lookup"><span data-stu-id="b167d-103">channel resource type</span></span>

> <span data-ttu-id="b167d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b167d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b167d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b167d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b167d-106">频道是[chatMessages](chatmessage.md) [团队](../resources/team.md)中的集合。</span><span class="sxs-lookup"><span data-stu-id="b167d-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="b167d-107">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="b167d-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="b167d-108">示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。</span><span class="sxs-lookup"><span data-stu-id="b167d-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="b167d-109">方法</span><span class="sxs-lookup"><span data-stu-id="b167d-109">Methods</span></span>

| <span data-ttu-id="b167d-110">方法</span><span class="sxs-lookup"><span data-stu-id="b167d-110">Method</span></span>       | <span data-ttu-id="b167d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b167d-111">Return Type</span></span>  |<span data-ttu-id="b167d-112">说明</span><span class="sxs-lookup"><span data-stu-id="b167d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b167d-113">列表通道</span><span class="sxs-lookup"><span data-stu-id="b167d-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="b167d-114">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="b167d-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="b167d-115">此团队中获取通道的列表。</span><span class="sxs-lookup"><span data-stu-id="b167d-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="b167d-116">创建通道</span><span class="sxs-lookup"><span data-stu-id="b167d-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="b167d-117">通道</span><span class="sxs-lookup"><span data-stu-id="b167d-117">channel</span></span>](channel.md) | <span data-ttu-id="b167d-118">创建新的通道通过包括的显示名称和说明。</span><span class="sxs-lookup"><span data-stu-id="b167d-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="b167d-119">获取通道</span><span class="sxs-lookup"><span data-stu-id="b167d-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="b167d-120">通道</span><span class="sxs-lookup"><span data-stu-id="b167d-120">channel</span></span>](channel.md) | <span data-ttu-id="b167d-121">读取属性和该频道的关系。</span><span class="sxs-lookup"><span data-stu-id="b167d-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="b167d-122">更新通道</span><span class="sxs-lookup"><span data-stu-id="b167d-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="b167d-123">通道</span><span class="sxs-lookup"><span data-stu-id="b167d-123">channel</span></span>](channel.md) | <span data-ttu-id="b167d-124">更新该频道的属性。</span><span class="sxs-lookup"><span data-stu-id="b167d-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="b167d-125">删除通道</span><span class="sxs-lookup"><span data-stu-id="b167d-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="b167d-126">无</span><span class="sxs-lookup"><span data-stu-id="b167d-126">None</span></span> | <span data-ttu-id="b167d-127">删除通道。</span><span class="sxs-lookup"><span data-stu-id="b167d-127">Delete a channel.</span></span>|
|[<span data-ttu-id="b167d-128">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="b167d-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="b167d-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b167d-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b167d-130">在通道中收到消息</span><span class="sxs-lookup"><span data-stu-id="b167d-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="b167d-131">创建聊天线程</span><span class="sxs-lookup"><span data-stu-id="b167d-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="b167d-132">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="b167d-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="b167d-133">创建在指定的频道的聊天线程。</span><span class="sxs-lookup"><span data-stu-id="b167d-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="b167d-134">属性</span><span class="sxs-lookup"><span data-stu-id="b167d-134">Properties</span></span>
| <span data-ttu-id="b167d-135">属性</span><span class="sxs-lookup"><span data-stu-id="b167d-135">Property</span></span>     | <span data-ttu-id="b167d-136">类型</span><span class="sxs-lookup"><span data-stu-id="b167d-136">Type</span></span>   |<span data-ttu-id="b167d-137">说明</span><span class="sxs-lookup"><span data-stu-id="b167d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b167d-138">说明</span><span class="sxs-lookup"><span data-stu-id="b167d-138">description</span></span>|<span data-ttu-id="b167d-139">字符串</span><span class="sxs-lookup"><span data-stu-id="b167d-139">String</span></span>|<span data-ttu-id="b167d-140">通道的可选文字说明。</span><span class="sxs-lookup"><span data-stu-id="b167d-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="b167d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b167d-141">displayName</span></span>|<span data-ttu-id="b167d-142">字符串</span><span class="sxs-lookup"><span data-stu-id="b167d-142">String</span></span>|<span data-ttu-id="b167d-143">通道名称将显示于 Microsoft 团队中的用户。</span><span class="sxs-lookup"><span data-stu-id="b167d-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="b167d-144">id</span><span class="sxs-lookup"><span data-stu-id="b167d-144">id</span></span>|<span data-ttu-id="b167d-145">字符串</span><span class="sxs-lookup"><span data-stu-id="b167d-145">String</span></span>|<span data-ttu-id="b167d-146">通道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b167d-146">The channels's unique identifier.</span></span> <span data-ttu-id="b167d-147">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="b167d-147">Read-only.</span></span>|
|<span data-ttu-id="b167d-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="b167d-148">isFavoriteByDefault</span></span>|<span data-ttu-id="b167d-149">布尔</span><span class="sxs-lookup"><span data-stu-id="b167d-149">Boolean</span></span>|<span data-ttu-id="b167d-150">是否通道应自动标记喜欢为团队的所有成员。</span><span class="sxs-lookup"><span data-stu-id="b167d-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="b167d-151">默认值： `false`。</span><span class="sxs-lookup"><span data-stu-id="b167d-151">Default: `false`.</span></span>|
|<span data-ttu-id="b167d-152">email</span><span class="sxs-lookup"><span data-stu-id="b167d-152">email</span></span>|<span data-ttu-id="b167d-153">布尔</span><span class="sxs-lookup"><span data-stu-id="b167d-153">Boolean</span></span>| <span data-ttu-id="b167d-154">向通道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b167d-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="b167d-155">只读。</span><span class="sxs-lookup"><span data-stu-id="b167d-155">Read-only.</span></span>|
|<span data-ttu-id="b167d-156">WebUrl</span><span class="sxs-lookup"><span data-stu-id="b167d-156">webUrl</span></span>|<span data-ttu-id="b167d-157">String</span><span class="sxs-lookup"><span data-stu-id="b167d-157">String</span></span>|<span data-ttu-id="b167d-158">将导航至 Microsoft 团队中的通道超链接。</span><span class="sxs-lookup"><span data-stu-id="b167d-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="b167d-159">这是您获取右键单击 Microsoft 团队中的通道，然后选择 Get 链接到通道时的 URL。</span><span class="sxs-lookup"><span data-stu-id="b167d-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="b167d-160">此 URL 应是视为不透明 blob，并且未分列。</span><span class="sxs-lookup"><span data-stu-id="b167d-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="b167d-161">只读。</span><span class="sxs-lookup"><span data-stu-id="b167d-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b167d-162">Relationships</span><span class="sxs-lookup"><span data-stu-id="b167d-162">Relationships</span></span>
| <span data-ttu-id="b167d-163">关系</span><span class="sxs-lookup"><span data-stu-id="b167d-163">Relationship</span></span> | <span data-ttu-id="b167d-164">类型</span><span class="sxs-lookup"><span data-stu-id="b167d-164">Type</span></span>   |<span data-ttu-id="b167d-165">Description</span><span class="sxs-lookup"><span data-stu-id="b167d-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b167d-166">messages</span><span class="sxs-lookup"><span data-stu-id="b167d-166">messages</span></span>|<span data-ttu-id="b167d-167">[chatMessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="b167d-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="b167d-168">在进入频道的所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="b167d-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="b167d-169">导航属性。</span><span class="sxs-lookup"><span data-stu-id="b167d-169">A navigation property.</span></span> <span data-ttu-id="b167d-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b167d-170">Nullable.</span></span> <span data-ttu-id="b167d-171">目前此 API 仅支持读取，但将最终太支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="b167d-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="b167d-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="b167d-172">chatThreads</span></span>|<span data-ttu-id="b167d-173">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="b167d-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="b167d-174">（这被淘汰以消息属性应用） chatThreads 支持创建新邮件，但未阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="b167d-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="b167d-175">ChatThreads 是导航属性，并且是可以为 Null。</span><span class="sxs-lookup"><span data-stu-id="b167d-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="b167d-176">选项卡</span><span class="sxs-lookup"><span data-stu-id="b167d-176">tabs</span></span>|<span data-ttu-id="b167d-177">[teamsTab](../resources/teamstab.md)集合</span><span class="sxs-lookup"><span data-stu-id="b167d-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="b167d-178">在进入频道的所有选项卡的集合。</span><span class="sxs-lookup"><span data-stu-id="b167d-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="b167d-179">导航属性。</span><span class="sxs-lookup"><span data-stu-id="b167d-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b167d-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b167d-180">JSON representation</span></span>

<span data-ttu-id="b167d-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b167d-181">Here is a JSON representation of the resource</span></span>

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
