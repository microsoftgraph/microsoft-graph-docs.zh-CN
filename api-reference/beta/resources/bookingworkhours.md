---
title: bookingWorkHours 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9a51fb9d4f97dde2e3b50d9a19481eeab31483d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535479"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="3fa1b-104">bookingWorkHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="3fa1b-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3fa1b-105">代表[bookingBusiness](bookingbusiness.md)或[bookingStaffMember](bookingstaffmember.md)的一周中一天的工作时间集。</span><span class="sxs-lookup"><span data-stu-id="3fa1b-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3fa1b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3fa1b-106">Properties</span></span>
| <span data-ttu-id="3fa1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="3fa1b-107">Property</span></span>     | <span data-ttu-id="3fa1b-108">类型</span><span class="sxs-lookup"><span data-stu-id="3fa1b-108">Type</span></span>   |<span data-ttu-id="3fa1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3fa1b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fa1b-110">为期</span><span class="sxs-lookup"><span data-stu-id="3fa1b-110">day</span></span>|<span data-ttu-id="3fa1b-111">String</span><span class="sxs-lookup"><span data-stu-id="3fa1b-111">String</span></span>| <span data-ttu-id="3fa1b-112">此实例所代表的星期中的一天。</span><span class="sxs-lookup"><span data-stu-id="3fa1b-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="3fa1b-113">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="3fa1b-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="3fa1b-114">因此</span><span class="sxs-lookup"><span data-stu-id="3fa1b-114">timeSlots</span></span>|<span data-ttu-id="3fa1b-115">[bookingWorkTimeSlot](bookingworktimeslot.md)集合</span><span class="sxs-lookup"><span data-stu-id="3fa1b-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="3fa1b-116">一天中的开始/结束时间的列表。</span><span class="sxs-lookup"><span data-stu-id="3fa1b-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fa1b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3fa1b-117">JSON representation</span></span>

<span data-ttu-id="3fa1b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fa1b-118">The following is a JSON representation of the resource.</span></span>

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
