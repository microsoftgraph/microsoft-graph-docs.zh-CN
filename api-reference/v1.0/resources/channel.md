---
title: 频道资源类型
description: '频道是的团队中的消息集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163712"
---
# <a name="channel-resource-type"></a><span data-ttu-id="ea311-103">频道资源类型</span><span class="sxs-lookup"><span data-stu-id="ea311-103">channel resource type</span></span>



<span data-ttu-id="ea311-104">频道是的[团队](../resources/team.md)中的消息集合。</span><span class="sxs-lookup"><span data-stu-id="ea311-104">A channel is a collection of chatMessages within a team.</span></span> <span data-ttu-id="ea311-105">频道表示团队内部的某个主题，因此是讨论的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="ea311-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="ea311-106">示例可以是“星期五团队午餐”和“体系结构讨论”频道。</span><span class="sxs-lookup"><span data-stu-id="ea311-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="ea311-107">方法</span><span class="sxs-lookup"><span data-stu-id="ea311-107">Methods</span></span>

| <span data-ttu-id="ea311-108">方法</span><span class="sxs-lookup"><span data-stu-id="ea311-108">Method</span></span>       | <span data-ttu-id="ea311-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea311-109">Return Type</span></span>  |<span data-ttu-id="ea311-110">说明</span><span class="sxs-lookup"><span data-stu-id="ea311-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea311-111">列出频道</span><span class="sxs-lookup"><span data-stu-id="ea311-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="ea311-112">[频道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="ea311-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="ea311-113">获取此团队中的频道列表。</span><span class="sxs-lookup"><span data-stu-id="ea311-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="ea311-114">创建频道</span><span class="sxs-lookup"><span data-stu-id="ea311-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="ea311-115">频道</span><span class="sxs-lookup"><span data-stu-id="ea311-115">channel</span></span>](channel.md) | <span data-ttu-id="ea311-116">通过包含显示名称和描述来新建频道。</span><span class="sxs-lookup"><span data-stu-id="ea311-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="ea311-117">获取频道</span><span class="sxs-lookup"><span data-stu-id="ea311-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="ea311-118">频道</span><span class="sxs-lookup"><span data-stu-id="ea311-118">channel</span></span>](channel.md) | <span data-ttu-id="ea311-119">读取频道的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea311-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="ea311-120">更新频道</span><span class="sxs-lookup"><span data-stu-id="ea311-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="ea311-121">频道</span><span class="sxs-lookup"><span data-stu-id="ea311-121">channel</span></span>](channel.md) | <span data-ttu-id="ea311-122">更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="ea311-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="ea311-123">删除频道</span><span class="sxs-lookup"><span data-stu-id="ea311-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="ea311-124">无</span><span class="sxs-lookup"><span data-stu-id="ea311-124">None</span></span> | <span data-ttu-id="ea311-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="ea311-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea311-126">属性</span><span class="sxs-lookup"><span data-stu-id="ea311-126">Properties</span></span>
| <span data-ttu-id="ea311-127">属性</span><span class="sxs-lookup"><span data-stu-id="ea311-127">Property</span></span>     | <span data-ttu-id="ea311-128">类型</span><span class="sxs-lookup"><span data-stu-id="ea311-128">Type</span></span>   |<span data-ttu-id="ea311-129">说明</span><span class="sxs-lookup"><span data-stu-id="ea311-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea311-130">说明</span><span class="sxs-lookup"><span data-stu-id="ea311-130">description</span></span>|<span data-ttu-id="ea311-131">String</span><span class="sxs-lookup"><span data-stu-id="ea311-131">String</span></span>|<span data-ttu-id="ea311-132">频道的可选文本描述。</span><span class="sxs-lookup"><span data-stu-id="ea311-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="ea311-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ea311-133">displayName</span></span>|<span data-ttu-id="ea311-134">String</span><span class="sxs-lookup"><span data-stu-id="ea311-134">String</span></span>|<span data-ttu-id="ea311-135">在 Microsoft Teams 中呈现在用户面前的频道名称。</span><span class="sxs-lookup"><span data-stu-id="ea311-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="ea311-136">id</span><span class="sxs-lookup"><span data-stu-id="ea311-136">id</span></span>|<span data-ttu-id="ea311-137">String</span><span class="sxs-lookup"><span data-stu-id="ea311-137">String</span></span>|<span data-ttu-id="ea311-138">频道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ea311-138">The channels's unique identifier.</span></span> <span data-ttu-id="ea311-139">只读。</span><span class="sxs-lookup"><span data-stu-id="ea311-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea311-140">关系</span><span class="sxs-lookup"><span data-stu-id="ea311-140">Relationships</span></span>
| <span data-ttu-id="ea311-141">关系</span><span class="sxs-lookup"><span data-stu-id="ea311-141">Relationship</span></span> | <span data-ttu-id="ea311-142">类型</span><span class="sxs-lookup"><span data-stu-id="ea311-142">Type</span></span>   |<span data-ttu-id="ea311-143">说明</span><span class="sxs-lookup"><span data-stu-id="ea311-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea311-144">选项卡</span><span class="sxs-lookup"><span data-stu-id="ea311-144">tabs</span></span>|<span data-ttu-id="ea311-145">[teamsTab](../resources/teamstab.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea311-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="ea311-146">频道中的所有选项卡集合。</span><span class="sxs-lookup"><span data-stu-id="ea311-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="ea311-147">一种导航属性。</span><span class="sxs-lookup"><span data-stu-id="ea311-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ea311-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea311-148">JSON representation</span></span>

<span data-ttu-id="ea311-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea311-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
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
