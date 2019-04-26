---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "计划详细信息" 对象。 最多可以定义6个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a410f748c43d50872936d4bcc106ffeb224d76cf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344555"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="8d7ca-105">plannerCategoryDescriptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d7ca-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d7ca-106">**plannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。</span><span class="sxs-lookup"><span data-stu-id="8d7ca-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="8d7ca-107">它属于 "[计划详细信息](plannerplandetails.md)" 对象。</span><span class="sxs-lookup"><span data-stu-id="8d7ca-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="8d7ca-108">最多可以定义6个类别。</span><span class="sxs-lookup"><span data-stu-id="8d7ca-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="8d7ca-109">属性</span><span class="sxs-lookup"><span data-stu-id="8d7ca-109">Properties</span></span>
| <span data-ttu-id="8d7ca-110">属性</span><span class="sxs-lookup"><span data-stu-id="8d7ca-110">Property</span></span>     | <span data-ttu-id="8d7ca-111">类型</span><span class="sxs-lookup"><span data-stu-id="8d7ca-111">Type</span></span>   |<span data-ttu-id="8d7ca-112">说明</span><span class="sxs-lookup"><span data-stu-id="8d7ca-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d7ca-113">category1</span><span class="sxs-lookup"><span data-stu-id="8d7ca-113">category1</span></span>|<span data-ttu-id="8d7ca-114">String</span><span class="sxs-lookup"><span data-stu-id="8d7ca-114">String</span></span>|<span data-ttu-id="8d7ca-115">与类别1关联的标签</span><span class="sxs-lookup"><span data-stu-id="8d7ca-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="8d7ca-116">category2</span><span class="sxs-lookup"><span data-stu-id="8d7ca-116">category2</span></span>|<span data-ttu-id="8d7ca-117">String</span><span class="sxs-lookup"><span data-stu-id="8d7ca-117">String</span></span>|<span data-ttu-id="8d7ca-118">与类别2关联的标签</span><span class="sxs-lookup"><span data-stu-id="8d7ca-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="8d7ca-119">category3</span><span class="sxs-lookup"><span data-stu-id="8d7ca-119">category3</span></span>|<span data-ttu-id="8d7ca-120">String</span><span class="sxs-lookup"><span data-stu-id="8d7ca-120">String</span></span>|<span data-ttu-id="8d7ca-121">与类别3相关联的标签</span><span class="sxs-lookup"><span data-stu-id="8d7ca-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="8d7ca-122">category4</span><span class="sxs-lookup"><span data-stu-id="8d7ca-122">category4</span></span>|<span data-ttu-id="8d7ca-123">String</span><span class="sxs-lookup"><span data-stu-id="8d7ca-123">String</span></span>|<span data-ttu-id="8d7ca-124">与类别4关联的标签</span><span class="sxs-lookup"><span data-stu-id="8d7ca-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="8d7ca-125">category5</span><span class="sxs-lookup"><span data-stu-id="8d7ca-125">category5</span></span>|<span data-ttu-id="8d7ca-126">String</span><span class="sxs-lookup"><span data-stu-id="8d7ca-126">String</span></span>|<span data-ttu-id="8d7ca-127">与类别5相关联的标签</span><span class="sxs-lookup"><span data-stu-id="8d7ca-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="8d7ca-128">category6</span><span class="sxs-lookup"><span data-stu-id="8d7ca-128">category6</span></span>|<span data-ttu-id="8d7ca-129">String</span><span class="sxs-lookup"><span data-stu-id="8d7ca-129">String</span></span>|<span data-ttu-id="8d7ca-130">与类别6关联的标签</span><span class="sxs-lookup"><span data-stu-id="8d7ca-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d7ca-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d7ca-131">JSON representation</span></span>
<span data-ttu-id="8d7ca-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d7ca-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
