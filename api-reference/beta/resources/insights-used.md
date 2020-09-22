---
title: usedInsight 资源类型
description: 表示特定用户使用的文档的洞察力。 该见解将返回用户查看或修改的最相关的文档。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06dec4840edae33d51ddb64fb48d93aaa8ccdfda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986064"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="d304e-104">usedInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="d304e-104">usedInsight resource type</span></span>

<span data-ttu-id="d304e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d304e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d304e-106">表示特定用户使用的文档的洞察力。</span><span class="sxs-lookup"><span data-stu-id="d304e-106">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="d304e-107">该见解将返回用户查看或修改的最相关的文档。</span><span class="sxs-lookup"><span data-stu-id="d304e-107">The insights returns the most relevant documents that a user viewed or modified.</span></span> <span data-ttu-id="d304e-108">其中包括以下文档：</span><span class="sxs-lookup"><span data-stu-id="d304e-108">This includes documents in:</span></span>

- <span data-ttu-id="d304e-109">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="d304e-109">OneDrive for Business</span></span>
- <span data-ttu-id="d304e-110">SharePoint</span><span class="sxs-lookup"><span data-stu-id="d304e-110">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="d304e-111">方法</span><span class="sxs-lookup"><span data-stu-id="d304e-111">Methods</span></span>

| <span data-ttu-id="d304e-112">方法</span><span class="sxs-lookup"><span data-stu-id="d304e-112">Method</span></span>       | <span data-ttu-id="d304e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="d304e-113">Return Type</span></span>  |<span data-ttu-id="d304e-114">说明</span><span class="sxs-lookup"><span data-stu-id="d304e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d304e-115">使用的列表</span><span class="sxs-lookup"><span data-stu-id="d304e-115">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="d304e-116">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d304e-116">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="d304e-117">获取已用文件的列表。</span><span class="sxs-lookup"><span data-stu-id="d304e-117">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="d304e-118">属性</span><span class="sxs-lookup"><span data-stu-id="d304e-118">Properties</span></span>

| <span data-ttu-id="d304e-119">属性</span><span class="sxs-lookup"><span data-stu-id="d304e-119">Property</span></span>              | <span data-ttu-id="d304e-120">类型</span><span class="sxs-lookup"><span data-stu-id="d304e-120">Type</span></span>                      | <span data-ttu-id="d304e-121">说明</span><span class="sxs-lookup"><span data-stu-id="d304e-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="d304e-122">id</span><span class="sxs-lookup"><span data-stu-id="d304e-122">id</span></span>                    | <span data-ttu-id="d304e-123">String</span><span class="sxs-lookup"><span data-stu-id="d304e-123">String</span></span>                    | <span data-ttu-id="d304e-124">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d304e-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="d304e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="d304e-125">Read only.</span></span>        |
| <span data-ttu-id="d304e-126">lastUsed</span><span class="sxs-lookup"><span data-stu-id="d304e-126">lastUsed</span></span>              | [<span data-ttu-id="d304e-127">usageDetails</span><span class="sxs-lookup"><span data-stu-id="d304e-127">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="d304e-128">有关用户上次查看或修改项目的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="d304e-128">Information about when the item was last viewed or modified by the user.</span></span> <span data-ttu-id="d304e-129">只读。</span><span class="sxs-lookup"><span data-stu-id="d304e-129">Read only.</span></span>      |
| <span data-ttu-id="d304e-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d304e-130">resourceVisualization</span></span> | [<span data-ttu-id="d304e-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d304e-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="d304e-132">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="d304e-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="d304e-133">只读</span><span class="sxs-lookup"><span data-stu-id="d304e-133">Read-only</span></span>      |
| <span data-ttu-id="d304e-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d304e-134">resourceReference</span></span>     | [<span data-ttu-id="d304e-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d304e-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="d304e-136">所用文档的引用属性，例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="d304e-136">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="d304e-137">只读</span><span class="sxs-lookup"><span data-stu-id="d304e-137">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="d304e-138">关系</span><span class="sxs-lookup"><span data-stu-id="d304e-138">Relationships</span></span>

| <span data-ttu-id="d304e-139">属性</span><span class="sxs-lookup"><span data-stu-id="d304e-139">Property</span></span>      | <span data-ttu-id="d304e-140">类型</span><span class="sxs-lookup"><span data-stu-id="d304e-140">Type</span></span>          | <span data-ttu-id="d304e-141">说明</span><span class="sxs-lookup"><span data-stu-id="d304e-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="d304e-142">资源</span><span class="sxs-lookup"><span data-stu-id="d304e-142">resource</span></span>      | <span data-ttu-id="d304e-143">[实体](entity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d304e-143">[entity](entity.md) collection</span></span>    | <span data-ttu-id="d304e-144">用于导航到所使用的项目。</span><span class="sxs-lookup"><span data-stu-id="d304e-144">Used for navigating to the item that was used.</span></span> <span data-ttu-id="d304e-145">对于文件附件，类型为 *fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="d304e-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="d304e-146">对于链接的附件，类型为 *driveItem*。</span><span class="sxs-lookup"><span data-stu-id="d304e-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d304e-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d304e-147">JSON representation</span></span>
<span data-ttu-id="d304e-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d304e-148">Here is a JSON representation of the resource</span></span>

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


