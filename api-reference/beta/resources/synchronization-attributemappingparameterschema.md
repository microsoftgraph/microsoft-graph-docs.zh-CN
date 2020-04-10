---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12f1a38340b4c341d65930000c22a6cd2daeb567
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219170"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="06d67-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="06d67-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="06d67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06d67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06d67-105">描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="06d67-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="06d67-106">属性</span><span class="sxs-lookup"><span data-stu-id="06d67-106">Properties</span></span>

| <span data-ttu-id="06d67-107">属性</span><span class="sxs-lookup"><span data-stu-id="06d67-107">Property</span></span>                   | <span data-ttu-id="06d67-108">类型</span><span class="sxs-lookup"><span data-stu-id="06d67-108">Type</span></span>                      | <span data-ttu-id="06d67-109">说明</span><span class="sxs-lookup"><span data-stu-id="06d67-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="06d67-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="06d67-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="06d67-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d67-111">Boolean</span></span>                   |<span data-ttu-id="06d67-112">给定参数可多次提供（例如， `Concatenate(string,string,...)`函数中的多个输入字符串）。</span><span class="sxs-lookup"><span data-stu-id="06d67-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="06d67-113">name</span><span class="sxs-lookup"><span data-stu-id="06d67-113">name</span></span>                        |<span data-ttu-id="06d67-114">String</span><span class="sxs-lookup"><span data-stu-id="06d67-114">String</span></span>                    |<span data-ttu-id="06d67-115">参数名称。</span><span class="sxs-lookup"><span data-stu-id="06d67-115">Parameter name.</span></span> |
|<span data-ttu-id="06d67-116">必需</span><span class="sxs-lookup"><span data-stu-id="06d67-116">required</span></span>                    |<span data-ttu-id="06d67-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d67-117">Boolean</span></span>                   |<span data-ttu-id="06d67-118">`true`如果参数是必需的;否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="06d67-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="06d67-119">type</span><span class="sxs-lookup"><span data-stu-id="06d67-119">type</span></span>                        |<span data-ttu-id="06d67-120">字符串</span><span class="sxs-lookup"><span data-stu-id="06d67-120">String</span></span>                    |<span data-ttu-id="06d67-121">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="06d67-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="06d67-122">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="06d67-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06d67-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06d67-123">JSON representation</span></span>

<span data-ttu-id="06d67-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06d67-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
