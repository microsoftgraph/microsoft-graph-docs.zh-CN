---
title: shiftAvailability 资源类型
description: 用户计划的工作及其定期模式的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86ad11ae32977ac07a7755ebe0a169686f6f605e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058051"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="9c31e-103">shiftAvailability 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c31e-103">shiftAvailability resource type</span></span>

<span data-ttu-id="9c31e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c31e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c31e-105">要安排的用户在 [班次](shift.md) 和定期模式中的可用性。</span><span class="sxs-lookup"><span data-stu-id="9c31e-105">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="9c31e-106">属性</span><span class="sxs-lookup"><span data-stu-id="9c31e-106">Properties</span></span>

| <span data-ttu-id="9c31e-107">属性</span><span class="sxs-lookup"><span data-stu-id="9c31e-107">Property</span></span>     | <span data-ttu-id="9c31e-108">类型</span><span class="sxs-lookup"><span data-stu-id="9c31e-108">Type</span></span>        | <span data-ttu-id="9c31e-109">说明</span><span class="sxs-lookup"><span data-stu-id="9c31e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c31e-110">recurrence</span><span class="sxs-lookup"><span data-stu-id="9c31e-110">recurrence</span></span>|[<span data-ttu-id="9c31e-111">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9c31e-111">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="9c31e-112">指定定期模式</span><span class="sxs-lookup"><span data-stu-id="9c31e-112">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="9c31e-113">因此</span><span class="sxs-lookup"><span data-stu-id="9c31e-113">timeSlots</span></span>|<span data-ttu-id="9c31e-114">[timeRange](timerange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c31e-114">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="9c31e-115">用户首选)  (s 的时间段。</span><span class="sxs-lookup"><span data-stu-id="9c31e-115">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="9c31e-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="9c31e-116">timeZone</span></span>|<span data-ttu-id="9c31e-117">String</span><span class="sxs-lookup"><span data-stu-id="9c31e-117">String</span></span>|<span data-ttu-id="9c31e-118">指定所指定时间的时区。</span><span class="sxs-lookup"><span data-stu-id="9c31e-118">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9c31e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c31e-119">JSON representation</span></span>

<span data-ttu-id="9c31e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c31e-120">The following is a JSON representation of the resource.</span></span>

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


