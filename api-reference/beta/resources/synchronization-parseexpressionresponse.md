---
title: parseExpressionResponse 资源类型
description: 表示 synchronizationSchema： parseExpression 操作的响应。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: e564cb2ad7a80c91fec7d6298254fa19bde4537c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133145"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="e063b-103">parseExpressionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="e063b-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="e063b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e063b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e063b-105">表示 [parseExpression 操作的响应](../api/synchronization-synchronizationschema-parseexpression.md) 。</span><span class="sxs-lookup"><span data-stu-id="e063b-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="e063b-106">属性</span><span class="sxs-lookup"><span data-stu-id="e063b-106">Properties</span></span>
| <span data-ttu-id="e063b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e063b-107">Property</span></span>     | <span data-ttu-id="e063b-108">类型</span><span class="sxs-lookup"><span data-stu-id="e063b-108">Type</span></span>   |<span data-ttu-id="e063b-109">说明</span><span class="sxs-lookup"><span data-stu-id="e063b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e063b-110">error</span><span class="sxs-lookup"><span data-stu-id="e063b-110">error</span></span>|<span data-ttu-id="e063b-111">publicError</span><span class="sxs-lookup"><span data-stu-id="e063b-111">publicError</span></span>|<span data-ttu-id="e063b-112">如果表达式计算导致错误，错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="e063b-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="e063b-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="e063b-113">evaluationResult</span></span>|<span data-ttu-id="e063b-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e063b-114">String collection</span></span>|<span data-ttu-id="e063b-115">由表达式的计算生成的值集合。</span><span class="sxs-lookup"><span data-stu-id="e063b-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="e063b-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="e063b-116">evaluationSucceeded</span></span>|<span data-ttu-id="e063b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e063b-117">Boolean</span></span>|<span data-ttu-id="e063b-118">`true` 评估是否成功。</span><span class="sxs-lookup"><span data-stu-id="e063b-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="e063b-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="e063b-119">parsedExpression</span></span>|[<span data-ttu-id="e063b-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e063b-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="e063b-121">一个代表已分析表达式的 [attributeMappingSource](synchronization-attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e063b-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="e063b-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="e063b-122">parsingSucceeded</span></span>|<span data-ttu-id="e063b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e063b-123">Boolean</span></span>|<span data-ttu-id="e063b-124">`true` 是否成功分析表达式。</span><span class="sxs-lookup"><span data-stu-id="e063b-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e063b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e063b-125">JSON representation</span></span>

<span data-ttu-id="e063b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e063b-126">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


