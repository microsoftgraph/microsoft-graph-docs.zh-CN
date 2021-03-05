---
title: timeConstraint 资源类型
description: 根据指定的活动和开放时间段的性质，将会议时间建议限制为一周中的特定时段和天。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d79fc1630522c30abea6ac5ec6f51d0f5a15e437
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472109"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="e6380-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6380-103">timeConstraint resource type</span></span>

<span data-ttu-id="e6380-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6380-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6380-105">根据指定的活动和开放时间段的性质，将会议时间建议限制为一周中的特定时段和天。</span><span class="sxs-lookup"><span data-stu-id="e6380-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6380-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6380-106">JSON representation</span></span>
<span data-ttu-id="e6380-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6380-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e6380-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6380-108">Properties</span></span>
| <span data-ttu-id="e6380-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6380-109">Property</span></span>     | <span data-ttu-id="e6380-110">类型</span><span class="sxs-lookup"><span data-stu-id="e6380-110">Type</span></span>   |<span data-ttu-id="e6380-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6380-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6380-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="e6380-112">activityDomain</span></span>|<span data-ttu-id="e6380-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="e6380-113">activityDomain</span></span>|<span data-ttu-id="e6380-114">（可选）会议性质。</span><span class="sxs-lookup"><span data-stu-id="e6380-114">The nature of the activity, optional.</span></span> <span data-ttu-id="e6380-115">可能的值是： `work` 、 `personal` 或 `unrestricted` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="e6380-115">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="e6380-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="e6380-116">timeslots</span></span>|<span data-ttu-id="e6380-117">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6380-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="e6380-118">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="e6380-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


