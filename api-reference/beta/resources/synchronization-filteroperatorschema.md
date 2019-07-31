---
title: filterOperatorSchema 资源类型
description: 介绍可在筛选器中使用的运算符。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2ed9ef208f888026224293ff86a36b62a3486d48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007891"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="40b68-103">filterOperatorSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="40b68-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b68-104">介绍可在[筛选器](synchronization-filter.md)中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="40b68-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="40b68-105">属性</span><span class="sxs-lookup"><span data-stu-id="40b68-105">Properties</span></span>

| <span data-ttu-id="40b68-106">属性</span><span class="sxs-lookup"><span data-stu-id="40b68-106">Property</span></span>                   | <span data-ttu-id="40b68-107">类型</span><span class="sxs-lookup"><span data-stu-id="40b68-107">Type</span></span>                      | <span data-ttu-id="40b68-108">说明</span><span class="sxs-lookup"><span data-stu-id="40b68-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="40b68-109">源语言</span><span class="sxs-lookup"><span data-stu-id="40b68-109">arity</span></span>                       |<span data-ttu-id="40b68-110">String</span><span class="sxs-lookup"><span data-stu-id="40b68-110">String</span></span>          |<span data-ttu-id="40b68-111">运算符的 Arity。</span><span class="sxs-lookup"><span data-stu-id="40b68-111">Arity of the operator.</span></span> <span data-ttu-id="40b68-112">可取值为：`Binary`、`Unary`。</span><span class="sxs-lookup"><span data-stu-id="40b68-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="40b68-113">默认值为`Binary`。</span><span class="sxs-lookup"><span data-stu-id="40b68-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="40b68-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="40b68-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="40b68-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="40b68-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="40b68-116">可取值为：`All`、`Any`。</span><span class="sxs-lookup"><span data-stu-id="40b68-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="40b68-117">仅适用于多值属性。</span><span class="sxs-lookup"><span data-stu-id="40b68-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="40b68-118">`All`表示所有值都必须满足条件。</span><span class="sxs-lookup"><span data-stu-id="40b68-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="40b68-119">`Any`表示必须至少有一个值满足条件。</span><span class="sxs-lookup"><span data-stu-id="40b68-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="40b68-120">默认值为`All`。</span><span class="sxs-lookup"><span data-stu-id="40b68-120">The default is `All`.</span></span>|
|<span data-ttu-id="40b68-121">name</span><span class="sxs-lookup"><span data-stu-id="40b68-121">name</span></span>                        |<span data-ttu-id="40b68-122">String</span><span class="sxs-lookup"><span data-stu-id="40b68-122">String</span></span>                     |<span data-ttu-id="40b68-123">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="40b68-123">Operator name.</span></span> |
|<span data-ttu-id="40b68-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="40b68-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="40b68-125">String collection</span><span class="sxs-lookup"><span data-stu-id="40b68-125">String collection</span></span>         |<span data-ttu-id="40b68-126">运算符支持的属性类型。</span><span class="sxs-lookup"><span data-stu-id="40b68-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="40b68-127">可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。</span><span class="sxs-lookup"><span data-stu-id="40b68-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40b68-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40b68-128">JSON representation</span></span>

<span data-ttu-id="40b68-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40b68-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
