---
title: timeConstraint 资源类型
description: 根据指定的活动和打开时间段的性质, 将会议时间建议限制在一周的特定时间和几天。
localization_priority: Normal
ms.openlocfilehash: b6e239abbd0d9f7b4f83df4a60625a2f88131476
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456950"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="bdbf0-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdbf0-103">timeConstraint resource type</span></span>

<span data-ttu-id="bdbf0-104">根据指定的活动和打开时间段的性质, 将会议时间建议限制在一周的特定时间和几天。</span><span class="sxs-lookup"><span data-stu-id="bdbf0-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdbf0-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdbf0-105">JSON representation</span></span>

<span data-ttu-id="bdbf0-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdbf0-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bdbf0-107">属性</span><span class="sxs-lookup"><span data-stu-id="bdbf0-107">Properties</span></span>
| <span data-ttu-id="bdbf0-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdbf0-108">Property</span></span>     | <span data-ttu-id="bdbf0-109">类型</span><span class="sxs-lookup"><span data-stu-id="bdbf0-109">Type</span></span>   |<span data-ttu-id="bdbf0-110">说明</span><span class="sxs-lookup"><span data-stu-id="bdbf0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdbf0-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="bdbf0-111">activityDomain</span></span>|<span data-ttu-id="bdbf0-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="bdbf0-112">activityDomain</span></span>|<span data-ttu-id="bdbf0-113">（可选）会议性质。</span><span class="sxs-lookup"><span data-stu-id="bdbf0-113">The nature of the activity, optional.</span></span> <span data-ttu-id="bdbf0-114">可能的值是: `work`、 `personal`、 `unrestricted`或`unknown`。</span><span class="sxs-lookup"><span data-stu-id="bdbf0-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="bdbf0-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="bdbf0-115">timeslots</span></span>|<span data-ttu-id="bdbf0-116">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdbf0-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="bdbf0-117">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="bdbf0-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
