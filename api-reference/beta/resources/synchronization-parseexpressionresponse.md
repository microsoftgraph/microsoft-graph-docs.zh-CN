---
title: parseExpressionResponse 资源类型
description: '代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641055"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="0d66d-103">parseExpressionResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d66d-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d66d-104">代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。</span><span class="sxs-lookup"><span data-stu-id="0d66d-104">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="0d66d-105">属性</span><span class="sxs-lookup"><span data-stu-id="0d66d-105">Properties</span></span>
| <span data-ttu-id="0d66d-106">属性</span><span class="sxs-lookup"><span data-stu-id="0d66d-106">Property</span></span>     | <span data-ttu-id="0d66d-107">类型</span><span class="sxs-lookup"><span data-stu-id="0d66d-107">Type</span></span>   |<span data-ttu-id="0d66d-108">说明</span><span class="sxs-lookup"><span data-stu-id="0d66d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d66d-109">error</span><span class="sxs-lookup"><span data-stu-id="0d66d-109">error</span></span>|<span data-ttu-id="0d66d-110">odata.error</span><span class="sxs-lookup"><span data-stu-id="0d66d-110">odata.error</span></span>|<span data-ttu-id="0d66d-111">错误详细信息，如果表达式评估导致出错。</span><span class="sxs-lookup"><span data-stu-id="0d66d-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="0d66d-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="0d66d-112">evaluationResult</span></span>|<span data-ttu-id="0d66d-113">String collection</span><span class="sxs-lookup"><span data-stu-id="0d66d-113">String collection</span></span>|<span data-ttu-id="0d66d-114">无条件表达式的计算值的集合。</span><span class="sxs-lookup"><span data-stu-id="0d66d-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="0d66d-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="0d66d-115">evaluationSucceeded</span></span>|<span data-ttu-id="0d66d-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="0d66d-116">Boolean</span></span>|<span data-ttu-id="0d66d-117">`true`评估是否成功。</span><span class="sxs-lookup"><span data-stu-id="0d66d-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="0d66d-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="0d66d-118">parsedExpression</span></span>|[<span data-ttu-id="0d66d-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="0d66d-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="0d66d-120">一个表示已分析的表达式[attributeMappingSource](synchronization-attributemappingsource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d66d-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="0d66d-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="0d66d-121">parsingSucceeded</span></span>|<span data-ttu-id="0d66d-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="0d66d-122">Boolean</span></span>|<span data-ttu-id="0d66d-123">`true`如果成功解析的表达式。</span><span class="sxs-lookup"><span data-stu-id="0d66d-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d66d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d66d-124">JSON representation</span></span>

<span data-ttu-id="0d66d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d66d-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
