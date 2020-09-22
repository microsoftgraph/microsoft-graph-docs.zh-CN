---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5209670c004da2b58d41444c0bfa31f12891b8d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074844"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="2a8cd-103">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a8cd-103">teamsTab resource type</span></span>

<span data-ttu-id="2a8cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a8cd-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="2a8cd-105">TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="2a8cd-106">方法</span><span class="sxs-lookup"><span data-stu-id="2a8cd-106">Methods</span></span>

| <span data-ttu-id="2a8cd-107">方法</span><span class="sxs-lookup"><span data-stu-id="2a8cd-107">Method</span></span>       | <span data-ttu-id="2a8cd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a8cd-108">Return Type</span></span>  |<span data-ttu-id="2a8cd-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a8cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a8cd-110">列出选项卡</span><span class="sxs-lookup"><span data-stu-id="2a8cd-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="2a8cd-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2a8cd-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2a8cd-112">列出固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="2a8cd-113">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="2a8cd-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="2a8cd-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2a8cd-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2a8cd-115">读取固定到频道的选项卡。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="2a8cd-116">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="2a8cd-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="2a8cd-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2a8cd-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2a8cd-118">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="2a8cd-119">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="2a8cd-119">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="2a8cd-120">无</span><span class="sxs-lookup"><span data-stu-id="2a8cd-120">None</span></span> | <span data-ttu-id="2a8cd-121">将选项卡添加（固定）到频道。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="2a8cd-122">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="2a8cd-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="2a8cd-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2a8cd-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="2a8cd-124">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="2a8cd-125">属性</span><span class="sxs-lookup"><span data-stu-id="2a8cd-125">Properties</span></span>

|<span data-ttu-id="2a8cd-126">属性</span><span class="sxs-lookup"><span data-stu-id="2a8cd-126">Property</span></span>|<span data-ttu-id="2a8cd-127">类型</span><span class="sxs-lookup"><span data-stu-id="2a8cd-127">Type</span></span>|<span data-ttu-id="2a8cd-128">说明</span><span class="sxs-lookup"><span data-stu-id="2a8cd-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="2a8cd-129">id</span><span class="sxs-lookup"><span data-stu-id="2a8cd-129">id</span></span>              |   <span data-ttu-id="2a8cd-130">string</span><span class="sxs-lookup"><span data-stu-id="2a8cd-130">string</span></span>                  |  <span data-ttu-id="2a8cd-131">唯一标识 "通道" 选项卡的特定实例的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="2a8cd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2a8cd-132">displayName</span></span>            |   <span data-ttu-id="2a8cd-133">string</span><span class="sxs-lookup"><span data-stu-id="2a8cd-133">string</span></span>                  |  <span data-ttu-id="2a8cd-134">选项卡的名称。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="2a8cd-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="2a8cd-135">webUrl</span></span>          |   <span data-ttu-id="2a8cd-136">string</span><span class="sxs-lookup"><span data-stu-id="2a8cd-136">string</span></span>                  |  <span data-ttu-id="2a8cd-137">选项卡实例的深层链接 URL。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="2a8cd-138">只读。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-138">Read only.</span></span>     |
|  <span data-ttu-id="2a8cd-139">configuration</span><span class="sxs-lookup"><span data-stu-id="2a8cd-139">configuration</span></span>        |   [<span data-ttu-id="2a8cd-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a8cd-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="2a8cd-141">应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="2a8cd-142">关系</span><span class="sxs-lookup"><span data-stu-id="2a8cd-142">Relationships</span></span>

| <span data-ttu-id="2a8cd-143">关系</span><span class="sxs-lookup"><span data-stu-id="2a8cd-143">Relationship</span></span> | <span data-ttu-id="2a8cd-144">类型</span><span class="sxs-lookup"><span data-stu-id="2a8cd-144">Type</span></span>   | <span data-ttu-id="2a8cd-145">说明</span><span class="sxs-lookup"><span data-stu-id="2a8cd-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2a8cd-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2a8cd-146">teamsApp</span></span>|[<span data-ttu-id="2a8cd-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2a8cd-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2a8cd-148">链接到该选项卡的应用程序。创建选项卡后，不能更改此选项。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a8cd-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a8cd-149">JSON representation</span></span>

<span data-ttu-id="2a8cd-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a8cd-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="2a8cd-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2a8cd-151">See also</span></span>

[<span data-ttu-id="2a8cd-152">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="2a8cd-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

