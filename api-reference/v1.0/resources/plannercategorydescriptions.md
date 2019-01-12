---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于计划详细信息对象。最多可定义 6 个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1cf1ee1c6e8ccc4e90f78985b352062fce37df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984344"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="45bb0-105">plannerCategoryDescriptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="45bb0-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="45bb0-p102">**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。</span><span class="sxs-lookup"><span data-stu-id="45bb0-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="45bb0-109">属性</span><span class="sxs-lookup"><span data-stu-id="45bb0-109">Properties</span></span>
| <span data-ttu-id="45bb0-110">属性</span><span class="sxs-lookup"><span data-stu-id="45bb0-110">Property</span></span>     | <span data-ttu-id="45bb0-111">类型</span><span class="sxs-lookup"><span data-stu-id="45bb0-111">Type</span></span>   |<span data-ttu-id="45bb0-112">说明</span><span class="sxs-lookup"><span data-stu-id="45bb0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45bb0-113">category1</span><span class="sxs-lookup"><span data-stu-id="45bb0-113">category1</span></span>|<span data-ttu-id="45bb0-114">String</span><span class="sxs-lookup"><span data-stu-id="45bb0-114">String</span></span>|<span data-ttu-id="45bb0-115">与类别 1 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="45bb0-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="45bb0-116">category2</span><span class="sxs-lookup"><span data-stu-id="45bb0-116">category2</span></span>|<span data-ttu-id="45bb0-117">String</span><span class="sxs-lookup"><span data-stu-id="45bb0-117">String</span></span>|<span data-ttu-id="45bb0-118">与类别 2 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="45bb0-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="45bb0-119">category3</span><span class="sxs-lookup"><span data-stu-id="45bb0-119">category3</span></span>|<span data-ttu-id="45bb0-120">String</span><span class="sxs-lookup"><span data-stu-id="45bb0-120">String</span></span>|<span data-ttu-id="45bb0-121">与类别 3 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="45bb0-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="45bb0-122">category4</span><span class="sxs-lookup"><span data-stu-id="45bb0-122">category4</span></span>|<span data-ttu-id="45bb0-123">String</span><span class="sxs-lookup"><span data-stu-id="45bb0-123">String</span></span>|<span data-ttu-id="45bb0-124">与类别 4 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="45bb0-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="45bb0-125">category5</span><span class="sxs-lookup"><span data-stu-id="45bb0-125">category5</span></span>|<span data-ttu-id="45bb0-126">String</span><span class="sxs-lookup"><span data-stu-id="45bb0-126">String</span></span>|<span data-ttu-id="45bb0-127">与类别 5 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="45bb0-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="45bb0-128">category6</span><span class="sxs-lookup"><span data-stu-id="45bb0-128">category6</span></span>|<span data-ttu-id="45bb0-129">String</span><span class="sxs-lookup"><span data-stu-id="45bb0-129">String</span></span>|<span data-ttu-id="45bb0-130">与类别 6 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="45bb0-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45bb0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45bb0-131">JSON representation</span></span>
<span data-ttu-id="45bb0-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45bb0-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
