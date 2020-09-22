---
title: timeConstraint 资源类型
description: 根据指定的活动和打开时间段的性质，将会议时间建议限制在一周的特定时间和几天。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4cd26445864ab68bc83ef8d67495897e7244e48f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090849"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="3f3e5-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f3e5-103">timeConstraint resource type</span></span>

<span data-ttu-id="3f3e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f3e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f3e5-105">根据指定的活动和打开时间段的性质，将会议时间建议限制在一周的特定时间和几天。</span><span class="sxs-lookup"><span data-stu-id="3f3e5-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f3e5-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f3e5-106">JSON representation</span></span>

<span data-ttu-id="3f3e5-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f3e5-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="3f3e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="3f3e5-108">Properties</span></span>
| <span data-ttu-id="3f3e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="3f3e5-109">Property</span></span>     | <span data-ttu-id="3f3e5-110">类型</span><span class="sxs-lookup"><span data-stu-id="3f3e5-110">Type</span></span>   |<span data-ttu-id="3f3e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="3f3e5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f3e5-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="3f3e5-112">activityDomain</span></span>|<span data-ttu-id="3f3e5-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="3f3e5-113">activityDomain</span></span>|<span data-ttu-id="3f3e5-114">（可选）会议性质。</span><span class="sxs-lookup"><span data-stu-id="3f3e5-114">The nature of the activity, optional.</span></span> <span data-ttu-id="3f3e5-115">可能的值是： `work` 、 `personal` 、 `unrestricted` 或 `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="3f3e5-115">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="3f3e5-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="3f3e5-116">timeslots</span></span>|<span data-ttu-id="3f3e5-117">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f3e5-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="3f3e5-118">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="3f3e5-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

