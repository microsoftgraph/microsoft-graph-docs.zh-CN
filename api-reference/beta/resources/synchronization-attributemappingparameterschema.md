---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c8779211382ffcf7284c5ebf4035be6134efd8bf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128734"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="2dd8d-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="2dd8d-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="2dd8d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dd8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dd8d-105">描述在 [attributeMappingFunctionSchema 中使用的单个参数](../resources/synchronization-attributemappingfunctionschema.md)。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2dd8d-106">属性</span><span class="sxs-lookup"><span data-stu-id="2dd8d-106">Properties</span></span>

| <span data-ttu-id="2dd8d-107">属性</span><span class="sxs-lookup"><span data-stu-id="2dd8d-107">Property</span></span>                   | <span data-ttu-id="2dd8d-108">类型</span><span class="sxs-lookup"><span data-stu-id="2dd8d-108">Type</span></span>                      | <span data-ttu-id="2dd8d-109">说明</span><span class="sxs-lookup"><span data-stu-id="2dd8d-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="2dd8d-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="2dd8d-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="2dd8d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dd8d-111">Boolean</span></span>                   |<span data-ttu-id="2dd8d-112">给定的参数可以多次提供， (例如，函数中的多个输入 `Concatenate(string,string,...)` 字符串) 。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="2dd8d-113">name</span><span class="sxs-lookup"><span data-stu-id="2dd8d-113">name</span></span>                        |<span data-ttu-id="2dd8d-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2dd8d-114">String</span></span>                    |<span data-ttu-id="2dd8d-115">参数名称。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-115">Parameter name.</span></span> |
|<span data-ttu-id="2dd8d-116">必需</span><span class="sxs-lookup"><span data-stu-id="2dd8d-116">required</span></span>                    |<span data-ttu-id="2dd8d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dd8d-117">Boolean</span></span>                   |<span data-ttu-id="2dd8d-118">`true` 如果需要参数;否则 `false` 。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="2dd8d-119">type</span><span class="sxs-lookup"><span data-stu-id="2dd8d-119">type</span></span>                        |<span data-ttu-id="2dd8d-120">字符串</span><span class="sxs-lookup"><span data-stu-id="2dd8d-120">String</span></span>                    |<span data-ttu-id="2dd8d-121">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="2dd8d-122">默认值为“`String`”。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dd8d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2dd8d-123">JSON representation</span></span>

<span data-ttu-id="2dd8d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dd8d-124">The following is a JSON representation of the resource.</span></span>

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


