---
title: bookingWorkHours 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9a51fb9d4f97dde2e3b50d9a19481eeab31483d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527533"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="c068e-104">bookingWorkHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="c068e-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="c068e-105">代表一组的一天的周， [bookingBusiness](bookingbusiness.md)或[bookingStaffMember](bookingstaffmember.md)中的工作时间。</span><span class="sxs-lookup"><span data-stu-id="c068e-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c068e-106">属性</span><span class="sxs-lookup"><span data-stu-id="c068e-106">Properties</span></span>
| <span data-ttu-id="c068e-107">属性</span><span class="sxs-lookup"><span data-stu-id="c068e-107">Property</span></span>     | <span data-ttu-id="c068e-108">类型</span><span class="sxs-lookup"><span data-stu-id="c068e-108">Type</span></span>   |<span data-ttu-id="c068e-109">说明</span><span class="sxs-lookup"><span data-stu-id="c068e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c068e-110">Day</span><span class="sxs-lookup"><span data-stu-id="c068e-110">day</span></span>|<span data-ttu-id="c068e-111">String</span><span class="sxs-lookup"><span data-stu-id="c068e-111">String</span></span>| <span data-ttu-id="c068e-112">此实例表示一周中的某一天。</span><span class="sxs-lookup"><span data-stu-id="c068e-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="c068e-113">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="c068e-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="c068e-114">timeslots</span><span class="sxs-lookup"><span data-stu-id="c068e-114">timeSlots</span></span>|<span data-ttu-id="c068e-115">[bookingWorkTimeSlot](bookingworktimeslot.md)集合</span><span class="sxs-lookup"><span data-stu-id="c068e-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="c068e-116">在一天开始/结束时间的列表。</span><span class="sxs-lookup"><span data-stu-id="c068e-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c068e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c068e-117">JSON representation</span></span>

<span data-ttu-id="c068e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c068e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworkhours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
