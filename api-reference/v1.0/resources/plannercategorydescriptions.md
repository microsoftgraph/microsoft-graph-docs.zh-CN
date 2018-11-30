---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于计划详细信息对象。最多可定义 6 个类别。 '
ms.openlocfilehash: e71cbd1f41d23747691b3738b5a46ff302a72168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008637"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="7346b-105">plannerCategoryDescriptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="7346b-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="7346b-p102">**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。</span><span class="sxs-lookup"><span data-stu-id="7346b-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="7346b-109">属性</span><span class="sxs-lookup"><span data-stu-id="7346b-109">Properties</span></span>
| <span data-ttu-id="7346b-110">属性</span><span class="sxs-lookup"><span data-stu-id="7346b-110">Property</span></span>     | <span data-ttu-id="7346b-111">类型</span><span class="sxs-lookup"><span data-stu-id="7346b-111">Type</span></span>   |<span data-ttu-id="7346b-112">说明</span><span class="sxs-lookup"><span data-stu-id="7346b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7346b-113">category1</span><span class="sxs-lookup"><span data-stu-id="7346b-113">category1</span></span>|<span data-ttu-id="7346b-114">String</span><span class="sxs-lookup"><span data-stu-id="7346b-114">String</span></span>|<span data-ttu-id="7346b-115">与类别 1 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="7346b-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="7346b-116">category2</span><span class="sxs-lookup"><span data-stu-id="7346b-116">category2</span></span>|<span data-ttu-id="7346b-117">String</span><span class="sxs-lookup"><span data-stu-id="7346b-117">String</span></span>|<span data-ttu-id="7346b-118">与类别 2 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="7346b-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="7346b-119">category3</span><span class="sxs-lookup"><span data-stu-id="7346b-119">category3</span></span>|<span data-ttu-id="7346b-120">String</span><span class="sxs-lookup"><span data-stu-id="7346b-120">String</span></span>|<span data-ttu-id="7346b-121">与类别 3 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="7346b-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="7346b-122">category4</span><span class="sxs-lookup"><span data-stu-id="7346b-122">category4</span></span>|<span data-ttu-id="7346b-123">String</span><span class="sxs-lookup"><span data-stu-id="7346b-123">String</span></span>|<span data-ttu-id="7346b-124">与类别 4 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="7346b-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="7346b-125">category5</span><span class="sxs-lookup"><span data-stu-id="7346b-125">category5</span></span>|<span data-ttu-id="7346b-126">String</span><span class="sxs-lookup"><span data-stu-id="7346b-126">String</span></span>|<span data-ttu-id="7346b-127">与类别 5 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="7346b-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="7346b-128">category6</span><span class="sxs-lookup"><span data-stu-id="7346b-128">category6</span></span>|<span data-ttu-id="7346b-129">String</span><span class="sxs-lookup"><span data-stu-id="7346b-129">String</span></span>|<span data-ttu-id="7346b-130">与类别 6 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="7346b-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7346b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7346b-131">JSON representation</span></span>
<span data-ttu-id="7346b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7346b-132">Here is a JSON representation of the resource.</span></span>

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