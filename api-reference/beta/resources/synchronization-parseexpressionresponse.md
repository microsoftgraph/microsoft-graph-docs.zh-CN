---
title: parseExpressionResponse 资源类型
description: '表示来自[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作的响应。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d63a8834640d357e41051750f7f2cd50b8724fee
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620484"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="e3158-103">parseExpressionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3158-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3158-104">表示来自[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作的响应。</span><span class="sxs-lookup"><span data-stu-id="e3158-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="e3158-105">属性</span><span class="sxs-lookup"><span data-stu-id="e3158-105">Properties</span></span>
| <span data-ttu-id="e3158-106">属性</span><span class="sxs-lookup"><span data-stu-id="e3158-106">Property</span></span>     | <span data-ttu-id="e3158-107">类型</span><span class="sxs-lookup"><span data-stu-id="e3158-107">Type</span></span>   |<span data-ttu-id="e3158-108">说明</span><span class="sxs-lookup"><span data-stu-id="e3158-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3158-109">error</span><span class="sxs-lookup"><span data-stu-id="e3158-109">error</span></span>|<span data-ttu-id="e3158-110">publicError</span><span class="sxs-lookup"><span data-stu-id="e3158-110">publicError</span></span>|<span data-ttu-id="e3158-111">如果表达式求值导致错误, 则为错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="e3158-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="e3158-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="e3158-112">evaluationResult</span></span>|<span data-ttu-id="e3158-113">String collection</span><span class="sxs-lookup"><span data-stu-id="e3158-113">String collection</span></span>|<span data-ttu-id="e3158-114">由表达式的计算产生的值的集合。</span><span class="sxs-lookup"><span data-stu-id="e3158-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="e3158-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="e3158-115">evaluationSucceeded</span></span>|<span data-ttu-id="e3158-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3158-116">Boolean</span></span>|<span data-ttu-id="e3158-117">`true`如果评估成功。</span><span class="sxs-lookup"><span data-stu-id="e3158-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="e3158-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="e3158-118">parsedExpression</span></span>|[<span data-ttu-id="e3158-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e3158-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="e3158-120">一个代表已分析的表达式的[attributeMappingSource](synchronization-attributemappingsource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3158-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="e3158-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="e3158-121">parsingSucceeded</span></span>|<span data-ttu-id="e3158-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3158-122">Boolean</span></span>|<span data-ttu-id="e3158-123">`true`如果表达式已成功分析。</span><span class="sxs-lookup"><span data-stu-id="e3158-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3158-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3158-124">JSON representation</span></span>

<span data-ttu-id="e3158-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3158-125">The following is a JSON representation of the resource.</span></span>

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
