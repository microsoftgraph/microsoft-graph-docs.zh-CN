---
title: attributeMappingSource 资源类型
description: '定义如何值应为源对象中提取 （或转换）。 例如，它可以是简单取自源对象上, 一个给定属性的值或它可以是字符串串联/提取/替换基于多个源属性更为复杂的表达式。 '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510405"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="1735f-104">attributeMappingSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="1735f-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1735f-105">定义如何值应为源对象中提取 （或转换）。</span><span class="sxs-lookup"><span data-stu-id="1735f-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="1735f-106">例如，它可以是简单取自源对象上, 一个给定属性的值或它可以是字符串串联/提取/替换基于多个源属性更为复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="1735f-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="1735f-107">属性</span><span class="sxs-lookup"><span data-stu-id="1735f-107">Properties</span></span>

| <span data-ttu-id="1735f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1735f-108">Property</span></span>              | <span data-ttu-id="1735f-109">类型</span><span class="sxs-lookup"><span data-stu-id="1735f-109">Type</span></span>                      | <span data-ttu-id="1735f-110">说明</span><span class="sxs-lookup"><span data-stu-id="1735f-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="1735f-111">表达式</span><span class="sxs-lookup"><span data-stu-id="1735f-111">expression</span></span>             |<span data-ttu-id="1735f-112">String</span><span class="sxs-lookup"><span data-stu-id="1735f-112">String</span></span>                     |<span data-ttu-id="1735f-113">此**attributeMappingSource**对象的表达式等效表示形式。</span><span class="sxs-lookup"><span data-stu-id="1735f-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="1735f-114">name</span><span class="sxs-lookup"><span data-stu-id="1735f-114">name</span></span>                   |<span data-ttu-id="1735f-115">String</span><span class="sxs-lookup"><span data-stu-id="1735f-115">String</span></span>                     |<span data-ttu-id="1735f-116">映射源名称参数。</span><span class="sxs-lookup"><span data-stu-id="1735f-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="1735f-117">具体取决于**type**属性值，这可以是函数，源属性或用于以常量值的名称的名称。</span><span class="sxs-lookup"><span data-stu-id="1735f-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="1735f-118">参数</span><span class="sxs-lookup"><span data-stu-id="1735f-118">parameters</span></span>             |<span data-ttu-id="1735f-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="1735f-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="1735f-120">如果该对象代表一个函数，列出函数参数。</span><span class="sxs-lookup"><span data-stu-id="1735f-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="1735f-121">参数包含**attributeMappingSource**对象本身，允许使用复杂的表达式。</span><span class="sxs-lookup"><span data-stu-id="1735f-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="1735f-122">如果**类型**不是`Function`，此属性将为空数组。</span><span class="sxs-lookup"><span data-stu-id="1735f-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="1735f-123">type</span><span class="sxs-lookup"><span data-stu-id="1735f-123">type</span></span>                   | <span data-ttu-id="1735f-124">String</span><span class="sxs-lookup"><span data-stu-id="1735f-124">String</span></span>                    |<span data-ttu-id="1735f-125">此属性映射源的类型。</span><span class="sxs-lookup"><span data-stu-id="1735f-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="1735f-126">可取值为：`Attribute`、`Constant`、`Function`。</span><span class="sxs-lookup"><span data-stu-id="1735f-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="1735f-127">默认值为 `Attribute`。</span><span class="sxs-lookup"><span data-stu-id="1735f-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="1735f-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1735f-128">JSON representation</span></span>

<span data-ttu-id="1735f-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1735f-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="1735f-130">JSON 示例</span><span class="sxs-lookup"><span data-stu-id="1735f-130">JSON Examples</span></span>

<span data-ttu-id="1735f-131">简单属性对属性映射</span><span class="sxs-lookup"><span data-stu-id="1735f-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="1735f-132">源属性中提取前 8 个字符的表达式</span><span class="sxs-lookup"><span data-stu-id="1735f-132">Expression extracting first 8 characters from the source attribute</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
