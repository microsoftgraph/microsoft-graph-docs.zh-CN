---
title: filterOperand 资源类型
description: 包含操作数的值的集合。
localization_priority: Normal
ms.openlocfilehash: ab62477889cc92954ed308c508e18a638cd59375
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581805"
---
# <a name="filteroperand-resource-type"></a><span data-ttu-id="0d0f3-103">filterOperand 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d0f3-103">filterOperand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d0f3-104">包含操作数的值的集合。</span><span class="sxs-lookup"><span data-stu-id="0d0f3-104">Contains a collection of values for the operand.</span></span>

## <a name="properties"></a><span data-ttu-id="0d0f3-105">属性</span><span class="sxs-lookup"><span data-stu-id="0d0f3-105">Properties</span></span>
| <span data-ttu-id="0d0f3-106">属性</span><span class="sxs-lookup"><span data-stu-id="0d0f3-106">Property</span></span>     | <span data-ttu-id="0d0f3-107">类型</span><span class="sxs-lookup"><span data-stu-id="0d0f3-107">Type</span></span>   |<span data-ttu-id="0d0f3-108">说明</span><span class="sxs-lookup"><span data-stu-id="0d0f3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d0f3-109">值</span><span class="sxs-lookup"><span data-stu-id="0d0f3-109">values</span></span>|<span data-ttu-id="0d0f3-110">String collection</span><span class="sxs-lookup"><span data-stu-id="0d0f3-110">String collection</span></span>|<span data-ttu-id="0d0f3-111">值的集合。</span><span class="sxs-lookup"><span data-stu-id="0d0f3-111">Collection of values.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d0f3-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d0f3-112">JSON representation</span></span>

<span data-ttu-id="0d0f3-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d0f3-113">The following is a JSON representation of the resource.</span></span>

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
