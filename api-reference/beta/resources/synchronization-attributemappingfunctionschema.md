---
title: attributeMappingFunctionSchema 资源类型
description: 介绍可在属性映射中用于在同步期间转换值的函数。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 195f8e11737d2f9ae48675cdb7a7046869090e19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520245"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="f0512-103">attributeMappingFunctionSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0512-103">attributeMappingFunctionSchema resource type</span></span>

<span data-ttu-id="f0512-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0512-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0512-105">介绍可在[属性映射](synchronization-attributemapping.md)中用于在同步期间转换值的函数。</span><span class="sxs-lookup"><span data-stu-id="f0512-105">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="f0512-106">方法</span><span class="sxs-lookup"><span data-stu-id="f0512-106">Methods</span></span>

| <span data-ttu-id="f0512-107">方法</span><span class="sxs-lookup"><span data-stu-id="f0512-107">Method</span></span>           | <span data-ttu-id="f0512-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f0512-108">Return Type</span></span>    |<span data-ttu-id="f0512-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0512-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0512-110">List</span><span class="sxs-lookup"><span data-stu-id="f0512-110">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="f0512-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0512-111">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="f0512-112">列出受支持的属性映射函数。</span><span class="sxs-lookup"><span data-stu-id="f0512-112">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0512-113">属性</span><span class="sxs-lookup"><span data-stu-id="f0512-113">Properties</span></span>

| <span data-ttu-id="f0512-114">属性</span><span class="sxs-lookup"><span data-stu-id="f0512-114">Property</span></span>                   | <span data-ttu-id="f0512-115">类型</span><span class="sxs-lookup"><span data-stu-id="f0512-115">Type</span></span>                      | <span data-ttu-id="f0512-116">说明</span><span class="sxs-lookup"><span data-stu-id="f0512-116">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="f0512-117">name</span><span class="sxs-lookup"><span data-stu-id="f0512-117">name</span></span>                        |<span data-ttu-id="f0512-118">String</span><span class="sxs-lookup"><span data-stu-id="f0512-118">String</span></span>                    |<span data-ttu-id="f0512-119">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="f0512-119">Operator name.</span></span> |
|<span data-ttu-id="f0512-120">parameters</span><span class="sxs-lookup"><span data-stu-id="f0512-120">parameters</span></span>                  |<span data-ttu-id="f0512-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0512-121">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="f0512-122">函数参数的集合。</span><span class="sxs-lookup"><span data-stu-id="f0512-122">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0512-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0512-123">JSON representation</span></span>

<span data-ttu-id="f0512-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0512-124">The following is a JSON representation of the resource.</span></span>

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
