---
title: rubricQualitySelectedColumnModel 资源类型
description: 指示在对 educationRubric 进行评分时教师选择的 rubricLevel
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a381ad878f16dab6197c72bd19d6f5aeee86f4a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016056"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="d7b04-103">rubricQualitySelectedColumnModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7b04-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="d7b04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7b04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b04-105">指示在向[educationRubric](educationrubric.md)评分时教师选择的[rubricLevel](rubriclevel.md) 。</span><span class="sxs-lookup"><span data-stu-id="d7b04-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d7b04-106">属性</span><span class="sxs-lookup"><span data-stu-id="d7b04-106">Properties</span></span>

| <span data-ttu-id="d7b04-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7b04-107">Property</span></span>     | <span data-ttu-id="d7b04-108">类型</span><span class="sxs-lookup"><span data-stu-id="d7b04-108">Type</span></span>        | <span data-ttu-id="d7b04-109">说明</span><span class="sxs-lookup"><span data-stu-id="d7b04-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7b04-110">columnId</span><span class="sxs-lookup"><span data-stu-id="d7b04-110">columnId</span></span>|<span data-ttu-id="d7b04-111">String</span><span class="sxs-lookup"><span data-stu-id="d7b04-111">String</span></span>|<span data-ttu-id="d7b04-112">此质量所对应的所选级别的 ID。</span><span class="sxs-lookup"><span data-stu-id="d7b04-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="d7b04-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="d7b04-113">qualityId</span></span>|<span data-ttu-id="d7b04-114">String</span><span class="sxs-lookup"><span data-stu-id="d7b04-114">String</span></span>|<span data-ttu-id="d7b04-115">关联质量的 ID。</span><span class="sxs-lookup"><span data-stu-id="d7b04-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7b04-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7b04-116">JSON representation</span></span>

<span data-ttu-id="d7b04-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7b04-117">The following is a JSON representation of the resource.</span></span>

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

