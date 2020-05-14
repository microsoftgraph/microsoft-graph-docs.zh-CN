---
title: usedInsight 资源类型
description: 表示特定用户使用的文档的洞察力。 该见解将返回用户查看或修改的最相关的文档。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa5d5adc9b7716f26c1b05edb00122da57d625ab
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44227015"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="7ceff-104">usedInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ceff-104">usedInsight resource type</span></span>

<span data-ttu-id="7ceff-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ceff-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ceff-106">表示特定用户使用的文档的洞察力。</span><span class="sxs-lookup"><span data-stu-id="7ceff-106">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="7ceff-107">该见解将返回用户查看或修改的最相关的文档。</span><span class="sxs-lookup"><span data-stu-id="7ceff-107">The insights returns the most relevant documents that a user viewed or modified.</span></span> <span data-ttu-id="7ceff-108">其中包括以下文档：</span><span class="sxs-lookup"><span data-stu-id="7ceff-108">This includes documents in:</span></span>

- <span data-ttu-id="7ceff-109">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="7ceff-109">OneDrive for Business</span></span>
- <span data-ttu-id="7ceff-110">SharePoint</span><span class="sxs-lookup"><span data-stu-id="7ceff-110">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="7ceff-111">方法</span><span class="sxs-lookup"><span data-stu-id="7ceff-111">Methods</span></span>

| <span data-ttu-id="7ceff-112">方法</span><span class="sxs-lookup"><span data-stu-id="7ceff-112">Method</span></span>       | <span data-ttu-id="7ceff-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ceff-113">Return Type</span></span>  |<span data-ttu-id="7ceff-114">说明</span><span class="sxs-lookup"><span data-stu-id="7ceff-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ceff-115">使用的列表</span><span class="sxs-lookup"><span data-stu-id="7ceff-115">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="7ceff-116">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ceff-116">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="7ceff-117">获取已用文件的列表。</span><span class="sxs-lookup"><span data-stu-id="7ceff-117">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ceff-118">属性</span><span class="sxs-lookup"><span data-stu-id="7ceff-118">Properties</span></span>

| <span data-ttu-id="7ceff-119">属性</span><span class="sxs-lookup"><span data-stu-id="7ceff-119">Property</span></span>              | <span data-ttu-id="7ceff-120">类型</span><span class="sxs-lookup"><span data-stu-id="7ceff-120">Type</span></span>                      | <span data-ttu-id="7ceff-121">说明</span><span class="sxs-lookup"><span data-stu-id="7ceff-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="7ceff-122">id</span><span class="sxs-lookup"><span data-stu-id="7ceff-122">id</span></span>                    | <span data-ttu-id="7ceff-123">String</span><span class="sxs-lookup"><span data-stu-id="7ceff-123">String</span></span>                    | <span data-ttu-id="7ceff-124">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7ceff-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="7ceff-125">只读。</span><span class="sxs-lookup"><span data-stu-id="7ceff-125">Read only.</span></span>        |
| <span data-ttu-id="7ceff-126">lastUsed</span><span class="sxs-lookup"><span data-stu-id="7ceff-126">lastUsed</span></span>              | [<span data-ttu-id="7ceff-127">usageDetails</span><span class="sxs-lookup"><span data-stu-id="7ceff-127">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="7ceff-128">有关用户上次查看或修改项目的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="7ceff-128">Information about when the item was last viewed or modified by the user.</span></span> <span data-ttu-id="7ceff-129">只读。</span><span class="sxs-lookup"><span data-stu-id="7ceff-129">Read only.</span></span>      |
| <span data-ttu-id="7ceff-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="7ceff-130">resourceVisualization</span></span> | [<span data-ttu-id="7ceff-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="7ceff-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="7ceff-132">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="7ceff-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="7ceff-133">只读</span><span class="sxs-lookup"><span data-stu-id="7ceff-133">Read-only</span></span>      |
| <span data-ttu-id="7ceff-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="7ceff-134">resourceReference</span></span>     | [<span data-ttu-id="7ceff-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="7ceff-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="7ceff-136">所用文档的引用属性，例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="7ceff-136">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="7ceff-137">只读</span><span class="sxs-lookup"><span data-stu-id="7ceff-137">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="7ceff-138">关系</span><span class="sxs-lookup"><span data-stu-id="7ceff-138">Relationships</span></span>

| <span data-ttu-id="7ceff-139">属性</span><span class="sxs-lookup"><span data-stu-id="7ceff-139">Property</span></span>      | <span data-ttu-id="7ceff-140">类型</span><span class="sxs-lookup"><span data-stu-id="7ceff-140">Type</span></span>          | <span data-ttu-id="7ceff-141">说明</span><span class="sxs-lookup"><span data-stu-id="7ceff-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="7ceff-142">资源</span><span class="sxs-lookup"><span data-stu-id="7ceff-142">resource</span></span>      | <span data-ttu-id="7ceff-143">[实体](entity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ceff-143">[entity](entity.md) collection</span></span>    | <span data-ttu-id="7ceff-144">用于导航到所使用的项目。</span><span class="sxs-lookup"><span data-stu-id="7ceff-144">Used for navigating to the item that was used.</span></span> <span data-ttu-id="7ceff-145">对于文件附件，类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="7ceff-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="7ceff-146">对于链接的附件，类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="7ceff-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ceff-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ceff-147">JSON representation</span></span>
<span data-ttu-id="7ceff-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ceff-148">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
