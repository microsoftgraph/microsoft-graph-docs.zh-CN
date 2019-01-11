---
title: parseExpressionResponse 资源类型
description: '代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832947"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="cb7f5-103">parseExpressionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb7f5-103">parseExpressionResponse resource type</span></span>

> <span data-ttu-id="cb7f5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb7f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb7f5-106">代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-106">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="cb7f5-107">属性</span><span class="sxs-lookup"><span data-stu-id="cb7f5-107">Properties</span></span>
| <span data-ttu-id="cb7f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="cb7f5-108">Property</span></span>     | <span data-ttu-id="cb7f5-109">类型</span><span class="sxs-lookup"><span data-stu-id="cb7f5-109">Type</span></span>   |<span data-ttu-id="cb7f5-110">Description</span><span class="sxs-lookup"><span data-stu-id="cb7f5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb7f5-111">error</span><span class="sxs-lookup"><span data-stu-id="cb7f5-111">error</span></span>|<span data-ttu-id="cb7f5-112">odata.error</span><span class="sxs-lookup"><span data-stu-id="cb7f5-112">odata.error</span></span>|<span data-ttu-id="cb7f5-113">错误详细信息，如果表达式评估导致出错。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-113">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="cb7f5-114">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="cb7f5-114">evaluationResult</span></span>|<span data-ttu-id="cb7f5-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="cb7f5-115">String collection</span></span>|<span data-ttu-id="cb7f5-116">无条件表达式的计算值的集合。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-116">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="cb7f5-117">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="cb7f5-117">evaluationSucceeded</span></span>|<span data-ttu-id="cb7f5-118">布尔</span><span class="sxs-lookup"><span data-stu-id="cb7f5-118">Boolean</span></span>|<span data-ttu-id="cb7f5-119">`true`评估是否成功。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-119">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="cb7f5-120">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="cb7f5-120">parsedExpression</span></span>|[<span data-ttu-id="cb7f5-121">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="cb7f5-121">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="cb7f5-122">一个表示已分析的表达式[attributeMappingSource](synchronization-attributemappingsource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-122">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="cb7f5-123">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="cb7f5-123">parsingSucceeded</span></span>|<span data-ttu-id="cb7f5-124">布尔</span><span class="sxs-lookup"><span data-stu-id="cb7f5-124">Boolean</span></span>|<span data-ttu-id="cb7f5-125">`true`如果成功解析的表达式。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-125">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb7f5-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb7f5-126">JSON representation</span></span>

<span data-ttu-id="cb7f5-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
