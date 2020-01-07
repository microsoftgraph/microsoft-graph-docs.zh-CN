---
title: shiftAvailability 资源类型
description: 用户计划的工作及其定期模式的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a284774b76774da0420322f0cd2e092aec6ce83
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952284"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="a0058-103">shiftAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0058-103">shiftAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0058-104">要安排的用户在[班次](shift.md)和定期模式中的可用性。</span><span class="sxs-lookup"><span data-stu-id="a0058-104">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="a0058-105">属性</span><span class="sxs-lookup"><span data-stu-id="a0058-105">Properties</span></span>

| <span data-ttu-id="a0058-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0058-106">Property</span></span>     | <span data-ttu-id="a0058-107">类型</span><span class="sxs-lookup"><span data-stu-id="a0058-107">Type</span></span>        | <span data-ttu-id="a0058-108">Description</span><span class="sxs-lookup"><span data-stu-id="a0058-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0058-109">recurrence</span><span class="sxs-lookup"><span data-stu-id="a0058-109">recurrence</span></span>|[<span data-ttu-id="a0058-110">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a0058-110">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="a0058-111">指定定期模式</span><span class="sxs-lookup"><span data-stu-id="a0058-111">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="a0058-112">因此</span><span class="sxs-lookup"><span data-stu-id="a0058-112">timeSlots</span></span>|<span data-ttu-id="a0058-113">[timeRange](timerange.md)集合</span><span class="sxs-lookup"><span data-stu-id="a0058-113">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="a0058-114">用户首选的时隙（s）。</span><span class="sxs-lookup"><span data-stu-id="a0058-114">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="a0058-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="a0058-115">timeZone</span></span>|<span data-ttu-id="a0058-116">String</span><span class="sxs-lookup"><span data-stu-id="a0058-116">String</span></span>|<span data-ttu-id="a0058-117">指定所指定时间的时区。</span><span class="sxs-lookup"><span data-stu-id="a0058-117">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0058-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0058-118">JSON representation</span></span>

<span data-ttu-id="a0058-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0058-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
