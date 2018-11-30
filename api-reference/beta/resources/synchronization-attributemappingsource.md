---
title: attributeMappingSource 资源类型
description: '定义如何值应为源对象中提取 （或转换）。 例如，它可以是简单取自源对象上, 一个给定属性的值或它可以是字符串串联/提取/替换基于多个源属性更为复杂的表达式。 '
ms.openlocfilehash: aeb39c829d7be081fe9ee08aa5845e6ced1194dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044823"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="91768-104">attributeMappingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="91768-104">attributeMappingSource resource type</span></span>

> <span data-ttu-id="91768-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91768-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91768-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91768-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91768-107">定义如何值应为源对象中提取 （或转换）。</span><span class="sxs-lookup"><span data-stu-id="91768-107">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="91768-108">例如，它可以是简单取自源对象上, 一个给定属性的值或它可以是字符串串联/提取/替换基于多个源属性更为复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="91768-108">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="91768-109">属性</span><span class="sxs-lookup"><span data-stu-id="91768-109">Properties</span></span>

| <span data-ttu-id="91768-110">属性</span><span class="sxs-lookup"><span data-stu-id="91768-110">Property</span></span>              | <span data-ttu-id="91768-111">类型</span><span class="sxs-lookup"><span data-stu-id="91768-111">Type</span></span>                      | <span data-ttu-id="91768-112">说明</span><span class="sxs-lookup"><span data-stu-id="91768-112">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="91768-113">表达式</span><span class="sxs-lookup"><span data-stu-id="91768-113">expression</span></span>             |<span data-ttu-id="91768-114">字符串</span><span class="sxs-lookup"><span data-stu-id="91768-114">String</span></span>                     |<span data-ttu-id="91768-115">此**attributeMappingSource**对象的表达式等效表示形式。</span><span class="sxs-lookup"><span data-stu-id="91768-115">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="91768-116">name</span><span class="sxs-lookup"><span data-stu-id="91768-116">name</span></span>                   |<span data-ttu-id="91768-117">字符串</span><span class="sxs-lookup"><span data-stu-id="91768-117">String</span></span>                     |<span data-ttu-id="91768-118">映射源名称参数。</span><span class="sxs-lookup"><span data-stu-id="91768-118">Name parameter of the mapping source.</span></span> <span data-ttu-id="91768-119">具体取决于**type**属性值，这可以是函数，源属性或用于以常量值的名称的名称。</span><span class="sxs-lookup"><span data-stu-id="91768-119">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="91768-120">parameters</span><span class="sxs-lookup"><span data-stu-id="91768-120">parameters</span></span>             |<span data-ttu-id="91768-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="91768-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="91768-122">如果该对象代表一个函数，列出函数参数。</span><span class="sxs-lookup"><span data-stu-id="91768-122">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="91768-123">参数包含**attributeMappingSource**对象本身，允许使用复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="91768-123">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="91768-124">如果**类型**不是`Function`，此属性将为空数组。</span><span class="sxs-lookup"><span data-stu-id="91768-124">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="91768-125">type</span><span class="sxs-lookup"><span data-stu-id="91768-125">type</span></span>                   | <span data-ttu-id="91768-126">字符串</span><span class="sxs-lookup"><span data-stu-id="91768-126">String</span></span>                    |<span data-ttu-id="91768-127">此属性映射源的类型。</span><span class="sxs-lookup"><span data-stu-id="91768-127">The type of this attribute mapping source.</span></span> <span data-ttu-id="91768-128">可取值为：`Attribute`、`Constant`、`Function`。</span><span class="sxs-lookup"><span data-stu-id="91768-128">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="91768-129">默认值为 `Attribute`。</span><span class="sxs-lookup"><span data-stu-id="91768-129">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="91768-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91768-130">JSON representation</span></span>

<span data-ttu-id="91768-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91768-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="91768-132">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="91768-132">JSON Examples</span></span>

<span data-ttu-id="91768-133">简单属性对属性映射</span><span class="sxs-lookup"><span data-stu-id="91768-133">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="91768-134">源属性中提取前 8 个字符的表达式</span><span class="sxs-lookup"><span data-stu-id="91768-134">Expression extracting first 8 characters from the source attribute</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
