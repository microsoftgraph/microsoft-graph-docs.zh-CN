---
title: 通道资源类型
description: '频道是团队中的邮件的集合。 '
author: nkramer
ms.openlocfilehash: f9ab71213180732a0c8c626d5b32b9074bd135d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337084"
---
# <a name="channel-resource-type"></a><span data-ttu-id="040aa-103">通道资源类型</span><span class="sxs-lookup"><span data-stu-id="040aa-103">channel resource type</span></span>



<span data-ttu-id="040aa-104">频道是[团队](../resources/team.md)中的邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="040aa-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="040aa-105">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="040aa-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="040aa-106">示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。</span><span class="sxs-lookup"><span data-stu-id="040aa-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="040aa-107">方法</span><span class="sxs-lookup"><span data-stu-id="040aa-107">Methods</span></span>

| <span data-ttu-id="040aa-108">方法</span><span class="sxs-lookup"><span data-stu-id="040aa-108">Method</span></span>       | <span data-ttu-id="040aa-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="040aa-109">Return Type</span></span>  |<span data-ttu-id="040aa-110">说明</span><span class="sxs-lookup"><span data-stu-id="040aa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="040aa-111">列表通道</span><span class="sxs-lookup"><span data-stu-id="040aa-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="040aa-112">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="040aa-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="040aa-113">此团队中获取通道的列表。</span><span class="sxs-lookup"><span data-stu-id="040aa-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="040aa-114">创建通道</span><span class="sxs-lookup"><span data-stu-id="040aa-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="040aa-115">通道</span><span class="sxs-lookup"><span data-stu-id="040aa-115">channel</span></span>](channel.md) | <span data-ttu-id="040aa-116">创建新的通道通过包括的显示名称和说明。</span><span class="sxs-lookup"><span data-stu-id="040aa-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="040aa-117">获取通道</span><span class="sxs-lookup"><span data-stu-id="040aa-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="040aa-118">通道</span><span class="sxs-lookup"><span data-stu-id="040aa-118">channel</span></span>](channel.md) | <span data-ttu-id="040aa-119">读取属性和该频道的关系。</span><span class="sxs-lookup"><span data-stu-id="040aa-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="040aa-120">更新通道</span><span class="sxs-lookup"><span data-stu-id="040aa-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="040aa-121">通道</span><span class="sxs-lookup"><span data-stu-id="040aa-121">channel</span></span>](channel.md) | <span data-ttu-id="040aa-122">更新该频道的属性。</span><span class="sxs-lookup"><span data-stu-id="040aa-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="040aa-123">删除通道</span><span class="sxs-lookup"><span data-stu-id="040aa-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="040aa-124">无</span><span class="sxs-lookup"><span data-stu-id="040aa-124">None</span></span> | <span data-ttu-id="040aa-125">删除通道。</span><span class="sxs-lookup"><span data-stu-id="040aa-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="040aa-126">属性</span><span class="sxs-lookup"><span data-stu-id="040aa-126">Properties</span></span>
| <span data-ttu-id="040aa-127">属性</span><span class="sxs-lookup"><span data-stu-id="040aa-127">Property</span></span>     | <span data-ttu-id="040aa-128">类型</span><span class="sxs-lookup"><span data-stu-id="040aa-128">Type</span></span>   |<span data-ttu-id="040aa-129">说明</span><span class="sxs-lookup"><span data-stu-id="040aa-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="040aa-130">说明</span><span class="sxs-lookup"><span data-stu-id="040aa-130">description</span></span>|<span data-ttu-id="040aa-131">字符串</span><span class="sxs-lookup"><span data-stu-id="040aa-131">String</span></span>|<span data-ttu-id="040aa-132">通道的可选文字说明。</span><span class="sxs-lookup"><span data-stu-id="040aa-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="040aa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="040aa-133">displayName</span></span>|<span data-ttu-id="040aa-134">字符串</span><span class="sxs-lookup"><span data-stu-id="040aa-134">String</span></span>|<span data-ttu-id="040aa-135">通道名称将显示于 Microsoft 团队中的用户。</span><span class="sxs-lookup"><span data-stu-id="040aa-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="040aa-136">id</span><span class="sxs-lookup"><span data-stu-id="040aa-136">id</span></span>|<span data-ttu-id="040aa-137">字符串</span><span class="sxs-lookup"><span data-stu-id="040aa-137">String</span></span>|<span data-ttu-id="040aa-138">通道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="040aa-138">The channels's unique identifier.</span></span> <span data-ttu-id="040aa-139">只读。</span><span class="sxs-lookup"><span data-stu-id="040aa-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="040aa-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="040aa-140">Relationships</span></span>
| <span data-ttu-id="040aa-141">关系</span><span class="sxs-lookup"><span data-stu-id="040aa-141">Relationship</span></span> | <span data-ttu-id="040aa-142">类型</span><span class="sxs-lookup"><span data-stu-id="040aa-142">Type</span></span>   |<span data-ttu-id="040aa-143">说明</span><span class="sxs-lookup"><span data-stu-id="040aa-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="040aa-144">选项卡</span><span class="sxs-lookup"><span data-stu-id="040aa-144">tabs</span></span>|<span data-ttu-id="040aa-145">[teamsTab](../resources/teamstab.md)集合</span><span class="sxs-lookup"><span data-stu-id="040aa-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="040aa-146">在进入频道的所有选项卡的集合。</span><span class="sxs-lookup"><span data-stu-id="040aa-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="040aa-147">导航属性。</span><span class="sxs-lookup"><span data-stu-id="040aa-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="040aa-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="040aa-148">JSON representation</span></span>

<span data-ttu-id="040aa-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="040aa-149">Here is a JSON representation of the resource</span></span>

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
