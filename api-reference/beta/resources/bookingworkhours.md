---
title: bookingWorkHours 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 389b035dcef92db166e4290c71160c12842dc887
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338850"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="cb222-104">bookingWorkHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb222-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="cb222-105">代表[bookingBusiness](bookingbusiness.md)或[bookingStaffMember](bookingstaffmember.md)的一周中一天的工作时间集。</span><span class="sxs-lookup"><span data-stu-id="cb222-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cb222-106">属性</span><span class="sxs-lookup"><span data-stu-id="cb222-106">Properties</span></span>
| <span data-ttu-id="cb222-107">属性</span><span class="sxs-lookup"><span data-stu-id="cb222-107">Property</span></span>     | <span data-ttu-id="cb222-108">类型</span><span class="sxs-lookup"><span data-stu-id="cb222-108">Type</span></span>   |<span data-ttu-id="cb222-109">说明</span><span class="sxs-lookup"><span data-stu-id="cb222-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb222-110">为期</span><span class="sxs-lookup"><span data-stu-id="cb222-110">day</span></span>|<span data-ttu-id="cb222-111">String</span><span class="sxs-lookup"><span data-stu-id="cb222-111">String</span></span>| <span data-ttu-id="cb222-112">此实例所代表的星期中的一天。</span><span class="sxs-lookup"><span data-stu-id="cb222-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="cb222-113">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="cb222-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="cb222-114">因此</span><span class="sxs-lookup"><span data-stu-id="cb222-114">timeSlots</span></span>|<span data-ttu-id="cb222-115">[bookingWorkTimeSlot](bookingworktimeslot.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb222-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="cb222-116">一天中的开始/结束时间的列表。</span><span class="sxs-lookup"><span data-stu-id="cb222-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb222-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb222-117">JSON representation</span></span>

<span data-ttu-id="cb222-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb222-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
