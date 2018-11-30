---
title: attributeMappingFunctionSchema 资源类型
description: 介绍可用于中的属性映射同步过程中转换值的函数。
ms.openlocfilehash: 9760669bb29700bfa79c1cd375857b4fd673879b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045374"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="b3750-103">attributeMappingFunctionSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3750-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="b3750-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3750-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3750-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3750-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3750-106">介绍可在[属性映射](synchronization-attributemapping.md)用于同步过程中转换值的函数。</span><span class="sxs-lookup"><span data-stu-id="b3750-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="b3750-107">方法</span><span class="sxs-lookup"><span data-stu-id="b3750-107">Methods</span></span>

| <span data-ttu-id="b3750-108">方法</span><span class="sxs-lookup"><span data-stu-id="b3750-108">Method</span></span>           | <span data-ttu-id="b3750-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3750-109">Return Type</span></span>    |<span data-ttu-id="b3750-110">说明</span><span class="sxs-lookup"><span data-stu-id="b3750-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3750-111">List</span><span class="sxs-lookup"><span data-stu-id="b3750-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="b3750-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3750-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="b3750-113">支持列表属性的映射功能。</span><span class="sxs-lookup"><span data-stu-id="b3750-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3750-114">属性</span><span class="sxs-lookup"><span data-stu-id="b3750-114">Properties</span></span>

| <span data-ttu-id="b3750-115">属性</span><span class="sxs-lookup"><span data-stu-id="b3750-115">Property</span></span>                   | <span data-ttu-id="b3750-116">类型</span><span class="sxs-lookup"><span data-stu-id="b3750-116">Type</span></span>                      | <span data-ttu-id="b3750-117">说明</span><span class="sxs-lookup"><span data-stu-id="b3750-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="b3750-118">name</span><span class="sxs-lookup"><span data-stu-id="b3750-118">name</span></span>                        |<span data-ttu-id="b3750-119">字符串</span><span class="sxs-lookup"><span data-stu-id="b3750-119">String</span></span>                    |<span data-ttu-id="b3750-120">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="b3750-120">Operator name.</span></span> |
|<span data-ttu-id="b3750-121">parameters</span><span class="sxs-lookup"><span data-stu-id="b3750-121">parameters</span></span>                  |<span data-ttu-id="b3750-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3750-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="b3750-123">函数参数的集合。</span><span class="sxs-lookup"><span data-stu-id="b3750-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3750-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3750-124">JSON representation</span></span>

<span data-ttu-id="b3750-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3750-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->