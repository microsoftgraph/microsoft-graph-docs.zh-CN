---
title: timeConstraint 资源类型
description: 根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。
ms.openlocfilehash: 82ab18eb09201236f3227c7dd0660519092a3133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008359"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="127e1-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="127e1-103">timeConstraint resource type</span></span>

<span data-ttu-id="127e1-104">根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。</span><span class="sxs-lookup"><span data-stu-id="127e1-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="127e1-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="127e1-105">JSON representation</span></span>

<span data-ttu-id="127e1-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="127e1-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="127e1-107">属性</span><span class="sxs-lookup"><span data-stu-id="127e1-107">Properties</span></span>
| <span data-ttu-id="127e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="127e1-108">Property</span></span>     | <span data-ttu-id="127e1-109">类型</span><span class="sxs-lookup"><span data-stu-id="127e1-109">Type</span></span>   |<span data-ttu-id="127e1-110">说明</span><span class="sxs-lookup"><span data-stu-id="127e1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="127e1-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="127e1-111">activityDomain</span></span>|<span data-ttu-id="127e1-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="127e1-112">activityDomain</span></span>|<span data-ttu-id="127e1-113">活动，可选的特点。</span><span class="sxs-lookup"><span data-stu-id="127e1-113">The nature of the activity, optional.</span></span> <span data-ttu-id="127e1-114">可能的值为： `work`， `personal`， `unrestricted`，或`unknown`。</span><span class="sxs-lookup"><span data-stu-id="127e1-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="127e1-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="127e1-115">timeslots</span></span>|<span data-ttu-id="127e1-116">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="127e1-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="127e1-117">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="127e1-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
