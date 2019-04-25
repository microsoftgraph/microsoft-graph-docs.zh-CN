---
title: plannerCategoryDescriptions 资源类型
description: '**plannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。 它属于 "计划详细信息" 对象。 最多可以定义6个类别。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 33031dc3c688e1fefb34109cb0a4a303dbe1c183
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579028"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="09ffc-105">plannerCategoryDescriptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="09ffc-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ffc-106">**plannerCategoryDescriptions**资源表示已为计划定义的类别的描述性标签。</span><span class="sxs-lookup"><span data-stu-id="09ffc-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="09ffc-107">它属于 "[计划详细信息](plannerplandetails.md)" 对象。</span><span class="sxs-lookup"><span data-stu-id="09ffc-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="09ffc-108">最多可以定义6个类别。</span><span class="sxs-lookup"><span data-stu-id="09ffc-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="09ffc-109">属性</span><span class="sxs-lookup"><span data-stu-id="09ffc-109">Properties</span></span>
| <span data-ttu-id="09ffc-110">属性</span><span class="sxs-lookup"><span data-stu-id="09ffc-110">Property</span></span>     | <span data-ttu-id="09ffc-111">类型</span><span class="sxs-lookup"><span data-stu-id="09ffc-111">Type</span></span>   |<span data-ttu-id="09ffc-112">说明</span><span class="sxs-lookup"><span data-stu-id="09ffc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09ffc-113">category1</span><span class="sxs-lookup"><span data-stu-id="09ffc-113">category1</span></span>|<span data-ttu-id="09ffc-114">String</span><span class="sxs-lookup"><span data-stu-id="09ffc-114">String</span></span>|<span data-ttu-id="09ffc-115">与类别1关联的标签</span><span class="sxs-lookup"><span data-stu-id="09ffc-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="09ffc-116">category2</span><span class="sxs-lookup"><span data-stu-id="09ffc-116">category2</span></span>|<span data-ttu-id="09ffc-117">String</span><span class="sxs-lookup"><span data-stu-id="09ffc-117">String</span></span>|<span data-ttu-id="09ffc-118">与类别2关联的标签</span><span class="sxs-lookup"><span data-stu-id="09ffc-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="09ffc-119">category3</span><span class="sxs-lookup"><span data-stu-id="09ffc-119">category3</span></span>|<span data-ttu-id="09ffc-120">String</span><span class="sxs-lookup"><span data-stu-id="09ffc-120">String</span></span>|<span data-ttu-id="09ffc-121">与类别3相关联的标签</span><span class="sxs-lookup"><span data-stu-id="09ffc-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="09ffc-122">category4</span><span class="sxs-lookup"><span data-stu-id="09ffc-122">category4</span></span>|<span data-ttu-id="09ffc-123">String</span><span class="sxs-lookup"><span data-stu-id="09ffc-123">String</span></span>|<span data-ttu-id="09ffc-124">与类别4关联的标签</span><span class="sxs-lookup"><span data-stu-id="09ffc-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="09ffc-125">category5</span><span class="sxs-lookup"><span data-stu-id="09ffc-125">category5</span></span>|<span data-ttu-id="09ffc-126">String</span><span class="sxs-lookup"><span data-stu-id="09ffc-126">String</span></span>|<span data-ttu-id="09ffc-127">与类别5相关联的标签</span><span class="sxs-lookup"><span data-stu-id="09ffc-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="09ffc-128">category6</span><span class="sxs-lookup"><span data-stu-id="09ffc-128">category6</span></span>|<span data-ttu-id="09ffc-129">String</span><span class="sxs-lookup"><span data-stu-id="09ffc-129">String</span></span>|<span data-ttu-id="09ffc-130">与类别6关联的标签</span><span class="sxs-lookup"><span data-stu-id="09ffc-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09ffc-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09ffc-131">JSON representation</span></span>
<span data-ttu-id="09ffc-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09ffc-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannercategorydescriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
