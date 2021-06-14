---
title: rubricCriterion 资源类型
description: 标准标准。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 21b79fd69649cf1afd340f422d544818bf247628
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912171"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="b4ad0-103">rubricCriterion 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4ad0-103">rubricCriterion resource type</span></span>

<span data-ttu-id="b4ad0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4ad0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4ad0-105">标准标准。</span><span class="sxs-lookup"><span data-stu-id="b4ad0-105">A criterion of a rubric.</span></span> 

<span data-ttu-id="b4ad0-106">有关标准质量、级别和条件之间的关系的说明，请参阅[educationRubric。](educationrubric.md) </span><span class="sxs-lookup"><span data-stu-id="b4ad0-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="b4ad0-107">属性</span><span class="sxs-lookup"><span data-stu-id="b4ad0-107">Properties</span></span>

| <span data-ttu-id="b4ad0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4ad0-108">Property</span></span>     | <span data-ttu-id="b4ad0-109">类型</span><span class="sxs-lookup"><span data-stu-id="b4ad0-109">Type</span></span>        | <span data-ttu-id="b4ad0-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4ad0-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4ad0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4ad0-111">description</span></span>|[<span data-ttu-id="b4ad0-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="b4ad0-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="b4ad0-113">此条件的说明。</span><span class="sxs-lookup"><span data-stu-id="b4ad0-113">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4ad0-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4ad0-114">JSON representation</span></span>

<span data-ttu-id="b4ad0-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4ad0-115">The following is a JSON representation of the resource.</span></span>

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

