---
title: plannerCategoryDescriptions 资源类型
description: '**PlannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "计划详细信息" 对象。 最多可以定义6个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d0ef4c4f91c4b2f8017a7b7555785c9dd10d082a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447134"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="e1d04-105">plannerCategoryDescriptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1d04-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="e1d04-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e1d04-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1d04-107">**PlannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。</span><span class="sxs-lookup"><span data-stu-id="e1d04-107">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="e1d04-108">它属于 "[计划详细信息](plannerplandetails.md)" 对象。</span><span class="sxs-lookup"><span data-stu-id="e1d04-108">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="e1d04-109">最多可以定义6个类别。</span><span class="sxs-lookup"><span data-stu-id="e1d04-109">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="e1d04-110">属性</span><span class="sxs-lookup"><span data-stu-id="e1d04-110">Properties</span></span>
| <span data-ttu-id="e1d04-111">属性</span><span class="sxs-lookup"><span data-stu-id="e1d04-111">Property</span></span>     | <span data-ttu-id="e1d04-112">类型</span><span class="sxs-lookup"><span data-stu-id="e1d04-112">Type</span></span>   |<span data-ttu-id="e1d04-113">说明</span><span class="sxs-lookup"><span data-stu-id="e1d04-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1d04-114">category1</span><span class="sxs-lookup"><span data-stu-id="e1d04-114">category1</span></span>|<span data-ttu-id="e1d04-115">String</span><span class="sxs-lookup"><span data-stu-id="e1d04-115">String</span></span>|<span data-ttu-id="e1d04-116">与类别1关联的标签</span><span class="sxs-lookup"><span data-stu-id="e1d04-116">The label associated with Category 1</span></span>|
|<span data-ttu-id="e1d04-117">category2</span><span class="sxs-lookup"><span data-stu-id="e1d04-117">category2</span></span>|<span data-ttu-id="e1d04-118">String</span><span class="sxs-lookup"><span data-stu-id="e1d04-118">String</span></span>|<span data-ttu-id="e1d04-119">与类别2关联的标签</span><span class="sxs-lookup"><span data-stu-id="e1d04-119">The label associated with Category 2</span></span>|
|<span data-ttu-id="e1d04-120">category3</span><span class="sxs-lookup"><span data-stu-id="e1d04-120">category3</span></span>|<span data-ttu-id="e1d04-121">String</span><span class="sxs-lookup"><span data-stu-id="e1d04-121">String</span></span>|<span data-ttu-id="e1d04-122">与类别3相关联的标签</span><span class="sxs-lookup"><span data-stu-id="e1d04-122">The label associated with Category 3</span></span>|
|<span data-ttu-id="e1d04-123">category4</span><span class="sxs-lookup"><span data-stu-id="e1d04-123">category4</span></span>|<span data-ttu-id="e1d04-124">String</span><span class="sxs-lookup"><span data-stu-id="e1d04-124">String</span></span>|<span data-ttu-id="e1d04-125">与类别4关联的标签</span><span class="sxs-lookup"><span data-stu-id="e1d04-125">The label associated with Category 4</span></span>|
|<span data-ttu-id="e1d04-126">category5</span><span class="sxs-lookup"><span data-stu-id="e1d04-126">category5</span></span>|<span data-ttu-id="e1d04-127">String</span><span class="sxs-lookup"><span data-stu-id="e1d04-127">String</span></span>|<span data-ttu-id="e1d04-128">与类别5相关联的标签</span><span class="sxs-lookup"><span data-stu-id="e1d04-128">The label associated with Category 5</span></span>|
|<span data-ttu-id="e1d04-129">category6</span><span class="sxs-lookup"><span data-stu-id="e1d04-129">category6</span></span>|<span data-ttu-id="e1d04-130">String</span><span class="sxs-lookup"><span data-stu-id="e1d04-130">String</span></span>|<span data-ttu-id="e1d04-131">与类别6关联的标签</span><span class="sxs-lookup"><span data-stu-id="e1d04-131">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1d04-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1d04-132">JSON representation</span></span>
<span data-ttu-id="e1d04-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1d04-133">Here is a JSON representation of the resource.</span></span>

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
