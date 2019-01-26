---
title: expressionInputObject 资源类型
description: '代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。'
localization_priority: Normal
ms.openlocfilehash: 4f0ba06651fdd8a296b0939d05ecefe996f0089f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570958"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="2ea03-103">expressionInputObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ea03-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ea03-104">代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作执行表达式求值。</span><span class="sxs-lookup"><span data-stu-id="2ea03-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="2ea03-105">属性</span><span class="sxs-lookup"><span data-stu-id="2ea03-105">Properties</span></span>
| <span data-ttu-id="2ea03-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ea03-106">Property</span></span>     | <span data-ttu-id="2ea03-107">类型</span><span class="sxs-lookup"><span data-stu-id="2ea03-107">Type</span></span>   |<span data-ttu-id="2ea03-108">说明</span><span class="sxs-lookup"><span data-stu-id="2ea03-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ea03-109">definition</span><span class="sxs-lookup"><span data-stu-id="2ea03-109">definition</span></span>|[<span data-ttu-id="2ea03-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="2ea03-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="2ea03-111">测试对象的定义。</span><span class="sxs-lookup"><span data-stu-id="2ea03-111">Definition of the test object.</span></span>|
|<span data-ttu-id="2ea03-112">properties</span><span class="sxs-lookup"><span data-stu-id="2ea03-112">properties</span></span>|<span data-ttu-id="2ea03-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="2ea03-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="2ea03-114">测试对象的属性值。</span><span class="sxs-lookup"><span data-stu-id="2ea03-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ea03-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ea03-115">JSON representation</span></span>

<span data-ttu-id="2ea03-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ea03-116">The following is a JSON representation of the resource.</span></span>

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
