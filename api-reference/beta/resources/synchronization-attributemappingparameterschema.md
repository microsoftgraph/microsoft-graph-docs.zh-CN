---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14be19389d7c84c3e1a212239f2ba9e414927254
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964827"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="60469-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="60469-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60469-104">描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="60469-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="60469-105">属性</span><span class="sxs-lookup"><span data-stu-id="60469-105">Properties</span></span>

| <span data-ttu-id="60469-106">属性</span><span class="sxs-lookup"><span data-stu-id="60469-106">Property</span></span>                   | <span data-ttu-id="60469-107">类型</span><span class="sxs-lookup"><span data-stu-id="60469-107">Type</span></span>                      | <span data-ttu-id="60469-108">说明</span><span class="sxs-lookup"><span data-stu-id="60469-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="60469-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="60469-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="60469-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="60469-110">Boolean</span></span>                   |<span data-ttu-id="60469-111">给定参数可多次提供 (例如, `Concatenate(string,string,...)`函数中的多个输入字符串)。</span><span class="sxs-lookup"><span data-stu-id="60469-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="60469-112">name</span><span class="sxs-lookup"><span data-stu-id="60469-112">name</span></span>                        |<span data-ttu-id="60469-113">String</span><span class="sxs-lookup"><span data-stu-id="60469-113">String</span></span>                    |<span data-ttu-id="60469-114">参数名称。</span><span class="sxs-lookup"><span data-stu-id="60469-114">Parameter name.</span></span> |
|<span data-ttu-id="60469-115">必需</span><span class="sxs-lookup"><span data-stu-id="60469-115">required</span></span>                    |<span data-ttu-id="60469-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="60469-116">Boolean</span></span>                   |<span data-ttu-id="60469-117">`true`如果参数是必需的;否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="60469-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="60469-118">type</span><span class="sxs-lookup"><span data-stu-id="60469-118">type</span></span>                        |<span data-ttu-id="60469-119">String</span><span class="sxs-lookup"><span data-stu-id="60469-119">String</span></span>                    |<span data-ttu-id="60469-120">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="60469-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="60469-121">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="60469-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60469-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60469-122">JSON representation</span></span>

<span data-ttu-id="60469-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60469-123">The following is a JSON representation of the resource.</span></span>

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
