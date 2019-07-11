---
title: attributeMappingFunctionSchema 资源类型
description: 介绍可在属性映射中用于在同步期间转换值的函数。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2290f2c3140d9c955dc3a3d4bc72f9b953a7775f
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620281"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="f5e48-103">attributeMappingFunctionSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5e48-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5e48-104">介绍可在[属性映射](synchronization-attributemapping.md)中用于在同步期间转换值的函数。</span><span class="sxs-lookup"><span data-stu-id="f5e48-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="f5e48-105">方法</span><span class="sxs-lookup"><span data-stu-id="f5e48-105">Methods</span></span>

| <span data-ttu-id="f5e48-106">方法</span><span class="sxs-lookup"><span data-stu-id="f5e48-106">Method</span></span>           | <span data-ttu-id="f5e48-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5e48-107">Return Type</span></span>    |<span data-ttu-id="f5e48-108">说明</span><span class="sxs-lookup"><span data-stu-id="f5e48-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5e48-109">List</span><span class="sxs-lookup"><span data-stu-id="f5e48-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="f5e48-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="f5e48-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="f5e48-111">列出受支持的属性映射函数。</span><span class="sxs-lookup"><span data-stu-id="f5e48-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5e48-112">属性</span><span class="sxs-lookup"><span data-stu-id="f5e48-112">Properties</span></span>

| <span data-ttu-id="f5e48-113">属性</span><span class="sxs-lookup"><span data-stu-id="f5e48-113">Property</span></span>                   | <span data-ttu-id="f5e48-114">类型</span><span class="sxs-lookup"><span data-stu-id="f5e48-114">Type</span></span>                      | <span data-ttu-id="f5e48-115">说明</span><span class="sxs-lookup"><span data-stu-id="f5e48-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="f5e48-116">name</span><span class="sxs-lookup"><span data-stu-id="f5e48-116">name</span></span>                        |<span data-ttu-id="f5e48-117">String</span><span class="sxs-lookup"><span data-stu-id="f5e48-117">String</span></span>                    |<span data-ttu-id="f5e48-118">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="f5e48-118">Operator name.</span></span> |
|<span data-ttu-id="f5e48-119">parameters</span><span class="sxs-lookup"><span data-stu-id="f5e48-119">parameters</span></span>                  |<span data-ttu-id="f5e48-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="f5e48-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="f5e48-121">函数参数的集合。</span><span class="sxs-lookup"><span data-stu-id="f5e48-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5e48-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5e48-122">JSON representation</span></span>

<span data-ttu-id="f5e48-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5e48-123">The following is a JSON representation of the resource.</span></span>

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
