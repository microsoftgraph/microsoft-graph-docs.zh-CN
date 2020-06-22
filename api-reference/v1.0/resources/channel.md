---
title: 频道资源类型
description: '频道是的团队中的消息集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b6a0baaa684808c4d05bdcebf4be6d761d41d1b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793582"
---
# <a name="channel-resource-type"></a><span data-ttu-id="5f388-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="5f388-103">channel resource type</span></span>

<span data-ttu-id="5f388-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f388-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f388-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="5f388-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="5f388-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="5f388-106">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="5f388-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="5f388-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="5f388-108">方法</span><span class="sxs-lookup"><span data-stu-id="5f388-108">Methods</span></span>

| <span data-ttu-id="5f388-109">方法</span><span class="sxs-lookup"><span data-stu-id="5f388-109">Method</span></span>       | <span data-ttu-id="5f388-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f388-110">Return Type</span></span>  |<span data-ttu-id="5f388-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f388-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f388-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="5f388-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="5f388-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="5f388-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="5f388-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="5f388-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="5f388-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="5f388-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="5f388-116">频道</span><span class="sxs-lookup"><span data-stu-id="5f388-116">channel</span></span>](channel.md) | <span data-ttu-id="5f388-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="5f388-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="5f388-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="5f388-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="5f388-119">频道</span><span class="sxs-lookup"><span data-stu-id="5f388-119">channel</span></span>](channel.md) | <span data-ttu-id="5f388-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f388-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="5f388-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="5f388-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="5f388-122">频道</span><span class="sxs-lookup"><span data-stu-id="5f388-122">channel</span></span>](channel.md) | <span data-ttu-id="5f388-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="5f388-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="5f388-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="5f388-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="5f388-125">无</span><span class="sxs-lookup"><span data-stu-id="5f388-125">None</span></span> | <span data-ttu-id="5f388-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="5f388-126">Delete a channel.</span></span>|
|[<span data-ttu-id="5f388-127">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="5f388-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="5f388-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5f388-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5f388-129">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="5f388-129">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="5f388-130">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="5f388-130">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="5f388-131">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5f388-131">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5f388-132">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="5f388-132">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="5f388-133">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="5f388-133">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="5f388-134">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5f388-134">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5f388-135">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="5f388-135">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="5f388-136">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="5f388-136">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="5f388-137">无</span><span class="sxs-lookup"><span data-stu-id="5f388-137">None</span></span> | <span data-ttu-id="5f388-138">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="5f388-138">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="5f388-139">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="5f388-139">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="5f388-140">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5f388-140">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="5f388-141">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="5f388-141">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f388-142">属性</span><span class="sxs-lookup"><span data-stu-id="5f388-142">Properties</span></span>

| <span data-ttu-id="5f388-143">属性</span><span class="sxs-lookup"><span data-stu-id="5f388-143">Property</span></span>   | <span data-ttu-id="5f388-144">类型</span><span class="sxs-lookup"><span data-stu-id="5f388-144">Type</span></span> | <span data-ttu-id="5f388-145">说明</span><span class="sxs-lookup"><span data-stu-id="5f388-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f388-146">说明</span><span class="sxs-lookup"><span data-stu-id="5f388-146">description</span></span>|<span data-ttu-id="5f388-147">String</span><span class="sxs-lookup"><span data-stu-id="5f388-147">String</span></span>|<span data-ttu-id="5f388-148">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="5f388-148">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="5f388-149">displayName</span><span class="sxs-lookup"><span data-stu-id="5f388-149">displayName</span></span>|<span data-ttu-id="5f388-150">String</span><span class="sxs-lookup"><span data-stu-id="5f388-150">String</span></span>|<span data-ttu-id="5f388-151">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="5f388-151">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="5f388-152">email</span><span class="sxs-lookup"><span data-stu-id="5f388-152">email</span></span>|<span data-ttu-id="5f388-153">String</span><span class="sxs-lookup"><span data-stu-id="5f388-153">String</span></span>| <span data-ttu-id="5f388-154">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5f388-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="5f388-155">只读。</span><span class="sxs-lookup"><span data-stu-id="5f388-155">Read-only.</span></span>|
|<span data-ttu-id="5f388-156">id</span><span class="sxs-lookup"><span data-stu-id="5f388-156">id</span></span>|<span data-ttu-id="5f388-157">String</span><span class="sxs-lookup"><span data-stu-id="5f388-157">String</span></span>|<span data-ttu-id="5f388-158">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5f388-158">The channels's unique identifier.</span></span> <span data-ttu-id="5f388-159">只读。</span><span class="sxs-lookup"><span data-stu-id="5f388-159">Read-only.</span></span>|
|<span data-ttu-id="5f388-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="5f388-160">webUrl</span></span>|<span data-ttu-id="5f388-161">String</span><span class="sxs-lookup"><span data-stu-id="5f388-161">String</span></span>|<span data-ttu-id="5f388-162">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="5f388-162">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="5f388-163">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="5f388-163">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="5f388-164">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="5f388-164">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="5f388-165">只读。</span><span class="sxs-lookup"><span data-stu-id="5f388-165">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f388-166">关系</span><span class="sxs-lookup"><span data-stu-id="5f388-166">Relationships</span></span>

| <span data-ttu-id="5f388-167">关系</span><span class="sxs-lookup"><span data-stu-id="5f388-167">Relationship</span></span> | <span data-ttu-id="5f388-168">类型</span><span class="sxs-lookup"><span data-stu-id="5f388-168">Type</span></span> | <span data-ttu-id="5f388-169">说明</span><span class="sxs-lookup"><span data-stu-id="5f388-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f388-170">messages</span><span class="sxs-lookup"><span data-stu-id="5f388-170">messages</span></span>|<span data-ttu-id="5f388-171">[chatMessage](./chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f388-171">[chatMessage](./chatmessage.md) collection</span></span>|<span data-ttu-id="5f388-172">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="5f388-172">A collection of all the messages in the channel.</span></span> <span data-ttu-id="5f388-173">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="5f388-173">A navigation property.</span></span> <span data-ttu-id="5f388-174">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5f388-174">Nullable.</span></span>|
|<span data-ttu-id="5f388-175">选项卡</span><span class="sxs-lookup"><span data-stu-id="5f388-175">tabs</span></span>|<span data-ttu-id="5f388-176">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f388-176">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="5f388-177">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="5f388-177">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="5f388-178">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="5f388-178">A navigation property.</span></span>|
|[<span data-ttu-id="5f388-179">filesFolder</span><span class="sxs-lookup"><span data-stu-id="5f388-179">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="5f388-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="5f388-180">driveItem</span></span>](driveitem.md)|<span data-ttu-id="5f388-181">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="5f388-181">Metadata for the location where the channel's files are stored.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5f388-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f388-182">JSON representation</span></span>

<span data-ttu-id="5f388-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f388-183">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
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
