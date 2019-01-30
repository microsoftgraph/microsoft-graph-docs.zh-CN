---
title: filterOperatorSchema 资源类型
description: 介绍可用于筛选器运算符。
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641818"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="55682-103">filterOperatorSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="55682-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55682-104">介绍可用于[筛选器](synchronization-filter.md)运算符。</span><span class="sxs-lookup"><span data-stu-id="55682-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="55682-105">属性</span><span class="sxs-lookup"><span data-stu-id="55682-105">Properties</span></span>

| <span data-ttu-id="55682-106">属性</span><span class="sxs-lookup"><span data-stu-id="55682-106">Property</span></span>                   | <span data-ttu-id="55682-107">类型</span><span class="sxs-lookup"><span data-stu-id="55682-107">Type</span></span>                      | <span data-ttu-id="55682-108">说明</span><span class="sxs-lookup"><span data-stu-id="55682-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="55682-109">实参数量</span><span class="sxs-lookup"><span data-stu-id="55682-109">arity</span></span>                       |<span data-ttu-id="55682-110">String</span><span class="sxs-lookup"><span data-stu-id="55682-110">String</span></span>          |<span data-ttu-id="55682-111">实参运算符的数量。</span><span class="sxs-lookup"><span data-stu-id="55682-111">Arity of the operator.</span></span> <span data-ttu-id="55682-112">可取值为：`Binary`、`Unary`。</span><span class="sxs-lookup"><span data-stu-id="55682-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="55682-113">默认值是`Binary`。</span><span class="sxs-lookup"><span data-stu-id="55682-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="55682-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="55682-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="55682-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="55682-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="55682-116">可取值为：`All`、`Any`。</span><span class="sxs-lookup"><span data-stu-id="55682-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="55682-117">仅适用于多值属性。</span><span class="sxs-lookup"><span data-stu-id="55682-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="55682-118">`All`所有的值必须满足条件的方法。</span><span class="sxs-lookup"><span data-stu-id="55682-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="55682-119">`Any`至少一个值必须满足条件的方法。</span><span class="sxs-lookup"><span data-stu-id="55682-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="55682-120">默认值是`All`。</span><span class="sxs-lookup"><span data-stu-id="55682-120">The default is `All`.</span></span>|
|<span data-ttu-id="55682-121">name</span><span class="sxs-lookup"><span data-stu-id="55682-121">name</span></span>                        |<span data-ttu-id="55682-122">String</span><span class="sxs-lookup"><span data-stu-id="55682-122">String</span></span>                     |<span data-ttu-id="55682-123">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="55682-123">Operator name.</span></span> |
|<span data-ttu-id="55682-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="55682-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="55682-125">String collection</span><span class="sxs-lookup"><span data-stu-id="55682-125">String collection</span></span>         |<span data-ttu-id="55682-126">属性类型支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="55682-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="55682-127">可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。</span><span class="sxs-lookup"><span data-stu-id="55682-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55682-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55682-128">JSON representation</span></span>

<span data-ttu-id="55682-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55682-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
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
