---
title: filterOperand 资源类型
description: 包含的操作数值的集合。
localization_priority: Normal
ms.openlocfilehash: ab62477889cc92954ed308c508e18a638cd59375
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515375"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="9785b-103">filterOperand 资源类型</span><span class="sxs-lookup"><span data-stu-id="9785b-103">filterOperand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9785b-104">包含的操作数值的集合。</span><span class="sxs-lookup"><span data-stu-id="9785b-104">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="9785b-105">属性</span><span class="sxs-lookup"><span data-stu-id="9785b-105">Properties</span></span>
| <span data-ttu-id="9785b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9785b-106">Property</span></span>     | <span data-ttu-id="9785b-107">类型</span><span class="sxs-lookup"><span data-stu-id="9785b-107">Type</span></span>   |<span data-ttu-id="9785b-108">说明</span><span class="sxs-lookup"><span data-stu-id="9785b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9785b-109">values</span><span class="sxs-lookup"><span data-stu-id="9785b-109">values</span></span>|<span data-ttu-id="9785b-110">String 集合</span><span class="sxs-lookup"><span data-stu-id="9785b-110">String collection</span></span>|<span data-ttu-id="9785b-111">值的集合。</span><span class="sxs-lookup"><span data-stu-id="9785b-111">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9785b-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9785b-112">JSON representation</span></span>

<span data-ttu-id="9785b-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9785b-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperand"
}-->

```json
{
  "values": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
