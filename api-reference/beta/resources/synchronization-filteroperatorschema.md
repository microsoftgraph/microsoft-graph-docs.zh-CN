---
title: filterOperatorSchema 资源类型
description: 介绍可在筛选器中使用的运算符。
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581735"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="3377b-103">filterOperatorSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="3377b-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3377b-104">介绍可在[筛选器](synchronization-filter.md)中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="3377b-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3377b-105">属性</span><span class="sxs-lookup"><span data-stu-id="3377b-105">Properties</span></span>

| <span data-ttu-id="3377b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3377b-106">Property</span></span>                   | <span data-ttu-id="3377b-107">类型</span><span class="sxs-lookup"><span data-stu-id="3377b-107">Type</span></span>                      | <span data-ttu-id="3377b-108">说明</span><span class="sxs-lookup"><span data-stu-id="3377b-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="3377b-109">源语言</span><span class="sxs-lookup"><span data-stu-id="3377b-109">arity</span></span>                       |<span data-ttu-id="3377b-110">String</span><span class="sxs-lookup"><span data-stu-id="3377b-110">String</span></span>          |<span data-ttu-id="3377b-111">运算符的 Arity。</span><span class="sxs-lookup"><span data-stu-id="3377b-111">Arity of the operator.</span></span> <span data-ttu-id="3377b-112">可取值为：`Binary`、`Unary`。</span><span class="sxs-lookup"><span data-stu-id="3377b-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="3377b-113">默认值为`Binary`。</span><span class="sxs-lookup"><span data-stu-id="3377b-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="3377b-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="3377b-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="3377b-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="3377b-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="3377b-116">可取值为：`All`、`Any`。</span><span class="sxs-lookup"><span data-stu-id="3377b-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="3377b-117">仅适用于多值属性。</span><span class="sxs-lookup"><span data-stu-id="3377b-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="3377b-118">`All`表示所有值都必须满足条件。</span><span class="sxs-lookup"><span data-stu-id="3377b-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="3377b-119">`Any`表示必须至少有一个值满足条件。</span><span class="sxs-lookup"><span data-stu-id="3377b-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="3377b-120">默认值为`All`。</span><span class="sxs-lookup"><span data-stu-id="3377b-120">The default is `All`.</span></span>|
|<span data-ttu-id="3377b-121">name</span><span class="sxs-lookup"><span data-stu-id="3377b-121">name</span></span>                        |<span data-ttu-id="3377b-122">String</span><span class="sxs-lookup"><span data-stu-id="3377b-122">String</span></span>                     |<span data-ttu-id="3377b-123">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="3377b-123">Operator name.</span></span> |
|<span data-ttu-id="3377b-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="3377b-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="3377b-125">String collection</span><span class="sxs-lookup"><span data-stu-id="3377b-125">String collection</span></span>         |<span data-ttu-id="3377b-126">运算符支持的属性类型。</span><span class="sxs-lookup"><span data-stu-id="3377b-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="3377b-127">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="3377b-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3377b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3377b-128">JSON representation</span></span>

<span data-ttu-id="3377b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3377b-129">The following is a JSON representation of the resource.</span></span>

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
