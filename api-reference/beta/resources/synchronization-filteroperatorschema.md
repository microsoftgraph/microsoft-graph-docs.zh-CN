---
title: filterOperatorSchema 资源类型
description: 介绍可用于筛选器运算符。
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042701"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="09bb7-103">filterOperatorSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="09bb7-103">filterOperatorSchema resource type</span></span>

> <span data-ttu-id="09bb7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09bb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09bb7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09bb7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09bb7-106">介绍可用于[筛选器](synchronization-filter.md)运算符。</span><span class="sxs-lookup"><span data-stu-id="09bb7-106">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="09bb7-107">属性</span><span class="sxs-lookup"><span data-stu-id="09bb7-107">Properties</span></span>

| <span data-ttu-id="09bb7-108">属性</span><span class="sxs-lookup"><span data-stu-id="09bb7-108">Property</span></span>                   | <span data-ttu-id="09bb7-109">类型</span><span class="sxs-lookup"><span data-stu-id="09bb7-109">Type</span></span>                      | <span data-ttu-id="09bb7-110">说明</span><span class="sxs-lookup"><span data-stu-id="09bb7-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="09bb7-111">实参数量</span><span class="sxs-lookup"><span data-stu-id="09bb7-111">arity</span></span>                       |<span data-ttu-id="09bb7-112">字符串</span><span class="sxs-lookup"><span data-stu-id="09bb7-112">String</span></span>          |<span data-ttu-id="09bb7-113">实参运算符的数量。</span><span class="sxs-lookup"><span data-stu-id="09bb7-113">Arity of the operator.</span></span> <span data-ttu-id="09bb7-114">可取值为：`Binary`、`Unary`。</span><span class="sxs-lookup"><span data-stu-id="09bb7-114">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="09bb7-115">默认值是`Binary`。</span><span class="sxs-lookup"><span data-stu-id="09bb7-115">The default is `Binary`.</span></span>|
|<span data-ttu-id="09bb7-116">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="09bb7-116">multivaluedComparisonType</span></span>   |<span data-ttu-id="09bb7-117">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="09bb7-117">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="09bb7-118">可取值为：`All`、`Any`。</span><span class="sxs-lookup"><span data-stu-id="09bb7-118">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="09bb7-119">仅适用于多值属性。</span><span class="sxs-lookup"><span data-stu-id="09bb7-119">Applies only to multivalued attributes.</span></span> <span data-ttu-id="09bb7-120">`All`所有的值必须满足条件的方法。</span><span class="sxs-lookup"><span data-stu-id="09bb7-120">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="09bb7-121">`Any`至少一个值必须满足条件的方法。</span><span class="sxs-lookup"><span data-stu-id="09bb7-121">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="09bb7-122">默认值是`All`。</span><span class="sxs-lookup"><span data-stu-id="09bb7-122">The default is `All`.</span></span>|
|<span data-ttu-id="09bb7-123">name</span><span class="sxs-lookup"><span data-stu-id="09bb7-123">name</span></span>                        |<span data-ttu-id="09bb7-124">字符串</span><span class="sxs-lookup"><span data-stu-id="09bb7-124">String</span></span>                     |<span data-ttu-id="09bb7-125">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="09bb7-125">Operator name.</span></span> |
|<span data-ttu-id="09bb7-126">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="09bb7-126">supportedAttributeTypes</span></span>     |<span data-ttu-id="09bb7-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="09bb7-127">String collection</span></span>         |<span data-ttu-id="09bb7-128">属性类型支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="09bb7-128">Attribute types supported by the operator.</span></span> <span data-ttu-id="09bb7-129">可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。</span><span class="sxs-lookup"><span data-stu-id="09bb7-129">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09bb7-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09bb7-130">JSON representation</span></span>

<span data-ttu-id="09bb7-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09bb7-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->