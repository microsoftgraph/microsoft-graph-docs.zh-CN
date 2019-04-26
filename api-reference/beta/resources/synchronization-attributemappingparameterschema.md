---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
ms.openlocfilehash: 44234e7e76b5b0d0fb514366be6106c8177b56db
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342926"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="b81c3-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="b81c3-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b81c3-104">描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="b81c3-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b81c3-105">属性</span><span class="sxs-lookup"><span data-stu-id="b81c3-105">Properties</span></span>

| <span data-ttu-id="b81c3-106">属性</span><span class="sxs-lookup"><span data-stu-id="b81c3-106">Property</span></span>                   | <span data-ttu-id="b81c3-107">类型</span><span class="sxs-lookup"><span data-stu-id="b81c3-107">Type</span></span>                      | <span data-ttu-id="b81c3-108">说明</span><span class="sxs-lookup"><span data-stu-id="b81c3-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="b81c3-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="b81c3-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="b81c3-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="b81c3-110">Boolean</span></span>                   |<span data-ttu-id="b81c3-111">给定参数可多次提供 (例如, `Concatenate(string,string,...)`函数中的多个输入字符串)。</span><span class="sxs-lookup"><span data-stu-id="b81c3-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="b81c3-112">name</span><span class="sxs-lookup"><span data-stu-id="b81c3-112">name</span></span>                        |<span data-ttu-id="b81c3-113">String</span><span class="sxs-lookup"><span data-stu-id="b81c3-113">String</span></span>                    |<span data-ttu-id="b81c3-114">参数名称。</span><span class="sxs-lookup"><span data-stu-id="b81c3-114">Parameter name.</span></span> |
|<span data-ttu-id="b81c3-115">必需</span><span class="sxs-lookup"><span data-stu-id="b81c3-115">required</span></span>                    |<span data-ttu-id="b81c3-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b81c3-116">Boolean</span></span>                   |<span data-ttu-id="b81c3-117">`true`如果参数是必需的;否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="b81c3-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="b81c3-118">type</span><span class="sxs-lookup"><span data-stu-id="b81c3-118">type</span></span>                        |<span data-ttu-id="b81c3-119">String</span><span class="sxs-lookup"><span data-stu-id="b81c3-119">String</span></span>                    |<span data-ttu-id="b81c3-120">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="b81c3-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="b81c3-121">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="b81c3-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b81c3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b81c3-122">JSON representation</span></span>

<span data-ttu-id="b81c3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b81c3-123">The following is a JSON representation of the resource.</span></span>

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
