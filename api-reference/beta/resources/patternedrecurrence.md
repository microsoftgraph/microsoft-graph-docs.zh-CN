---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
ms.openlocfilehash: f4ffd62b54eb6d577269b36d0ee3bea0a3a0002c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568261"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="5af98-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="5af98-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5af98-104">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="5af98-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="5af98-105">属性</span><span class="sxs-lookup"><span data-stu-id="5af98-105">Properties</span></span>
| <span data-ttu-id="5af98-106">属性</span><span class="sxs-lookup"><span data-stu-id="5af98-106">Property</span></span>     | <span data-ttu-id="5af98-107">类型</span><span class="sxs-lookup"><span data-stu-id="5af98-107">Type</span></span>   |<span data-ttu-id="5af98-108">说明</span><span class="sxs-lookup"><span data-stu-id="5af98-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5af98-109">模式</span><span class="sxs-lookup"><span data-stu-id="5af98-109">pattern</span></span>|[<span data-ttu-id="5af98-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="5af98-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="5af98-111">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="5af98-111">The frequency of an event.</span></span>|
|<span data-ttu-id="5af98-112">区域</span><span class="sxs-lookup"><span data-stu-id="5af98-112">range</span></span>|[<span data-ttu-id="5af98-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="5af98-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="5af98-114">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="5af98-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5af98-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5af98-115">JSON representation</span></span>

<span data-ttu-id="5af98-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5af98-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patternedrecurrence.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
