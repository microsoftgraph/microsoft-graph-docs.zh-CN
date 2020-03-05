---
title: parseExpressionResponse 资源类型
description: 表示来自[synchronizationSchema： parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作的响应。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c752d5c021418dd4a3154a539a61c6ab3bae8a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520133"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="bf2a7-103">parseExpressionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf2a7-103">parseExpressionResponse resource type</span></span>

<span data-ttu-id="bf2a7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bf2a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf2a7-105">表示来自[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作的响应。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-105">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="bf2a7-106">属性</span><span class="sxs-lookup"><span data-stu-id="bf2a7-106">Properties</span></span>
| <span data-ttu-id="bf2a7-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf2a7-107">Property</span></span>     | <span data-ttu-id="bf2a7-108">类型</span><span class="sxs-lookup"><span data-stu-id="bf2a7-108">Type</span></span>   |<span data-ttu-id="bf2a7-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf2a7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2a7-110">error</span><span class="sxs-lookup"><span data-stu-id="bf2a7-110">error</span></span>|<span data-ttu-id="bf2a7-111">publicError</span><span class="sxs-lookup"><span data-stu-id="bf2a7-111">publicError</span></span>|<span data-ttu-id="bf2a7-112">如果表达式求值导致错误，则为错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-112">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="bf2a7-113">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="bf2a7-113">evaluationResult</span></span>|<span data-ttu-id="bf2a7-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="bf2a7-114">String collection</span></span>|<span data-ttu-id="bf2a7-115">由表达式的计算产生的值的集合。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-115">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="bf2a7-116">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="bf2a7-116">evaluationSucceeded</span></span>|<span data-ttu-id="bf2a7-117">布尔</span><span class="sxs-lookup"><span data-stu-id="bf2a7-117">Boolean</span></span>|<span data-ttu-id="bf2a7-118">`true`如果评估成功。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-118">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="bf2a7-119">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="bf2a7-119">parsedExpression</span></span>|[<span data-ttu-id="bf2a7-120">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="bf2a7-120">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="bf2a7-121">一个代表已分析的表达式的[attributeMappingSource](synchronization-attributemappingsource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-121">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="bf2a7-122">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="bf2a7-122">parsingSucceeded</span></span>|<span data-ttu-id="bf2a7-123">布尔</span><span class="sxs-lookup"><span data-stu-id="bf2a7-123">Boolean</span></span>|<span data-ttu-id="bf2a7-124">`true`如果表达式已成功分析。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-124">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf2a7-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf2a7-125">JSON representation</span></span>

<span data-ttu-id="bf2a7-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf2a7-126">The following is a JSON representation of the resource.</span></span>

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
