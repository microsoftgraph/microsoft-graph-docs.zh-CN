---
title: attributeMappingSource 资源类型
description: '定义应如何从源对象提取（或转换）值。 例如，它可以是从源对象的给定属性中获取的简单值，也可以是基于多个源属性的字符串串联/提取/替换的更复杂表达式。 '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 969f262f76f976c13f5c0a26ae53d67751b8820b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520231"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="5f620-104">attributeMappingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f620-104">attributeMappingSource resource type</span></span>

<span data-ttu-id="5f620-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5f620-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f620-106">定义应如何从源对象提取（或转换）值。</span><span class="sxs-lookup"><span data-stu-id="5f620-106">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="5f620-107">例如，它可以是从源对象的给定属性中获取的简单值，也可以是基于多个源属性的字符串串联/提取/替换的更复杂表达式。</span><span class="sxs-lookup"><span data-stu-id="5f620-107">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="5f620-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f620-108">Properties</span></span>

| <span data-ttu-id="5f620-109">属性</span><span class="sxs-lookup"><span data-stu-id="5f620-109">Property</span></span>              | <span data-ttu-id="5f620-110">类型</span><span class="sxs-lookup"><span data-stu-id="5f620-110">Type</span></span>                      | <span data-ttu-id="5f620-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f620-111">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="5f620-112">表达式</span><span class="sxs-lookup"><span data-stu-id="5f620-112">expression</span></span>             |<span data-ttu-id="5f620-113">String</span><span class="sxs-lookup"><span data-stu-id="5f620-113">String</span></span>                     |<span data-ttu-id="5f620-114">此**attributeMappingSource**对象的等效表达式表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f620-114">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="5f620-115">name</span><span class="sxs-lookup"><span data-stu-id="5f620-115">name</span></span>                   |<span data-ttu-id="5f620-116">String</span><span class="sxs-lookup"><span data-stu-id="5f620-116">String</span></span>                     |<span data-ttu-id="5f620-117">映射源的 Name 参数。</span><span class="sxs-lookup"><span data-stu-id="5f620-117">Name parameter of the mapping source.</span></span> <span data-ttu-id="5f620-118">根据**type**属性值，这可以是函数的名称、源属性的名称或要使用的常数值。</span><span class="sxs-lookup"><span data-stu-id="5f620-118">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="5f620-119">parameters</span><span class="sxs-lookup"><span data-stu-id="5f620-119">parameters</span></span>             |<span data-ttu-id="5f620-120">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="5f620-120">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="5f620-121">如果此对象代表函数，则列出函数参数。</span><span class="sxs-lookup"><span data-stu-id="5f620-121">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="5f620-122">参数由**attributeMappingSource**对象本身组成，从而允许复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="5f620-122">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="5f620-123">如果**type**不`Function`是，则此属性将为 null/空数组。</span><span class="sxs-lookup"><span data-stu-id="5f620-123">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="5f620-124">type</span><span class="sxs-lookup"><span data-stu-id="5f620-124">type</span></span>                   | <span data-ttu-id="5f620-125">String</span><span class="sxs-lookup"><span data-stu-id="5f620-125">String</span></span>                    |<span data-ttu-id="5f620-126">此属性映射源的类型。</span><span class="sxs-lookup"><span data-stu-id="5f620-126">The type of this attribute mapping source.</span></span> <span data-ttu-id="5f620-127">可取值为：`Attribute`、`Constant`、`Function`。</span><span class="sxs-lookup"><span data-stu-id="5f620-127">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="5f620-128">默认值为 `Attribute`。</span><span class="sxs-lookup"><span data-stu-id="5f620-128">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="5f620-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f620-129">JSON representation</span></span>

<span data-ttu-id="5f620-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f620-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="5f620-131">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="5f620-131">JSON Examples</span></span>

<span data-ttu-id="5f620-132">属性映射的简单属性</span><span class="sxs-lookup"><span data-stu-id="5f620-132">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="5f620-133">从 source 属性提取前8个字符的表达式</span><span class="sxs-lookup"><span data-stu-id="5f620-133">Expression extracting first 8 characters from the source attribute</span></span>

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
