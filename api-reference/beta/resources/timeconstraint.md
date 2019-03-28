---
title: timeConstraint 资源类型
description: 根据指定的活动和打开时间段的性质, 将会议时间建议限制在一周的特定时间和几天。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937768"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="69397-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="69397-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69397-104">根据指定的活动和打开时间段的性质, 将会议时间建议限制在一周的特定时间和几天。</span><span class="sxs-lookup"><span data-stu-id="69397-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="69397-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69397-105">JSON representation</span></span>
<span data-ttu-id="69397-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69397-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="69397-107">属性</span><span class="sxs-lookup"><span data-stu-id="69397-107">Properties</span></span>
| <span data-ttu-id="69397-108">属性</span><span class="sxs-lookup"><span data-stu-id="69397-108">Property</span></span>     | <span data-ttu-id="69397-109">类型</span><span class="sxs-lookup"><span data-stu-id="69397-109">Type</span></span>   |<span data-ttu-id="69397-110">说明</span><span class="sxs-lookup"><span data-stu-id="69397-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69397-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="69397-111">activityDomain</span></span>|<span data-ttu-id="69397-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="69397-112">activityDomain</span></span>|<span data-ttu-id="69397-113">（可选）会议性质。</span><span class="sxs-lookup"><span data-stu-id="69397-113">The nature of the activity, optional.</span></span> <span data-ttu-id="69397-114">可能的值包括`work`: `personal`、 `unrestricted`、或`unknown`。</span><span class="sxs-lookup"><span data-stu-id="69397-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="69397-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="69397-115">timeslots</span></span>|<span data-ttu-id="69397-116">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69397-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="69397-117">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="69397-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->