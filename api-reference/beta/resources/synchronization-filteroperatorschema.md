---
title: filterOperatorSchema 资源类型
description: 介绍可在筛选器中使用的运算符。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e80b80a7f37af8b86dfd3925fe268dba89cea17
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217810"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="dbac6-103">filterOperatorSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="dbac6-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="dbac6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbac6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbac6-105">介绍可在[筛选器](synchronization-filter.md)中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="dbac6-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dbac6-106">属性</span><span class="sxs-lookup"><span data-stu-id="dbac6-106">Properties</span></span>

| <span data-ttu-id="dbac6-107">属性</span><span class="sxs-lookup"><span data-stu-id="dbac6-107">Property</span></span>                   | <span data-ttu-id="dbac6-108">类型</span><span class="sxs-lookup"><span data-stu-id="dbac6-108">Type</span></span>                      | <span data-ttu-id="dbac6-109">说明</span><span class="sxs-lookup"><span data-stu-id="dbac6-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="dbac6-110">源语言</span><span class="sxs-lookup"><span data-stu-id="dbac6-110">arity</span></span>                       |<span data-ttu-id="dbac6-111">字符串</span><span class="sxs-lookup"><span data-stu-id="dbac6-111">String</span></span>          |<span data-ttu-id="dbac6-112">运算符的 Arity。</span><span class="sxs-lookup"><span data-stu-id="dbac6-112">Arity of the operator.</span></span> <span data-ttu-id="dbac6-113">可取值为：`Binary`、`Unary`。</span><span class="sxs-lookup"><span data-stu-id="dbac6-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="dbac6-114">默认值为`Binary`。</span><span class="sxs-lookup"><span data-stu-id="dbac6-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="dbac6-115">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="dbac6-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="dbac6-116">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="dbac6-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="dbac6-117">可取值为：`All`、`Any`。</span><span class="sxs-lookup"><span data-stu-id="dbac6-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="dbac6-118">仅适用于多值属性。</span><span class="sxs-lookup"><span data-stu-id="dbac6-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="dbac6-119">`All`表示所有值都必须满足条件。</span><span class="sxs-lookup"><span data-stu-id="dbac6-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="dbac6-120">`Any`表示必须至少有一个值满足条件。</span><span class="sxs-lookup"><span data-stu-id="dbac6-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="dbac6-121">默认值为`All`。</span><span class="sxs-lookup"><span data-stu-id="dbac6-121">The default is `All`.</span></span>|
|<span data-ttu-id="dbac6-122">name</span><span class="sxs-lookup"><span data-stu-id="dbac6-122">name</span></span>                        |<span data-ttu-id="dbac6-123">字符串</span><span class="sxs-lookup"><span data-stu-id="dbac6-123">String</span></span>                     |<span data-ttu-id="dbac6-124">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="dbac6-124">Operator name.</span></span> |
|<span data-ttu-id="dbac6-125">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="dbac6-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="dbac6-126">String collection</span><span class="sxs-lookup"><span data-stu-id="dbac6-126">String collection</span></span>         |<span data-ttu-id="dbac6-127">运算符支持的属性类型。</span><span class="sxs-lookup"><span data-stu-id="dbac6-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="dbac6-128">可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。</span><span class="sxs-lookup"><span data-stu-id="dbac6-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbac6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dbac6-129">JSON representation</span></span>

<span data-ttu-id="dbac6-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbac6-130">The following is a JSON representation of the resource.</span></span>

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
