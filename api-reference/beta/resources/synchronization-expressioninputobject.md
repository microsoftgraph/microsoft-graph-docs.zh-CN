---
title: expressionInputObject 资源类型
description: '代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641650"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="b6065-103">expressionInputObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6065-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6065-104">代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。</span><span class="sxs-lookup"><span data-stu-id="b6065-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="b6065-105">属性</span><span class="sxs-lookup"><span data-stu-id="b6065-105">Properties</span></span>
| <span data-ttu-id="b6065-106">属性</span><span class="sxs-lookup"><span data-stu-id="b6065-106">Property</span></span>     | <span data-ttu-id="b6065-107">类型</span><span class="sxs-lookup"><span data-stu-id="b6065-107">Type</span></span>   |<span data-ttu-id="b6065-108">说明</span><span class="sxs-lookup"><span data-stu-id="b6065-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6065-109">definition</span><span class="sxs-lookup"><span data-stu-id="b6065-109">definition</span></span>|[<span data-ttu-id="b6065-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="b6065-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="b6065-111">测试对象的定义。</span><span class="sxs-lookup"><span data-stu-id="b6065-111">Definition of the test object.</span></span>|
|<span data-ttu-id="b6065-112">properties</span><span class="sxs-lookup"><span data-stu-id="b6065-112">properties</span></span>|<span data-ttu-id="b6065-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6065-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="b6065-114">测试对象的属性值。</span><span class="sxs-lookup"><span data-stu-id="b6065-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6065-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6065-115">JSON representation</span></span>

<span data-ttu-id="b6065-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6065-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
