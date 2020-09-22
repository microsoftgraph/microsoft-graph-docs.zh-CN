---
title: rubricCriterion 资源类型
description: Rubric 的一个条件
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60123251d771d06032077231250efe53b35a787c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016103"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="2a569-103">rubricCriterion 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a569-103">rubricCriterion resource type</span></span>

<span data-ttu-id="2a569-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a569-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a569-105">Rubric 的一个条件。</span><span class="sxs-lookup"><span data-stu-id="2a569-105">A criterion of a rubric.</span></span> <span data-ttu-id="2a569-106">有关 rubric*质量*、*级别*和*条件*之间的关系的说明，请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="2a569-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="2a569-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a569-107">Properties</span></span>

| <span data-ttu-id="2a569-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a569-108">Property</span></span>     | <span data-ttu-id="2a569-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a569-109">Type</span></span>        | <span data-ttu-id="2a569-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a569-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a569-111">说明</span><span class="sxs-lookup"><span data-stu-id="2a569-111">description</span></span>|[<span data-ttu-id="2a569-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="2a569-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="2a569-113">此条件的说明。</span><span class="sxs-lookup"><span data-stu-id="2a569-113">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a569-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a569-114">JSON representation</span></span>

<span data-ttu-id="2a569-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a569-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricCriterion",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricCriterion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

