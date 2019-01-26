---
title: filterOperatorSchema 资源类型
description: 介绍可用于筛选器运算符。
localization_priority: Normal
ms.openlocfilehash: 366e00b5d21efeaf67e3e799c5b1c2412a68e268
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573677"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="bc5ea-103">filterOperatorSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc5ea-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc5ea-104">介绍可用于[筛选器](synchronization-filter.md)运算符。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bc5ea-105">属性</span><span class="sxs-lookup"><span data-stu-id="bc5ea-105">Properties</span></span>

| <span data-ttu-id="bc5ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="bc5ea-106">Property</span></span>                   | <span data-ttu-id="bc5ea-107">类型</span><span class="sxs-lookup"><span data-stu-id="bc5ea-107">Type</span></span>                      | <span data-ttu-id="bc5ea-108">说明</span><span class="sxs-lookup"><span data-stu-id="bc5ea-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="bc5ea-109">实参数量</span><span class="sxs-lookup"><span data-stu-id="bc5ea-109">arity</span></span>                       | <span data-ttu-id="bc5ea-110">microsoft.graph.scopeOperatorType</span><span class="sxs-lookup"><span data-stu-id="bc5ea-110">microsoft.graph.scopeOperatorType</span></span>         |<span data-ttu-id="bc5ea-111">实参运算符的数量。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-111">Arity of the operator.</span></span> <span data-ttu-id="bc5ea-112">可取值为：`Binary`、`Unary`。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="bc5ea-113">默认值是`Binary`。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="bc5ea-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="bc5ea-114">multivaluedComparisonType</span></span>   | <span data-ttu-id="bc5ea-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="bc5ea-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="bc5ea-116">可取值为：`All`、`Any`。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="bc5ea-117">仅适用于多值属性。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="bc5ea-118">`All`所有的值必须满足条件的方法。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="bc5ea-119">`Any`至少一个值必须满足条件的方法。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="bc5ea-120">默认值是`All`。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-120">The default is `All`.</span></span>|
|<span data-ttu-id="bc5ea-121">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="bc5ea-121">supportedAttributeTypes</span></span>     | <span data-ttu-id="bc5ea-122">特性类型集合</span><span class="sxs-lookup"><span data-stu-id="bc5ea-122">attributeType collection</span></span>         |<span data-ttu-id="bc5ea-123">属性类型支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-123">Attribute types supported by the operator.</span></span> <span data-ttu-id="bc5ea-124">可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-124">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc5ea-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc5ea-125">JSON representation</span></span>

<span data-ttu-id="bc5ea-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc5ea-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "microsoft.graph.scopeOperatorType",
  "multivaluedComparisonType": "microsoft.graph.scopeOperatorMultiValuedComparisonType",  
  "supportedAttributeTypes": ["attributeType"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
