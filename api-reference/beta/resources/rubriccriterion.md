---
title: rubricCriterion 资源类型
description: Rubric 的一个条件
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e1a2a0550a7e1f9f5865b8381b3f730d31cac6b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521017"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="ce875-103">rubricCriterion 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce875-103">rubricCriterion resource type</span></span>

<span data-ttu-id="ce875-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ce875-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce875-105">Rubric 的一个条件。</span><span class="sxs-lookup"><span data-stu-id="ce875-105">A criterion of a rubric.</span></span> <span data-ttu-id="ce875-106">有关 rubric*质量*、*级别*和*条件*之间的关系的说明，请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="ce875-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="ce875-107">属性</span><span class="sxs-lookup"><span data-stu-id="ce875-107">Properties</span></span>

| <span data-ttu-id="ce875-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce875-108">Property</span></span>     | <span data-ttu-id="ce875-109">类型</span><span class="sxs-lookup"><span data-stu-id="ce875-109">Type</span></span>        | <span data-ttu-id="ce875-110">说明</span><span class="sxs-lookup"><span data-stu-id="ce875-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce875-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce875-111">description</span></span>|[<span data-ttu-id="ce875-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="ce875-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="ce875-113">此条件的说明。</span><span class="sxs-lookup"><span data-stu-id="ce875-113">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce875-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce875-114">JSON representation</span></span>

<span data-ttu-id="ce875-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce875-115">The following is a JSON representation of the resource.</span></span>

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