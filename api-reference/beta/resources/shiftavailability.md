---
title: shiftAvailability 资源类型
description: 用户计划的工作及其定期模式的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8e06b64bc01be163149468c9090df2a8ea59497d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520623"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="76c71-103">shiftAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="76c71-103">shiftAvailability resource type</span></span>

<span data-ttu-id="76c71-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="76c71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c71-105">要安排的用户在[班次](shift.md)和定期模式中的可用性。</span><span class="sxs-lookup"><span data-stu-id="76c71-105">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="76c71-106">属性</span><span class="sxs-lookup"><span data-stu-id="76c71-106">Properties</span></span>

| <span data-ttu-id="76c71-107">属性</span><span class="sxs-lookup"><span data-stu-id="76c71-107">Property</span></span>     | <span data-ttu-id="76c71-108">类型</span><span class="sxs-lookup"><span data-stu-id="76c71-108">Type</span></span>        | <span data-ttu-id="76c71-109">说明</span><span class="sxs-lookup"><span data-stu-id="76c71-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76c71-110">recurrence</span><span class="sxs-lookup"><span data-stu-id="76c71-110">recurrence</span></span>|[<span data-ttu-id="76c71-111">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="76c71-111">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="76c71-112">指定定期模式</span><span class="sxs-lookup"><span data-stu-id="76c71-112">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="76c71-113">因此</span><span class="sxs-lookup"><span data-stu-id="76c71-113">timeSlots</span></span>|<span data-ttu-id="76c71-114">[timeRange](timerange.md)集合</span><span class="sxs-lookup"><span data-stu-id="76c71-114">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="76c71-115">用户首选的时隙（s）。</span><span class="sxs-lookup"><span data-stu-id="76c71-115">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="76c71-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="76c71-116">timeZone</span></span>|<span data-ttu-id="76c71-117">String</span><span class="sxs-lookup"><span data-stu-id="76c71-117">String</span></span>|<span data-ttu-id="76c71-118">指定所指定时间的时区。</span><span class="sxs-lookup"><span data-stu-id="76c71-118">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76c71-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76c71-119">JSON representation</span></span>

<span data-ttu-id="76c71-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76c71-120">The following is a JSON representation of the resource.</span></span>

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
