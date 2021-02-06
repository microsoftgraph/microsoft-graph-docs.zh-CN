---
title: attributeMappingSource 资源类型
description: 定义如何从源对象中提取 (或) 转换值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 50443eb85ed87bce466e7842f46d0c457f28e216
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133236"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="2ccd7-103">attributeMappingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ccd7-103">attributeMappingSource resource type</span></span>

<span data-ttu-id="2ccd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ccd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ccd7-105">定义如何从源对象中提取 (或) 转换值。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="2ccd7-106">例如，它可以是一个从源对象的给定属性提取的简单值，也可以是基于多个源属性的更复杂的字符串连接/提取/替换表达式。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="2ccd7-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ccd7-107">Properties</span></span>

| <span data-ttu-id="2ccd7-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ccd7-108">Property</span></span>              | <span data-ttu-id="2ccd7-109">类型</span><span class="sxs-lookup"><span data-stu-id="2ccd7-109">Type</span></span>                      | <span data-ttu-id="2ccd7-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ccd7-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="2ccd7-111">表达式</span><span class="sxs-lookup"><span data-stu-id="2ccd7-111">expression</span></span>             |<span data-ttu-id="2ccd7-112">字符串</span><span class="sxs-lookup"><span data-stu-id="2ccd7-112">String</span></span>                     |<span data-ttu-id="2ccd7-113">此 **attributeMappingSource 对象的等效表达式** 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="2ccd7-114">name</span><span class="sxs-lookup"><span data-stu-id="2ccd7-114">name</span></span>                   |<span data-ttu-id="2ccd7-115">字符串</span><span class="sxs-lookup"><span data-stu-id="2ccd7-115">String</span></span>                     |<span data-ttu-id="2ccd7-116">映射源的名称参数。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="2ccd7-117">根据 **类型** 属性值，它可以是函数的名称、源属性的名称或要使用的常量值。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="2ccd7-118">parameters</span><span class="sxs-lookup"><span data-stu-id="2ccd7-118">parameters</span></span>             |<span data-ttu-id="2ccd7-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ccd7-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="2ccd7-120">如果此对象代表函数，则列出函数参数。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="2ccd7-121">参数由 **attributeMappingSource** 对象本身组成，允许使用复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="2ccd7-122">如果 **type** 不是 `Function` ，则此属性将为 null/空数组。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="2ccd7-123">type</span><span class="sxs-lookup"><span data-stu-id="2ccd7-123">type</span></span>                   | <span data-ttu-id="2ccd7-124">字符串</span><span class="sxs-lookup"><span data-stu-id="2ccd7-124">String</span></span>                    |<span data-ttu-id="2ccd7-125">此属性映射源的类型。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="2ccd7-126">可取值为：`Attribute`、`Constant`、`Function`。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="2ccd7-127">默认值为“`Attribute`”。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-127">Default is `Attribute`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ccd7-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ccd7-128">JSON representation</span></span>

<span data-ttu-id="2ccd7-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ccd7-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="2ccd7-130">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="2ccd7-130">JSON Examples</span></span>

<span data-ttu-id="2ccd7-131">简单属性到属性映射</span><span class="sxs-lookup"><span data-stu-id="2ccd7-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="2ccd7-132">从源属性提取前 8 个字符的表达式</span><span class="sxs-lookup"><span data-stu-id="2ccd7-132">Expression extracting first 8 characters from the source attribute</span></span>

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


