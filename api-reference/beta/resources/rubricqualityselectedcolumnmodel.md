---
title: rubricQualitySelectedColumnModel 资源类型
description: 指示在对 educationRubric 进行评分时教师选择的 rubricLevel
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6fd6ff5d9def23a6a6fb180c8d12398437e5dce0
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173291"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="b68bc-103">rubricQualitySelectedColumnModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="b68bc-103">rubricQualitySelectedColumnModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b68bc-104">指示在向[educationRubric](educationrubric.md)评分时教师选择的[rubricLevel](rubriclevel.md) 。</span><span class="sxs-lookup"><span data-stu-id="b68bc-104">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b68bc-105">属性</span><span class="sxs-lookup"><span data-stu-id="b68bc-105">Properties</span></span>

| <span data-ttu-id="b68bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="b68bc-106">Property</span></span>     | <span data-ttu-id="b68bc-107">类型</span><span class="sxs-lookup"><span data-stu-id="b68bc-107">Type</span></span>        | <span data-ttu-id="b68bc-108">说明</span><span class="sxs-lookup"><span data-stu-id="b68bc-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b68bc-109">columnId</span><span class="sxs-lookup"><span data-stu-id="b68bc-109">columnId</span></span>|<span data-ttu-id="b68bc-110">String</span><span class="sxs-lookup"><span data-stu-id="b68bc-110">String</span></span>|<span data-ttu-id="b68bc-111">此质量所对应的所选级别的 ID。</span><span class="sxs-lookup"><span data-stu-id="b68bc-111">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="b68bc-112">qualityId</span><span class="sxs-lookup"><span data-stu-id="b68bc-112">qualityId</span></span>|<span data-ttu-id="b68bc-113">String</span><span class="sxs-lookup"><span data-stu-id="b68bc-113">String</span></span>|<span data-ttu-id="b68bc-114">关联质量的 ID。</span><span class="sxs-lookup"><span data-stu-id="b68bc-114">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b68bc-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b68bc-115">JSON representation</span></span>

<span data-ttu-id="b68bc-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b68bc-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->