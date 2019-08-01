---
title: 频道资源类型
description: '频道是的团队中的消息集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1db6133b4bb4c74e9515a9f14cc6f430ef0e32d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033012"
---
# <a name="channel-resource-type"></a><span data-ttu-id="52ae1-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="52ae1-103">channel resource type</span></span>

<span data-ttu-id="52ae1-104">[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。</span><span class="sxs-lookup"><span data-stu-id="52ae1-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="52ae1-105">每个频道专用于特定主题、部门或项目。</span><span class="sxs-lookup"><span data-stu-id="52ae1-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="52ae1-106">频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。</span><span class="sxs-lookup"><span data-stu-id="52ae1-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="52ae1-107">方法</span><span class="sxs-lookup"><span data-stu-id="52ae1-107">Methods</span></span>

| <span data-ttu-id="52ae1-108">方法</span><span class="sxs-lookup"><span data-stu-id="52ae1-108">Method</span></span>       | <span data-ttu-id="52ae1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="52ae1-109">Return Type</span></span>  |<span data-ttu-id="52ae1-110">说明</span><span class="sxs-lookup"><span data-stu-id="52ae1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52ae1-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="52ae1-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="52ae1-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="52ae1-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="52ae1-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="52ae1-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="52ae1-115">频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-115">channel</span></span>](channel.md) | <span data-ttu-id="52ae1-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="52ae1-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="52ae1-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="52ae1-118">频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-118">channel</span></span>](channel.md) | <span data-ttu-id="52ae1-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52ae1-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="52ae1-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="52ae1-121">频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-121">channel</span></span>](channel.md) | <span data-ttu-id="52ae1-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="52ae1-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="52ae1-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="52ae1-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="52ae1-124">无</span><span class="sxs-lookup"><span data-stu-id="52ae1-124">None</span></span> | <span data-ttu-id="52ae1-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="52ae1-125">Delete a channel.</span></span>|
|[<span data-ttu-id="52ae1-126">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="52ae1-126">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="52ae1-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="52ae1-127">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="52ae1-128">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="52ae1-128">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="52ae1-129">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="52ae1-129">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="52ae1-130">teamsTab</span><span class="sxs-lookup"><span data-stu-id="52ae1-130">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="52ae1-131">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="52ae1-131">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="52ae1-132">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="52ae1-132">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="52ae1-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="52ae1-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="52ae1-134">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="52ae1-134">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="52ae1-135">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="52ae1-135">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="52ae1-136">无</span><span class="sxs-lookup"><span data-stu-id="52ae1-136">None</span></span> | <span data-ttu-id="52ae1-137">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="52ae1-137">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="52ae1-138">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="52ae1-138">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="52ae1-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="52ae1-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="52ae1-140">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="52ae1-140">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="52ae1-141">属性</span><span class="sxs-lookup"><span data-stu-id="52ae1-141">Properties</span></span>
| <span data-ttu-id="52ae1-142">属性</span><span class="sxs-lookup"><span data-stu-id="52ae1-142">Property</span></span>     | <span data-ttu-id="52ae1-143">类型</span><span class="sxs-lookup"><span data-stu-id="52ae1-143">Type</span></span>   |<span data-ttu-id="52ae1-144">说明</span><span class="sxs-lookup"><span data-stu-id="52ae1-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52ae1-145">说明</span><span class="sxs-lookup"><span data-stu-id="52ae1-145">description</span></span>|<span data-ttu-id="52ae1-146">String</span><span class="sxs-lookup"><span data-stu-id="52ae1-146">String</span></span>|<span data-ttu-id="52ae1-147">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="52ae1-147">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="52ae1-148">displayName</span><span class="sxs-lookup"><span data-stu-id="52ae1-148">displayName</span></span>|<span data-ttu-id="52ae1-149">String</span><span class="sxs-lookup"><span data-stu-id="52ae1-149">String</span></span>|<span data-ttu-id="52ae1-150">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="52ae1-150">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="52ae1-151">email</span><span class="sxs-lookup"><span data-stu-id="52ae1-151">email</span></span>|<span data-ttu-id="52ae1-152">String</span><span class="sxs-lookup"><span data-stu-id="52ae1-152">String</span></span>| <span data-ttu-id="52ae1-153">用于向频道发送邮件的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="52ae1-153">The email address for sending messages to the channel.</span></span> <span data-ttu-id="52ae1-154">只读。</span><span class="sxs-lookup"><span data-stu-id="52ae1-154">Read-only.</span></span>|
|<span data-ttu-id="52ae1-155">id</span><span class="sxs-lookup"><span data-stu-id="52ae1-155">id</span></span>|<span data-ttu-id="52ae1-156">String</span><span class="sxs-lookup"><span data-stu-id="52ae1-156">String</span></span>|<span data-ttu-id="52ae1-157">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="52ae1-157">The channels's unique identifier.</span></span> <span data-ttu-id="52ae1-158">只读。</span><span class="sxs-lookup"><span data-stu-id="52ae1-158">Read-only.</span></span>|
|<span data-ttu-id="52ae1-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="52ae1-159">webUrl</span></span>|<span data-ttu-id="52ae1-160">String</span><span class="sxs-lookup"><span data-stu-id="52ae1-160">String</span></span>|<span data-ttu-id="52ae1-161">导航至 Microsoft Teams 中的频道的超链接。</span><span class="sxs-lookup"><span data-stu-id="52ae1-161">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="52ae1-162">在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。</span><span class="sxs-lookup"><span data-stu-id="52ae1-162">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="52ae1-163">应将此 URL 视为不透明的 blob，而不对其进行解析。</span><span class="sxs-lookup"><span data-stu-id="52ae1-163">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="52ae1-164">只读。</span><span class="sxs-lookup"><span data-stu-id="52ae1-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52ae1-165">关系</span><span class="sxs-lookup"><span data-stu-id="52ae1-165">Relationships</span></span>
| <span data-ttu-id="52ae1-166">关系</span><span class="sxs-lookup"><span data-stu-id="52ae1-166">Relationship</span></span> | <span data-ttu-id="52ae1-167">类型</span><span class="sxs-lookup"><span data-stu-id="52ae1-167">Type</span></span>   |<span data-ttu-id="52ae1-168">说明</span><span class="sxs-lookup"><span data-stu-id="52ae1-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52ae1-169">选项卡</span><span class="sxs-lookup"><span data-stu-id="52ae1-169">tabs</span></span>|<span data-ttu-id="52ae1-170">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52ae1-170">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="52ae1-171">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="52ae1-171">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="52ae1-172">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="52ae1-172">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52ae1-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52ae1-173">JSON representation</span></span>

<span data-ttu-id="52ae1-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52ae1-174">Here is a JSON representation of the resource</span></span>

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
