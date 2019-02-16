---
title: findMeetingTimesTimeConstraints 资源类型
description: 根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057350"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a><span data-ttu-id="81f73-103">findMeetingTimesTimeConstraints 资源类型</span><span class="sxs-lookup"><span data-stu-id="81f73-103">findMeetingTimesTimeConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81f73-104">将会议时间建议限制为活动和特定时间范围的性质。 |</span><span class="sxs-lookup"><span data-stu-id="81f73-104">Restricts meeting time suggestions to the nature of activity and certain ranges of time.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="81f73-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81f73-105">JSON representation</span></span>

<span data-ttu-id="81f73-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81f73-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="81f73-107">属性</span><span class="sxs-lookup"><span data-stu-id="81f73-107">Properties</span></span>
| <span data-ttu-id="81f73-108">属性</span><span class="sxs-lookup"><span data-stu-id="81f73-108">Property</span></span>     | <span data-ttu-id="81f73-109">类型</span><span class="sxs-lookup"><span data-stu-id="81f73-109">Type</span></span>   |<span data-ttu-id="81f73-110">说明</span><span class="sxs-lookup"><span data-stu-id="81f73-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81f73-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="81f73-111">activityDomain</span></span>|<span data-ttu-id="81f73-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="81f73-112">activityDomain</span></span>|<span data-ttu-id="81f73-p101">（可选）活动性质。可取值为：`work`、`personal`、`unrestricted` 或 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="81f73-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="81f73-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="81f73-115">timeslots</span></span>|<span data-ttu-id="81f73-116">[searchWindowTimeSlot](searchwindowtimeslot.md)集合</span><span class="sxs-lookup"><span data-stu-id="81f73-116">[searchWindowTimeSlot](searchwindowtimeslot.md) collection</span></span>|<span data-ttu-id="81f73-117">要查看可能的会议时间的时间范围数组。</span><span class="sxs-lookup"><span data-stu-id="81f73-117">An array of time ranges to look into for possible meeting times.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->