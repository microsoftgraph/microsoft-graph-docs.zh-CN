---
title: 频道资源类型
description: '频道是的团队中的消息集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f995fa1cb725ae5c0764f349180e7f757a9f423e
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272652"
---
# <a name="channel-resource-type"></a><span data-ttu-id="9feaf-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="9feaf-103">channel resource type</span></span>

<span data-ttu-id="9feaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9feaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9feaf-105">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="9feaf-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="9feaf-106">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="9feaf-106">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="9feaf-107">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="9feaf-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="9feaf-108">方法</span><span class="sxs-lookup"><span data-stu-id="9feaf-108">Methods</span></span>

| <span data-ttu-id="9feaf-109">方法</span><span class="sxs-lookup"><span data-stu-id="9feaf-109">Method</span></span>       | <span data-ttu-id="9feaf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9feaf-110">Return Type</span></span>  |<span data-ttu-id="9feaf-111">说明</span><span class="sxs-lookup"><span data-stu-id="9feaf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9feaf-112">列出频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="9feaf-113">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="9feaf-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="9feaf-114">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="9feaf-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="9feaf-115">创建频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="9feaf-116">频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-116">channel</span></span>](channel.md) | <span data-ttu-id="9feaf-117">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="9feaf-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="9feaf-118">获取频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="9feaf-119">频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-119">channel</span></span>](channel.md) | <span data-ttu-id="9feaf-120">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9feaf-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="9feaf-121">更新频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="9feaf-122">频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-122">channel</span></span>](channel.md) | <span data-ttu-id="9feaf-123">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="9feaf-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="9feaf-124">删除频道</span><span class="sxs-lookup"><span data-stu-id="9feaf-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="9feaf-125">无</span><span class="sxs-lookup"><span data-stu-id="9feaf-125">None</span></span> | <span data-ttu-id="9feaf-126">删除通道。</span><span class="sxs-lookup"><span data-stu-id="9feaf-126">Delete a channel.</span></span>|
|[<span data-ttu-id="9feaf-127">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="9feaf-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="9feaf-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9feaf-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9feaf-129">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="9feaf-129">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="9feaf-130">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="9feaf-130">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="9feaf-131">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9feaf-131">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9feaf-132">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="9feaf-132">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="9feaf-133">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="9feaf-133">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="9feaf-134">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9feaf-134">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9feaf-135">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="9feaf-135">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="9feaf-136">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="9feaf-136">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="9feaf-137">无</span><span class="sxs-lookup"><span data-stu-id="9feaf-137">None</span></span> | <span data-ttu-id="9feaf-138">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="9feaf-138">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="9feaf-139">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="9feaf-139">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="9feaf-140">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9feaf-140">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9feaf-141">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="9feaf-141">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="9feaf-142">属性</span><span class="sxs-lookup"><span data-stu-id="9feaf-142">Properties</span></span>

| <span data-ttu-id="9feaf-143">属性</span><span class="sxs-lookup"><span data-stu-id="9feaf-143">Property</span></span>   | <span data-ttu-id="9feaf-144">类型</span><span class="sxs-lookup"><span data-stu-id="9feaf-144">Type</span></span> | <span data-ttu-id="9feaf-145">说明</span><span class="sxs-lookup"><span data-stu-id="9feaf-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9feaf-146">说明</span><span class="sxs-lookup"><span data-stu-id="9feaf-146">description</span></span>|<span data-ttu-id="9feaf-147">String</span><span class="sxs-lookup"><span data-stu-id="9feaf-147">String</span></span>|<span data-ttu-id="9feaf-148">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="9feaf-148">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="9feaf-149">displayName</span><span class="sxs-lookup"><span data-stu-id="9feaf-149">displayName</span></span>|<span data-ttu-id="9feaf-150">String</span><span class="sxs-lookup"><span data-stu-id="9feaf-150">String</span></span>|<span data-ttu-id="9feaf-151">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="9feaf-151">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="9feaf-152">email</span><span class="sxs-lookup"><span data-stu-id="9feaf-152">email</span></span>|<span data-ttu-id="9feaf-153">String</span><span class="sxs-lookup"><span data-stu-id="9feaf-153">String</span></span>| <span data-ttu-id="9feaf-154">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9feaf-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="9feaf-155">只读。</span><span class="sxs-lookup"><span data-stu-id="9feaf-155">Read-only.</span></span>|
|<span data-ttu-id="9feaf-156">id</span><span class="sxs-lookup"><span data-stu-id="9feaf-156">id</span></span>|<span data-ttu-id="9feaf-157">String</span><span class="sxs-lookup"><span data-stu-id="9feaf-157">String</span></span>|<span data-ttu-id="9feaf-158">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9feaf-158">The channels's unique identifier.</span></span> <span data-ttu-id="9feaf-159">只读。</span><span class="sxs-lookup"><span data-stu-id="9feaf-159">Read-only.</span></span>|
|<span data-ttu-id="9feaf-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="9feaf-160">webUrl</span></span>|<span data-ttu-id="9feaf-161">String</span><span class="sxs-lookup"><span data-stu-id="9feaf-161">String</span></span>|<span data-ttu-id="9feaf-162">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="9feaf-162">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="9feaf-163">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="9feaf-163">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="9feaf-164">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="9feaf-164">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="9feaf-165">只读。</span><span class="sxs-lookup"><span data-stu-id="9feaf-165">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9feaf-166">关系</span><span class="sxs-lookup"><span data-stu-id="9feaf-166">Relationships</span></span>

| <span data-ttu-id="9feaf-167">关系</span><span class="sxs-lookup"><span data-stu-id="9feaf-167">Relationship</span></span> | <span data-ttu-id="9feaf-168">类型</span><span class="sxs-lookup"><span data-stu-id="9feaf-168">Type</span></span> | <span data-ttu-id="9feaf-169">说明</span><span class="sxs-lookup"><span data-stu-id="9feaf-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9feaf-170">messages</span><span class="sxs-lookup"><span data-stu-id="9feaf-170">messages</span></span>|<span data-ttu-id="9feaf-171">[chatMessage](./chatmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9feaf-171">[chatMessage](./chatmessage.md) collection</span></span>|<span data-ttu-id="9feaf-172">频道中的所有消息集合。</span><span class="sxs-lookup"><span data-stu-id="9feaf-172">A collection of all the messages in the channel.</span></span> <span data-ttu-id="9feaf-173">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="9feaf-173">A navigation property.</span></span> <span data-ttu-id="9feaf-174">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9feaf-174">Nullable.</span></span>|
|<span data-ttu-id="9feaf-175">选项卡</span><span class="sxs-lookup"><span data-stu-id="9feaf-175">tabs</span></span>|<span data-ttu-id="9feaf-176">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9feaf-176">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="9feaf-177">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="9feaf-177">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="9feaf-178">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="9feaf-178">A navigation property.</span></span>|
|<span data-ttu-id="9feaf-179">filesFolder</span><span class="sxs-lookup"><span data-stu-id="9feaf-179">filesFolder</span></span>|[<span data-ttu-id="9feaf-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="9feaf-180">driveItem</span></span>](driveitem.md)|<span data-ttu-id="9feaf-181">用于存储频道文件的位置的元数据。</span><span class="sxs-lookup"><span data-stu-id="9feaf-181">Metadata for the location where the channel's files are stored.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9feaf-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9feaf-182">JSON representation</span></span>

<span data-ttu-id="9feaf-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9feaf-183">Here is a JSON representation of the resource</span></span>

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
