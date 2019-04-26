---
title: patternedRecurrence 资源类型
description: 定期模式和区域。
localization_priority: Normal
ms.openlocfilehash: 063df70dfeeb1d37cfc5e23710108dd4cfc9ae57
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344921"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="38eb6-103">patternedRecurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="38eb6-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38eb6-104">定期模式和区域。</span><span class="sxs-lookup"><span data-stu-id="38eb6-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="38eb6-105">属性</span><span class="sxs-lookup"><span data-stu-id="38eb6-105">Properties</span></span>
| <span data-ttu-id="38eb6-106">属性</span><span class="sxs-lookup"><span data-stu-id="38eb6-106">Property</span></span>     | <span data-ttu-id="38eb6-107">类型</span><span class="sxs-lookup"><span data-stu-id="38eb6-107">Type</span></span>   |<span data-ttu-id="38eb6-108">说明</span><span class="sxs-lookup"><span data-stu-id="38eb6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38eb6-109">模式</span><span class="sxs-lookup"><span data-stu-id="38eb6-109">pattern</span></span>|[<span data-ttu-id="38eb6-110">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="38eb6-110">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="38eb6-111">事件发生的频率。</span><span class="sxs-lookup"><span data-stu-id="38eb6-111">The frequency of an event.</span></span>|
|<span data-ttu-id="38eb6-112">区域</span><span class="sxs-lookup"><span data-stu-id="38eb6-112">range</span></span>|[<span data-ttu-id="38eb6-113">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="38eb6-113">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="38eb6-114">事件的持续时间。</span><span class="sxs-lookup"><span data-stu-id="38eb6-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38eb6-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38eb6-115">JSON representation</span></span>

<span data-ttu-id="38eb6-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38eb6-116">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
