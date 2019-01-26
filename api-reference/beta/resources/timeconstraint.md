---
title: timeConstraint 资源类型
description: 根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。
localization_priority: Normal
ms.openlocfilehash: 45469211aa4925834fd9d20da6a9905ac87d221e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577233"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="0ba64-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ba64-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ba64-104">根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。</span><span class="sxs-lookup"><span data-stu-id="0ba64-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ba64-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ba64-105">JSON representation</span></span>

<span data-ttu-id="0ba64-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ba64-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0ba64-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ba64-107">Properties</span></span>
| <span data-ttu-id="0ba64-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ba64-108">Property</span></span>     | <span data-ttu-id="0ba64-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ba64-109">Type</span></span>   |<span data-ttu-id="0ba64-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ba64-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ba64-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="0ba64-111">activityDomain</span></span>|<span data-ttu-id="0ba64-112">String</span><span class="sxs-lookup"><span data-stu-id="0ba64-112">String</span></span>|<span data-ttu-id="0ba64-p101">（可选）活动性质。可取值为：`work`、`personal`、`unrestricted` 或 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="0ba64-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="0ba64-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="0ba64-115">timeslots</span></span>|<span data-ttu-id="0ba64-116">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ba64-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="0ba64-117">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="0ba64-117">An array of time periods.</span></span>|

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
