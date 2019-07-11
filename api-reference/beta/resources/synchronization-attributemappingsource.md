---
title: attributeMappingSource 资源类型
description: '定义应如何从源对象提取 (或转换) 值。 例如, 它可以是从源对象的给定属性中获取的简单值, 也可以是基于多个源属性的字符串串联/提取/替换的更复杂表达式。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0c5ef197a72767fb0c764689558b9c005be856f8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621450"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="2a147-104">attributeMappingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a147-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a147-105">定义应如何从源对象提取 (或转换) 值。</span><span class="sxs-lookup"><span data-stu-id="2a147-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="2a147-106">例如, 它可以是从源对象的给定属性中获取的简单值, 也可以是基于多个源属性的字符串串联/提取/替换的更复杂表达式。</span><span class="sxs-lookup"><span data-stu-id="2a147-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="2a147-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a147-107">Properties</span></span>

| <span data-ttu-id="2a147-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a147-108">Property</span></span>              | <span data-ttu-id="2a147-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a147-109">Type</span></span>                      | <span data-ttu-id="2a147-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a147-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="2a147-111">表达式</span><span class="sxs-lookup"><span data-stu-id="2a147-111">expression</span></span>             |<span data-ttu-id="2a147-112">String</span><span class="sxs-lookup"><span data-stu-id="2a147-112">String</span></span>                     |<span data-ttu-id="2a147-113">此**attributeMappingSource**对象的等效表达式表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a147-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="2a147-114">name</span><span class="sxs-lookup"><span data-stu-id="2a147-114">name</span></span>                   |<span data-ttu-id="2a147-115">String</span><span class="sxs-lookup"><span data-stu-id="2a147-115">String</span></span>                     |<span data-ttu-id="2a147-116">映射源的 Name 参数。</span><span class="sxs-lookup"><span data-stu-id="2a147-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="2a147-117">根据**type**属性值, 这可以是函数的名称、源属性的名称或要使用的常数值。</span><span class="sxs-lookup"><span data-stu-id="2a147-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="2a147-118">parameters</span><span class="sxs-lookup"><span data-stu-id="2a147-118">parameters</span></span>             |<span data-ttu-id="2a147-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="2a147-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="2a147-120">如果此对象代表函数, 则列出函数参数。</span><span class="sxs-lookup"><span data-stu-id="2a147-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="2a147-121">参数由**attributeMappingSource**对象本身组成, 从而允许复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="2a147-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="2a147-122">如果**type**不`Function`是, 则此属性将为 null/空数组。</span><span class="sxs-lookup"><span data-stu-id="2a147-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="2a147-123">type</span><span class="sxs-lookup"><span data-stu-id="2a147-123">type</span></span>                   | <span data-ttu-id="2a147-124">String</span><span class="sxs-lookup"><span data-stu-id="2a147-124">String</span></span>                    |<span data-ttu-id="2a147-125">此属性映射源的类型。</span><span class="sxs-lookup"><span data-stu-id="2a147-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="2a147-126">可取值为：`Attribute`、`Constant`、`Function`。</span><span class="sxs-lookup"><span data-stu-id="2a147-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="2a147-127">默认值为 `Attribute`。</span><span class="sxs-lookup"><span data-stu-id="2a147-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="2a147-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a147-128">JSON representation</span></span>

<span data-ttu-id="2a147-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a147-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a><span data-ttu-id="2a147-130">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="2a147-130">JSON Examples</span></span>

<span data-ttu-id="2a147-131">属性映射的简单属性</span><span class="sxs-lookup"><span data-stu-id="2a147-131">Simple attribute to attribute mapping</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

<span data-ttu-id="2a147-132">从 source 属性提取前8个字符的表达式</span><span class="sxs-lookup"><span data-stu-id="2a147-132">Expression extracting first 8 characters from the source attribute</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
