---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于计划详细信息对象。最多可定义 6 个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4175692182d115e884642ef8f9956cc4db5dae2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930941"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="2b38f-105">plannerCategoryDescriptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b38f-105">plannerCategoryDescriptions resource type</span></span>

> <span data-ttu-id="2b38f-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2b38f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b38f-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b38f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b38f-p103">**plannerCategoryDescriptions** 资源表示已为计划定义的类别的描述性标签。它属于[计划详细信息](plannerplandetails.md)对象。最多可定义 6 个类别。</span><span class="sxs-lookup"><span data-stu-id="2b38f-p103">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="2b38f-111">属性</span><span class="sxs-lookup"><span data-stu-id="2b38f-111">Properties</span></span>
| <span data-ttu-id="2b38f-112">属性</span><span class="sxs-lookup"><span data-stu-id="2b38f-112">Property</span></span>     | <span data-ttu-id="2b38f-113">类型</span><span class="sxs-lookup"><span data-stu-id="2b38f-113">Type</span></span>   |<span data-ttu-id="2b38f-114">说明</span><span class="sxs-lookup"><span data-stu-id="2b38f-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b38f-115">category1</span><span class="sxs-lookup"><span data-stu-id="2b38f-115">category1</span></span>|<span data-ttu-id="2b38f-116">String</span><span class="sxs-lookup"><span data-stu-id="2b38f-116">String</span></span>|<span data-ttu-id="2b38f-117">与类别 1 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2b38f-117">The label associated with Category 1</span></span>|
|<span data-ttu-id="2b38f-118">category2</span><span class="sxs-lookup"><span data-stu-id="2b38f-118">category2</span></span>|<span data-ttu-id="2b38f-119">String</span><span class="sxs-lookup"><span data-stu-id="2b38f-119">String</span></span>|<span data-ttu-id="2b38f-120">与类别 2 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2b38f-120">The label associated with Category 2</span></span>|
|<span data-ttu-id="2b38f-121">category3</span><span class="sxs-lookup"><span data-stu-id="2b38f-121">category3</span></span>|<span data-ttu-id="2b38f-122">String</span><span class="sxs-lookup"><span data-stu-id="2b38f-122">String</span></span>|<span data-ttu-id="2b38f-123">与类别 3 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2b38f-123">The label associated with Category 3</span></span>|
|<span data-ttu-id="2b38f-124">category4</span><span class="sxs-lookup"><span data-stu-id="2b38f-124">category4</span></span>|<span data-ttu-id="2b38f-125">String</span><span class="sxs-lookup"><span data-stu-id="2b38f-125">String</span></span>|<span data-ttu-id="2b38f-126">与类别 4 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2b38f-126">The label associated with Category 4</span></span>|
|<span data-ttu-id="2b38f-127">category5</span><span class="sxs-lookup"><span data-stu-id="2b38f-127">category5</span></span>|<span data-ttu-id="2b38f-128">String</span><span class="sxs-lookup"><span data-stu-id="2b38f-128">String</span></span>|<span data-ttu-id="2b38f-129">与类别 5 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2b38f-129">The label associated with Category 5</span></span>|
|<span data-ttu-id="2b38f-130">category6</span><span class="sxs-lookup"><span data-stu-id="2b38f-130">category6</span></span>|<span data-ttu-id="2b38f-131">String</span><span class="sxs-lookup"><span data-stu-id="2b38f-131">String</span></span>|<span data-ttu-id="2b38f-132">与类别 6 相关联的标签</span><span class="sxs-lookup"><span data-stu-id="2b38f-132">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b38f-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b38f-133">JSON representation</span></span>
<span data-ttu-id="2b38f-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b38f-134">Here is a JSON representation of the resource.</span></span>

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
