---
title: parseExpressionResponse 资源类型
description: 表示来自 synchronizationSchema： parseExpression 操作的响应。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ef96bda8e9e28c655c4bbcf0153ea83ef5b0c8e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217603"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="37321-103">parseExpressionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="37321-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="37321-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37321-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37321-105">表示来自[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作的响应。</span><span class="sxs-lookup"><span data-stu-id="37321-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="37321-106">属性</span><span class="sxs-lookup"><span data-stu-id="37321-106">Properties</span></span>
| <span data-ttu-id="37321-107">属性</span><span class="sxs-lookup"><span data-stu-id="37321-107">Property</span></span>     | <span data-ttu-id="37321-108">类型</span><span class="sxs-lookup"><span data-stu-id="37321-108">Type</span></span>   |<span data-ttu-id="37321-109">说明</span><span class="sxs-lookup"><span data-stu-id="37321-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37321-110">error</span><span class="sxs-lookup"><span data-stu-id="37321-110">error</span></span>|<span data-ttu-id="37321-111">publicError</span><span class="sxs-lookup"><span data-stu-id="37321-111">publicError</span></span>|<span data-ttu-id="37321-112">如果表达式求值导致错误，则为错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="37321-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="37321-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="37321-113">evaluationResult</span></span>|<span data-ttu-id="37321-114">String collection</span><span class="sxs-lookup"><span data-stu-id="37321-114">String collection</span></span>|<span data-ttu-id="37321-115">由表达式的计算产生的值的集合。</span><span class="sxs-lookup"><span data-stu-id="37321-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="37321-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="37321-116">evaluationSucceeded</span></span>|<span data-ttu-id="37321-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="37321-117">Boolean</span></span>|<span data-ttu-id="37321-118">`true`如果评估成功。</span><span class="sxs-lookup"><span data-stu-id="37321-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="37321-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="37321-119">parsedExpression</span></span>|[<span data-ttu-id="37321-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="37321-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="37321-121">一个代表已分析的表达式的[attributeMappingSource](synchronization-attributemappingsource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="37321-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="37321-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="37321-122">parsingSucceeded</span></span>|<span data-ttu-id="37321-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="37321-123">Boolean</span></span>|<span data-ttu-id="37321-124">`true`如果表达式已成功分析。</span><span class="sxs-lookup"><span data-stu-id="37321-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37321-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37321-125">JSON representation</span></span>

<span data-ttu-id="37321-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37321-126">The following is a JSON representation of the resource.</span></span>

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
