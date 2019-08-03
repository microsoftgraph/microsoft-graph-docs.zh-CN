---
title: rubricCriterion 资源类型
description: Rubric 的一个条件
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 250132ab5304ab9df94707349df951e5b1e995a6
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173340"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="1a043-103">rubricCriterion 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a043-103">rubricCriterion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a043-104">Rubric 的一个条件。</span><span class="sxs-lookup"><span data-stu-id="1a043-104">A criterion of a rubric.</span></span> <span data-ttu-id="1a043-105">有关 rubric*质量*、*级别*和*条件*之间的关系的说明, 请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="1a043-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="1a043-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a043-106">Properties</span></span>

| <span data-ttu-id="1a043-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a043-107">Property</span></span>     | <span data-ttu-id="1a043-108">类型</span><span class="sxs-lookup"><span data-stu-id="1a043-108">Type</span></span>        | <span data-ttu-id="1a043-109">说明</span><span class="sxs-lookup"><span data-stu-id="1a043-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a043-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a043-110">description</span></span>|[<span data-ttu-id="1a043-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="1a043-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="1a043-112">此条件的说明。</span><span class="sxs-lookup"><span data-stu-id="1a043-112">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a043-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a043-113">JSON representation</span></span>

<span data-ttu-id="1a043-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a043-114">The following is a JSON representation of the resource.</span></span>

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