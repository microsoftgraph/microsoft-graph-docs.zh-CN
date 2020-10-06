---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f9860f6d1385374258eeed11dd8db4db21ba895c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364397"
---
# <a name="channel-resource-type"></a><span data-ttu-id="c8250-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="c8250-103">channel resource type</span></span>

<span data-ttu-id="c8250-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8250-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c8250-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="c8250-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="c8250-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="c8250-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="c8250-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="c8250-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="c8250-108">方法</span><span class="sxs-lookup"><span data-stu-id="c8250-108">Methods</span></span>

| <span data-ttu-id="c8250-109">方法</span><span class="sxs-lookup"><span data-stu-id="c8250-109">Method</span></span>       | <span data-ttu-id="c8250-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8250-110">Return Type</span></span>  |<span data-ttu-id="c8250-111">说明</span><span class="sxs-lookup"><span data-stu-id="c8250-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8250-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="c8250-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="c8250-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="c8250-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="c8250-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="c8250-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="c8250-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="c8250-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="c8250-116">频道</span><span class="sxs-lookup"><span data-stu-id="c8250-116">channel</span></span>](channel.md) | <span data-ttu-id="c8250-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="c8250-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="c8250-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="c8250-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="c8250-119">频道</span><span class="sxs-lookup"><span data-stu-id="c8250-119">channel</span></span>](channel.md) | <span data-ttu-id="c8250-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8250-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="c8250-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="c8250-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="c8250-122">频道</span><span class="sxs-lookup"><span data-stu-id="c8250-122">channel</span></span>](channel.md) | <span data-ttu-id="c8250-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="c8250-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="c8250-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="c8250-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="c8250-125">无</span><span class="sxs-lookup"><span data-stu-id="c8250-125">None</span></span> | <span data-ttu-id="c8250-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="c8250-126">Delete a channel.</span></span>|
|[<span data-ttu-id="c8250-127">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="c8250-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="c8250-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c8250-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="c8250-129">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="c8250-129">Lists tabs pinned to a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8250-130">属性</span><span class="sxs-lookup"><span data-stu-id="c8250-130">Properties</span></span>

| <span data-ttu-id="c8250-131">属性</span><span class="sxs-lookup"><span data-stu-id="c8250-131">Property</span></span>   | <span data-ttu-id="c8250-132">类型</span><span class="sxs-lookup"><span data-stu-id="c8250-132">Type</span></span> |<span data-ttu-id="c8250-133">说明</span><span class="sxs-lookup"><span data-stu-id="c8250-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8250-134">说明</span><span class="sxs-lookup"><span data-stu-id="c8250-134">description</span></span>|<span data-ttu-id="c8250-135">String</span><span class="sxs-lookup"><span data-stu-id="c8250-135">String</span></span>|<span data-ttu-id="c8250-136">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="c8250-136">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="c8250-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c8250-137">displayName</span></span>|<span data-ttu-id="c8250-138">String</span><span class="sxs-lookup"><span data-stu-id="c8250-138">String</span></span>|<span data-ttu-id="c8250-139">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="c8250-139">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="c8250-140">id</span><span class="sxs-lookup"><span data-stu-id="c8250-140">id</span></span>|<span data-ttu-id="c8250-141">String</span><span class="sxs-lookup"><span data-stu-id="c8250-141">String</span></span>|<span data-ttu-id="c8250-142">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c8250-142">The channel's unique identifier.</span></span> <span data-ttu-id="c8250-143">只读。</span><span class="sxs-lookup"><span data-stu-id="c8250-143">Read-only.</span></span>|
|<span data-ttu-id="c8250-144">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="c8250-144">isFavoriteByDefault</span></span>|<span data-ttu-id="c8250-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8250-145">Boolean</span></span>|<span data-ttu-id="c8250-146">指示是否应对团队的所有成员将频道自动标记到“收藏夹”。</span><span class="sxs-lookup"><span data-stu-id="c8250-146">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="c8250-147">仅可使用“[创建团队](../api/team-post.md)”以编程方式设置。</span><span class="sxs-lookup"><span data-stu-id="c8250-147">Can only be set programmatically with [Create team](../api/team-post.md).</span></span> <span data-ttu-id="c8250-148">默认值：`false`。</span><span class="sxs-lookup"><span data-stu-id="c8250-148">Default: `false`.</span></span>|
|<span data-ttu-id="c8250-149">email</span><span class="sxs-lookup"><span data-stu-id="c8250-149">email</span></span>|<span data-ttu-id="c8250-150">String</span><span class="sxs-lookup"><span data-stu-id="c8250-150">String</span></span>| <span data-ttu-id="c8250-151">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c8250-151">The email address for sending messages to the channel.</span></span> <span data-ttu-id="c8250-152">只读。</span><span class="sxs-lookup"><span data-stu-id="c8250-152">Read-only.</span></span>|
|<span data-ttu-id="c8250-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="c8250-153">webUrl</span></span>|<span data-ttu-id="c8250-154">String</span><span class="sxs-lookup"><span data-stu-id="c8250-154">String</span></span>|<span data-ttu-id="c8250-155">将转到 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="c8250-155">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="c8250-156">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="c8250-156">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="c8250-157">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="c8250-157">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="c8250-158">只读。</span><span class="sxs-lookup"><span data-stu-id="c8250-158">Read-only.</span></span>|
|<span data-ttu-id="c8250-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8250-159">createdDateTime</span></span>|<span data-ttu-id="c8250-160">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8250-160">dateTimeOffset</span></span>|<span data-ttu-id="c8250-161">只读。</span><span class="sxs-lookup"><span data-stu-id="c8250-161">Read only.</span></span> <span data-ttu-id="c8250-162">创建频道的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c8250-162">Timestamp at which the channel was created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8250-163">关系</span><span class="sxs-lookup"><span data-stu-id="c8250-163">Relationships</span></span>

| <span data-ttu-id="c8250-164">关系</span><span class="sxs-lookup"><span data-stu-id="c8250-164">Relationship</span></span> | <span data-ttu-id="c8250-165">类型</span><span class="sxs-lookup"><span data-stu-id="c8250-165">Type</span></span> |<span data-ttu-id="c8250-166">说明</span><span class="sxs-lookup"><span data-stu-id="c8250-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8250-167">messages</span><span class="sxs-lookup"><span data-stu-id="c8250-167">messages</span></span>|<span data-ttu-id="c8250-168">[chatMessage](chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8250-168">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="c8250-169">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="c8250-169">A collection of all the messages in the channel.</span></span> <span data-ttu-id="c8250-170">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="c8250-170">A navigation property.</span></span> <span data-ttu-id="c8250-171">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c8250-171">Nullable.</span></span>|
|<span data-ttu-id="c8250-172">选项卡</span><span class="sxs-lookup"><span data-stu-id="c8250-172">tabs</span></span>|<span data-ttu-id="c8250-173">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8250-173">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="c8250-174">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="c8250-174">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="c8250-175">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="c8250-175">A navigation property.</span></span>|
|[<span data-ttu-id="c8250-176">filesFolder</span><span class="sxs-lookup"><span data-stu-id="c8250-176">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="c8250-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="c8250-177">driveItem</span></span>](driveitem.md)|<span data-ttu-id="c8250-178">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="c8250-178">Metadata for the location where the channel's files are stored.</span></span>|
|<span data-ttu-id="c8250-179">operations</span><span class="sxs-lookup"><span data-stu-id="c8250-179">operations</span></span>|<span data-ttu-id="c8250-180">[teamsAsyncOperation](teamsasyncoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8250-180">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="c8250-181">在此团队中运行过或正在运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="c8250-181">The async operations that ran or are running on this team.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c8250-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8250-182">JSON representation</span></span>

<span data-ttu-id="c8250-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8250-183">The following is a JSON representation of the resource.</span></span>

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
