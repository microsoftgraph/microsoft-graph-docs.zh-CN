---
title: 通道资源类型
description: '频道是 chatMessages 团队中的集合。 '
ms.openlocfilehash: e69c0e7cdef347c59006b1dcce192e7949c2f07e
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209710"
---
# <a name="channel-resource-type"></a><span data-ttu-id="f029a-103">通道资源类型</span><span class="sxs-lookup"><span data-stu-id="f029a-103">channel resource type</span></span>

> <span data-ttu-id="f029a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f029a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f029a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f029a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f029a-106">频道是[chatMessages](chatmessage.md) [团队](../resources/team.md)中的集合。</span><span class="sxs-lookup"><span data-stu-id="f029a-106">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="f029a-107">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="f029a-107">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="f029a-108">示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。</span><span class="sxs-lookup"><span data-stu-id="f029a-108">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="f029a-109">方法</span><span class="sxs-lookup"><span data-stu-id="f029a-109">Methods</span></span>

| <span data-ttu-id="f029a-110">方法</span><span class="sxs-lookup"><span data-stu-id="f029a-110">Method</span></span>       | <span data-ttu-id="f029a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f029a-111">Return Type</span></span>  |<span data-ttu-id="f029a-112">说明</span><span class="sxs-lookup"><span data-stu-id="f029a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f029a-113">列表通道</span><span class="sxs-lookup"><span data-stu-id="f029a-113">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="f029a-114">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="f029a-114">[channel](channel.md) collection</span></span> | <span data-ttu-id="f029a-115">此团队中获取通道的列表。</span><span class="sxs-lookup"><span data-stu-id="f029a-115">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="f029a-116">创建通道</span><span class="sxs-lookup"><span data-stu-id="f029a-116">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="f029a-117">通道</span><span class="sxs-lookup"><span data-stu-id="f029a-117">channel</span></span>](channel.md) | <span data-ttu-id="f029a-118">创建新的通道通过包括的显示名称和说明。</span><span class="sxs-lookup"><span data-stu-id="f029a-118">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="f029a-119">获取通道</span><span class="sxs-lookup"><span data-stu-id="f029a-119">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="f029a-120">通道</span><span class="sxs-lookup"><span data-stu-id="f029a-120">channel</span></span>](channel.md) | <span data-ttu-id="f029a-121">读取属性和该频道的关系。</span><span class="sxs-lookup"><span data-stu-id="f029a-121">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="f029a-122">更新通道</span><span class="sxs-lookup"><span data-stu-id="f029a-122">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="f029a-123">通道</span><span class="sxs-lookup"><span data-stu-id="f029a-123">channel</span></span>](channel.md) | <span data-ttu-id="f029a-124">更新该频道的属性。</span><span class="sxs-lookup"><span data-stu-id="f029a-124">Update properties of the channel.</span></span>|
|[<span data-ttu-id="f029a-125">删除通道</span><span class="sxs-lookup"><span data-stu-id="f029a-125">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="f029a-126">无</span><span class="sxs-lookup"><span data-stu-id="f029a-126">None</span></span> | <span data-ttu-id="f029a-127">删除通道。</span><span class="sxs-lookup"><span data-stu-id="f029a-127">Delete a channel.</span></span>|
|[<span data-ttu-id="f029a-128">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="f029a-128">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="f029a-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f029a-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f029a-130">在通道中收到消息</span><span class="sxs-lookup"><span data-stu-id="f029a-130">Get messages in a channel</span></span> |
|[<span data-ttu-id="f029a-131">创建聊天线程</span><span class="sxs-lookup"><span data-stu-id="f029a-131">Create chat thread</span></span>](../api/channel-post-chatthreads.md) | <span data-ttu-id="f029a-132">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="f029a-132">[chatThread](chatthread.md) collection</span></span>| <span data-ttu-id="f029a-133">创建在指定的频道的聊天线程。</span><span class="sxs-lookup"><span data-stu-id="f029a-133">Create a chat thread in the specified channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="f029a-134">属性</span><span class="sxs-lookup"><span data-stu-id="f029a-134">Properties</span></span>
| <span data-ttu-id="f029a-135">属性</span><span class="sxs-lookup"><span data-stu-id="f029a-135">Property</span></span>     | <span data-ttu-id="f029a-136">类型</span><span class="sxs-lookup"><span data-stu-id="f029a-136">Type</span></span>   |<span data-ttu-id="f029a-137">说明</span><span class="sxs-lookup"><span data-stu-id="f029a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f029a-138">说明</span><span class="sxs-lookup"><span data-stu-id="f029a-138">description</span></span>|<span data-ttu-id="f029a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="f029a-139">String</span></span>|<span data-ttu-id="f029a-140">通道的可选文字说明。</span><span class="sxs-lookup"><span data-stu-id="f029a-140">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="f029a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="f029a-141">displayName</span></span>|<span data-ttu-id="f029a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f029a-142">String</span></span>|<span data-ttu-id="f029a-143">通道名称将显示于 Microsoft 团队中的用户。</span><span class="sxs-lookup"><span data-stu-id="f029a-143">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="f029a-144">id</span><span class="sxs-lookup"><span data-stu-id="f029a-144">id</span></span>|<span data-ttu-id="f029a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f029a-145">String</span></span>|<span data-ttu-id="f029a-146">通道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f029a-146">The channels's unique identifier.</span></span> <span data-ttu-id="f029a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="f029a-147">Read-only.</span></span>|
|<span data-ttu-id="f029a-148">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="f029a-148">isFavoriteByDefault</span></span>|<span data-ttu-id="f029a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="f029a-149">Boolean</span></span>|<span data-ttu-id="f029a-150">是否通道应自动标记喜欢为团队的所有成员。</span><span class="sxs-lookup"><span data-stu-id="f029a-150">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="f029a-151">默认值： `false`。</span><span class="sxs-lookup"><span data-stu-id="f029a-151">Default: `false`.</span></span>|
|<span data-ttu-id="f029a-152">email</span><span class="sxs-lookup"><span data-stu-id="f029a-152">email</span></span>|<span data-ttu-id="f029a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f029a-153">Boolean</span></span>| <span data-ttu-id="f029a-154">向通道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f029a-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="f029a-155">只读。</span><span class="sxs-lookup"><span data-stu-id="f029a-155">Read-only.</span></span>|
|<span data-ttu-id="f029a-156">WebUrl</span><span class="sxs-lookup"><span data-stu-id="f029a-156">webUrl</span></span>|<span data-ttu-id="f029a-157">String</span><span class="sxs-lookup"><span data-stu-id="f029a-157">String</span></span>|<span data-ttu-id="f029a-158">将导航至 Microsoft 团队中的通道超链接。</span><span class="sxs-lookup"><span data-stu-id="f029a-158">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="f029a-159">这是您获取右键单击 Microsoft 团队中的通道，然后选择 Get 链接到通道时的 URL。</span><span class="sxs-lookup"><span data-stu-id="f029a-159">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="f029a-160">此 URL 应是视为不透明 blob，并且未分列。</span><span class="sxs-lookup"><span data-stu-id="f029a-160">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="f029a-161">只读。</span><span class="sxs-lookup"><span data-stu-id="f029a-161">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f029a-162">Relationships</span><span class="sxs-lookup"><span data-stu-id="f029a-162">Relationships</span></span>
| <span data-ttu-id="f029a-163">关系</span><span class="sxs-lookup"><span data-stu-id="f029a-163">Relationship</span></span> | <span data-ttu-id="f029a-164">类型</span><span class="sxs-lookup"><span data-stu-id="f029a-164">Type</span></span>   |<span data-ttu-id="f029a-165">说明</span><span class="sxs-lookup"><span data-stu-id="f029a-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f029a-166">messages</span><span class="sxs-lookup"><span data-stu-id="f029a-166">messages</span></span>|<span data-ttu-id="f029a-167">[chatMessage](chatmessage.md)集合</span><span class="sxs-lookup"><span data-stu-id="f029a-167">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="f029a-168">在进入频道的所有邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="f029a-168">A collection of all the messages in the channel.</span></span> <span data-ttu-id="f029a-169">导航属性。</span><span class="sxs-lookup"><span data-stu-id="f029a-169">A navigation property.</span></span> <span data-ttu-id="f029a-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f029a-170">Nullable.</span></span> <span data-ttu-id="f029a-171">目前此 API 仅支持读取，但将最终太支持写入消息。</span><span class="sxs-lookup"><span data-stu-id="f029a-171">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="f029a-172">chatThreads</span><span class="sxs-lookup"><span data-stu-id="f029a-172">chatThreads</span></span>|<span data-ttu-id="f029a-173">[chatThread](chatthread.md)集合</span><span class="sxs-lookup"><span data-stu-id="f029a-173">[chatThread](chatthread.md) collection</span></span>|<span data-ttu-id="f029a-174">（这被淘汰以消息属性应用） chatThreads 支持创建新邮件，但未阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="f029a-174">(This is being phased out in favor of the messages property) chatThreads supports creating new messages but not reading messages.</span></span> <span data-ttu-id="f029a-175">ChatThreads 是导航属性，并且是可以为 Null。</span><span class="sxs-lookup"><span data-stu-id="f029a-175">ChatThreads is a navigation property, and is Nullable.</span></span>|
|<span data-ttu-id="f029a-176">选项卡</span><span class="sxs-lookup"><span data-stu-id="f029a-176">tabs</span></span>|<span data-ttu-id="f029a-177">[teamsTab](../resources/teamstab.md)集合</span><span class="sxs-lookup"><span data-stu-id="f029a-177">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="f029a-178">在进入频道的所有选项卡的集合。</span><span class="sxs-lookup"><span data-stu-id="f029a-178">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="f029a-179">导航属性。</span><span class="sxs-lookup"><span data-stu-id="f029a-179">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f029a-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f029a-180">JSON representation</span></span>

<span data-ttu-id="f029a-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f029a-181">Here is a JSON representation of the resource</span></span>

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
