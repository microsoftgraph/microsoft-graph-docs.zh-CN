---
title: attributeMappingFunctionSchema 资源类型
description: 描述可在属性映射中使用的函数，以在同步期间转换值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a62d2d635504208fc8266e98add66a8503e3e4d2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128741"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="dd8a0-103">attributeMappingFunctionSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd8a0-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="dd8a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd8a0-105">描述可在属性映射中使用的函数 [，](synchronization-attributemapping.md) 以在同步期间转换值。</span><span class="sxs-lookup"><span data-stu-id="dd8a0-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="dd8a0-106">方法</span><span class="sxs-lookup"><span data-stu-id="dd8a0-106">Methods</span></span>

| <span data-ttu-id="dd8a0-107">方法</span><span class="sxs-lookup"><span data-stu-id="dd8a0-107">Method</span></span>           | <span data-ttu-id="dd8a0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd8a0-108">Return Type</span></span>    |<span data-ttu-id="dd8a0-109">Description</span><span class="sxs-lookup"><span data-stu-id="dd8a0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd8a0-110">List</span><span class="sxs-lookup"><span data-stu-id="dd8a0-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="dd8a0-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd8a0-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="dd8a0-112">列出支持的属性映射函数。</span><span class="sxs-lookup"><span data-stu-id="dd8a0-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd8a0-113">属性</span><span class="sxs-lookup"><span data-stu-id="dd8a0-113">Properties</span></span>

| <span data-ttu-id="dd8a0-114">属性</span><span class="sxs-lookup"><span data-stu-id="dd8a0-114">Property</span></span>                   | <span data-ttu-id="dd8a0-115">类型</span><span class="sxs-lookup"><span data-stu-id="dd8a0-115">Type</span></span>                      | <span data-ttu-id="dd8a0-116">说明</span><span class="sxs-lookup"><span data-stu-id="dd8a0-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="dd8a0-117">name</span><span class="sxs-lookup"><span data-stu-id="dd8a0-117">name</span></span>                        |<span data-ttu-id="dd8a0-118">字符串</span><span class="sxs-lookup"><span data-stu-id="dd8a0-118">String</span></span>                    |<span data-ttu-id="dd8a0-119">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="dd8a0-119">Operator name.</span></span> |
|<span data-ttu-id="dd8a0-120">parameters</span><span class="sxs-lookup"><span data-stu-id="dd8a0-120">parameters</span></span>                  |<span data-ttu-id="dd8a0-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd8a0-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="dd8a0-122">函数参数的集合。</span><span class="sxs-lookup"><span data-stu-id="dd8a0-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd8a0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd8a0-123">JSON representation</span></span>

<span data-ttu-id="dd8a0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd8a0-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


