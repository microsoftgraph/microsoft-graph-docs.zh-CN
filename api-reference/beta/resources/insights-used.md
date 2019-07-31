---
title: usedInsight 资源类型
description: 表示特定用户使用的文档的洞察力。 该见解将返回用户查看或访问的最相关的文档。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2b6e7a7c4df94e9ffbcb34ef200457b4a903eb24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005686"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="4deec-104">usedInsight 资源类型</span><span class="sxs-lookup"><span data-stu-id="4deec-104">usedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4deec-105">表示特定用户使用的文档的洞察力。</span><span class="sxs-lookup"><span data-stu-id="4deec-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="4deec-106">该见解将返回用户查看或访问的最相关的文档。</span><span class="sxs-lookup"><span data-stu-id="4deec-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="4deec-107">其中包括以下文档:</span><span class="sxs-lookup"><span data-stu-id="4deec-107">This includes documents in:</span></span>

- <span data-ttu-id="4deec-108">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="4deec-108">OneDrive for Business</span></span>
- <span data-ttu-id="4deec-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="4deec-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="4deec-110">方法</span><span class="sxs-lookup"><span data-stu-id="4deec-110">Methods</span></span>

| <span data-ttu-id="4deec-111">方法</span><span class="sxs-lookup"><span data-stu-id="4deec-111">Method</span></span>       | <span data-ttu-id="4deec-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="4deec-112">Return Type</span></span>  |<span data-ttu-id="4deec-113">说明</span><span class="sxs-lookup"><span data-stu-id="4deec-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4deec-114">使用的列表</span><span class="sxs-lookup"><span data-stu-id="4deec-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="4deec-115">[usedInsight](insights-used.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4deec-115">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="4deec-116">获取已用文件的列表。</span><span class="sxs-lookup"><span data-stu-id="4deec-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="4deec-117">属性</span><span class="sxs-lookup"><span data-stu-id="4deec-117">Properties</span></span>

| <span data-ttu-id="4deec-118">属性</span><span class="sxs-lookup"><span data-stu-id="4deec-118">Property</span></span>              | <span data-ttu-id="4deec-119">类型</span><span class="sxs-lookup"><span data-stu-id="4deec-119">Type</span></span>                      | <span data-ttu-id="4deec-120">说明</span><span class="sxs-lookup"><span data-stu-id="4deec-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="4deec-121">id</span><span class="sxs-lookup"><span data-stu-id="4deec-121">id</span></span>                    | <span data-ttu-id="4deec-122">String</span><span class="sxs-lookup"><span data-stu-id="4deec-122">String</span></span>                    | <span data-ttu-id="4deec-123">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4deec-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="4deec-124">只读。</span><span class="sxs-lookup"><span data-stu-id="4deec-124">Read only.</span></span>        |
| <span data-ttu-id="4deec-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="4deec-125">lastUsed</span></span>              | [<span data-ttu-id="4deec-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="4deec-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="4deec-127">有关用户上次查看和修改项目的时间的信息。</span><span class="sxs-lookup"><span data-stu-id="4deec-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="4deec-128">只读。</span><span class="sxs-lookup"><span data-stu-id="4deec-128">Read only.</span></span>     |
| <span data-ttu-id="4deec-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4deec-129">resourceVisualization</span></span> | [<span data-ttu-id="4deec-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4deec-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="4deec-131">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="4deec-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="4deec-132">只读</span><span class="sxs-lookup"><span data-stu-id="4deec-132">Read-only</span></span>      |
| <span data-ttu-id="4deec-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="4deec-133">resourceReference</span></span>     | [<span data-ttu-id="4deec-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="4deec-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="4deec-135">所用文档的引用属性, 例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="4deec-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="4deec-136">只读</span><span class="sxs-lookup"><span data-stu-id="4deec-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="4deec-137">关系</span><span class="sxs-lookup"><span data-stu-id="4deec-137">Relationships</span></span>

| <span data-ttu-id="4deec-138">属性</span><span class="sxs-lookup"><span data-stu-id="4deec-138">Property</span></span>      | <span data-ttu-id="4deec-139">类型</span><span class="sxs-lookup"><span data-stu-id="4deec-139">Type</span></span>          | <span data-ttu-id="4deec-140">说明</span><span class="sxs-lookup"><span data-stu-id="4deec-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="4deec-141">资源</span><span class="sxs-lookup"><span data-stu-id="4deec-141">resource</span></span>      | <span data-ttu-id="4deec-142">[实体](entity.md)集合</span><span class="sxs-lookup"><span data-stu-id="4deec-142">[entity](entity.md) collection</span></span>    | <span data-ttu-id="4deec-143">用于导航到所使用的项目。</span><span class="sxs-lookup"><span data-stu-id="4deec-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="4deec-144">对于文件附件, 类型为*fileAttachment*。</span><span class="sxs-lookup"><span data-stu-id="4deec-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="4deec-145">对于链接的附件, 类型为*driveItem*。</span><span class="sxs-lookup"><span data-stu-id="4deec-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4deec-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4deec-146">JSON representation</span></span>
<span data-ttu-id="4deec-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4deec-147">Here is a JSON representation of the resource</span></span>

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
