---
title: 通道资源类型
description: '频道是 chatMessages 团队中的集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6529c555e418589cb757a1bc52bda520bd792745
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952326"
---
# <a name="channel-resource-type"></a><span data-ttu-id="5fb11-103">通道资源类型</span><span class="sxs-lookup"><span data-stu-id="5fb11-103">channel resource type</span></span>

> <span data-ttu-id="5fb11-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5fb11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fb11-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5fb11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5fb11-106">频道是[chatMessages](chatmessage.md) [团队](../resources/team.md)中的集合。</span><span class="sxs-lookup"><span data-stu-id="5fb11-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="5fb11-107">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="5fb11-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="5fb11-108">示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。</span><span class="sxs-lookup"><span data-stu-id="5fb11-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="5fb11-109">方法</span><span class="sxs-lookup"><span data-stu-id="5fb11-109">Methods</span></span>

| <span data-ttu-id="5fb11-110">方法</span><span class="sxs-lookup"><span data-stu-id="5fb11-110">Method</span></span>       | <span data-ttu-id="5fb11-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fb11-111">Return Type</span></span>  |<span data-ttu-id="5fb11-112">说明</span><span class="sxs-lookup"><span data-stu-id="5fb11-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fb11-113">列表通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="5fb11-114">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fb11-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="5fb11-115">此团队中获取通道的列表。</span><span class="sxs-lookup"><span data-stu-id="5fb11-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="5fb11-116">创建通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="5fb11-117">通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-117">channel</span></span>](channel.md) | <span data-ttu-id="5fb11-118">创建新的通道通过包括的显示名称和说明。</span><span class="sxs-lookup"><span data-stu-id="5fb11-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="5fb11-119">获取通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="5fb11-120">通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-120">channel</span></span>](channel.md) | <span data-ttu-id="5fb11-121">读取属性和该频道的关系。</span><span class="sxs-lookup"><span data-stu-id="5fb11-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="5fb11-122">更新通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="5fb11-123">通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-123">channel</span></span>](channel.md) | <span data-ttu-id="5fb11-124">更新该频道的属性。</span><span class="sxs-lookup"><span data-stu-id="5fb11-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="5fb11-125">删除通道</span><span class="sxs-lookup"><span data-stu-id="5fb11-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="5fb11-126">无</span><span class="sxs-lookup"><span data-stu-id="5fb11-126">None</span></span> | <span data-ttu-id="5fb11-127">删除通道。</span><span class="sxs-lookup"><span data-stu-id="5fb11-127">Delete a channel.</span></span>|
|[<span data-ttu-id="5fb11-128">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="5fb11-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="5fb11-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="5fb11-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="5fb11-130">在通道中收到消息</span><span class="sxs-lookup"><span data-stu-id="5fb11-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="5fb11-131">创建聊天线程</span><span class="sxs-lookup"><span data-stu-id="5fb11-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="5fb11-132">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fb11-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="5fb11-133">创建在指定的频道的聊天线程。</span><span class="sxs-lookup"><span data-stu-id="5fb11-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="5fb11-134">属性</span><span class="sxs-lookup"><span data-stu-id="5fb11-134">Properties</span></span>
| <span data-ttu-id="5fb11-135">属性</span><span class="sxs-lookup"><span data-stu-id="5fb11-135">Property</span></span>     | <span data-ttu-id="5fb11-136">类型</span><span class="sxs-lookup"><span data-stu-id="5fb11-136">Type</span></span>   |<span data-ttu-id="5fb11-137">说明</span><span class="sxs-lookup"><span data-stu-id="5fb11-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fb11-138">说明</span><span class="sxs-lookup"><span data-stu-id="5fb11-138">description</span></span>|<span data-ttu-id="5fb11-139">字符串</span><span class="sxs-lookup"><span data-stu-id="5fb11-139">String</span></span>|<span data-ttu-id="5fb11-140">通道的可选文字说明。</span><span class="sxs-lookup"><span data-stu-id="5fb11-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="5fb11-141">displayName</span><span class="sxs-lookup"><span data-stu-id="5fb11-141">displayName</span></span>|<span data-ttu-id="5fb11-142">字符串</span><span class="sxs-lookup"><span data-stu-id="5fb11-142">String</span></span>|<span data-ttu-id="5fb11-143">通道名称将显示于 Microsoft 团队中的用户。</span><span class="sxs-lookup"><span data-stu-id="5fb11-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="5fb11-144">id</span><span class="sxs-lookup"><span data-stu-id="5fb11-144">id</span></span>|<span data-ttu-id="5fb11-145">字符串</span><span class="sxs-lookup"><span data-stu-id="5fb11-145">String</span></span>|<span data-ttu-id="5fb11-146">通道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5fb11-146">The channels's unique identifier.</span></span> <span data-ttu-id="5fb11-147">只读。</span><span class="sxs-lookup"><span data-stu-id="5fb11-147">Read-only.</span></span>|
|<span data-ttu-id="5fb11-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="5fb11-148">isFavoriteByDefault</span></span>|<span data-ttu-id="5fb11-149">布尔</span><span class="sxs-lookup"><span data-stu-id="5fb11-149">Boolean</span></span>|<span data-ttu-id="5fb11-150">是否通道应自动标记喜欢为团队的所有成员。</span><span class="sxs-lookup"><span data-stu-id="5fb11-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="5fb11-151">默认值： `false`。</span><span class="sxs-lookup"><span data-stu-id="5fb11-151">Default: `false`.</span></span>|
|<span data-ttu-id="5fb11-152">email</span><span class="sxs-lookup"><span data-stu-id="5fb11-152">email</span></span>|<span data-ttu-id="5fb11-153">布尔</span><span class="sxs-lookup"><span data-stu-id="5fb11-153">Boolean</span></span>| <span data-ttu-id="5fb11-154">向通道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5fb11-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="5fb11-155">只读。</span><span class="sxs-lookup"><span data-stu-id="5fb11-155">Read-only.</span></span>|
|<span data-ttu-id="5fb11-156">WebUrl</span><span class="sxs-lookup"><span data-stu-id="5fb11-156">webUrl</span></span>|<span data-ttu-id="5fb11-157">String</span><span class="sxs-lookup"><span data-stu-id="5fb11-157">String</span></span>|<span data-ttu-id="5fb11-158">将导航至 Microsoft 团队中的通道超链接。</span><span class="sxs-lookup"><span data-stu-id="5fb11-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="5fb11-159">这是您获取右键单击 Microsoft 团队中的通道，然后选择 Get 链接到通道时的 URL。</span><span class="sxs-lookup"><span data-stu-id="5fb11-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="5fb11-160">此 URL 应是视为不透明 blob，并且未分列。</span><span class="sxs-lookup"><span data-stu-id="5fb11-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="5fb11-161">只读。</span><span class="sxs-lookup"><span data-stu-id="5fb11-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5fb11-162">Relationships</span><span class="sxs-lookup"><span data-stu-id="5fb11-162">Relationships</span></span>
| <span data-ttu-id="5fb11-163">关系</span><span class="sxs-lookup"><span data-stu-id="5fb11-163">Relationship</span></span> | <span data-ttu-id="5fb11-164">类型</span><span class="sxs-lookup"><span data-stu-id="5fb11-164">Type</span></span>   |<span data-ttu-id="5fb11-165">说明</span><span class="sxs-lookup"><span data-stu-id="5fb11-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fb11-166">messages</span><span class="sxs-lookup"><span data-stu-id="5fb11-166">messages</span></span>|<span data-ttu-id="5fb11-167">[chatMessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fb11-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="5fb11-168">在进入频道的所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="5fb11-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="5fb11-169">导航属性。</span><span class="sxs-lookup"><span data-stu-id="5fb11-169">A navigation property.</span></span> <span data-ttu-id="5fb11-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5fb11-170">Nullable.</span></span> <span data-ttu-id="5fb11-171">目前此 API 仅支持读取，但将最终太支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="5fb11-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="5fb11-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="5fb11-172">chatThreads</span></span>|<span data-ttu-id="5fb11-173">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fb11-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="5fb11-174">（这被淘汰以消息属性应用） chatThreads 支持创建新邮件，但未阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="5fb11-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="5fb11-175">ChatThreads 是导航属性，并且是可以为 Null。</span><span class="sxs-lookup"><span data-stu-id="5fb11-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="5fb11-176">选项卡</span><span class="sxs-lookup"><span data-stu-id="5fb11-176">tabs</span></span>|<span data-ttu-id="5fb11-177">[teamsTab](../resources/teamstab.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fb11-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="5fb11-178">在进入频道的所有选项卡的集合。</span><span class="sxs-lookup"><span data-stu-id="5fb11-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="5fb11-179">导航属性。</span><span class="sxs-lookup"><span data-stu-id="5fb11-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5fb11-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fb11-180">JSON representation</span></span>

<span data-ttu-id="5fb11-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fb11-181">Here is a JSON representation of the resource</span></span>

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
