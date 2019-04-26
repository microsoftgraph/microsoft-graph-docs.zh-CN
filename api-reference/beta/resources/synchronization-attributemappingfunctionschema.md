---
title: attributeMappingFunctionSchema 资源类型
description: 介绍可在属性映射中用于在同步期间转换值的函数。
localization_priority: Normal
ms.openlocfilehash: ca66baf7fbc160cd4c57cba0f865ae07de9d5932
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345622"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="f46e4-103">attributeMappingFunctionSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="f46e4-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46e4-104">介绍可在[属性映射](synchronization-attributemapping.md)中用于在同步期间转换值的函数。</span><span class="sxs-lookup"><span data-stu-id="f46e4-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="f46e4-105">方法</span><span class="sxs-lookup"><span data-stu-id="f46e4-105">Methods</span></span>

| <span data-ttu-id="f46e4-106">方法</span><span class="sxs-lookup"><span data-stu-id="f46e4-106">Method</span></span>           | <span data-ttu-id="f46e4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f46e4-107">Return Type</span></span>    |<span data-ttu-id="f46e4-108">说明</span><span class="sxs-lookup"><span data-stu-id="f46e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f46e4-109">List</span><span class="sxs-lookup"><span data-stu-id="f46e4-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="f46e4-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="f46e4-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="f46e4-111">列出受支持的属性映射函数。</span><span class="sxs-lookup"><span data-stu-id="f46e4-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="f46e4-112">属性</span><span class="sxs-lookup"><span data-stu-id="f46e4-112">Properties</span></span>

| <span data-ttu-id="f46e4-113">属性</span><span class="sxs-lookup"><span data-stu-id="f46e4-113">Property</span></span>                   | <span data-ttu-id="f46e4-114">类型</span><span class="sxs-lookup"><span data-stu-id="f46e4-114">Type</span></span>                      | <span data-ttu-id="f46e4-115">说明</span><span class="sxs-lookup"><span data-stu-id="f46e4-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="f46e4-116">name</span><span class="sxs-lookup"><span data-stu-id="f46e4-116">name</span></span>                        |<span data-ttu-id="f46e4-117">String</span><span class="sxs-lookup"><span data-stu-id="f46e4-117">String</span></span>                    |<span data-ttu-id="f46e4-118">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="f46e4-118">Operator name.</span></span> |
|<span data-ttu-id="f46e4-119">parameters</span><span class="sxs-lookup"><span data-stu-id="f46e4-119">parameters</span></span>                  |<span data-ttu-id="f46e4-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="f46e4-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="f46e4-121">函数参数的集合。</span><span class="sxs-lookup"><span data-stu-id="f46e4-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f46e4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f46e4-122">JSON representation</span></span>

<span data-ttu-id="f46e4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f46e4-123">The following is a JSON representation of the resource.</span></span>

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
