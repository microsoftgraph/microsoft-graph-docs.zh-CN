---
title: bookingWorkHours 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fab0282e3ce380b8aa4283bd9a783fe8b2fc3390
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463598"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="5265d-104">bookingWorkHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="5265d-104">bookingWorkHours resource type</span></span>

<span data-ttu-id="5265d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5265d-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="5265d-106">代表[bookingBusiness](bookingbusiness.md)或[bookingStaffMember](bookingstaffmember.md)的一周中一天的工作时间集。</span><span class="sxs-lookup"><span data-stu-id="5265d-106">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5265d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5265d-107">Properties</span></span>
| <span data-ttu-id="5265d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5265d-108">Property</span></span>     | <span data-ttu-id="5265d-109">类型</span><span class="sxs-lookup"><span data-stu-id="5265d-109">Type</span></span>   |<span data-ttu-id="5265d-110">说明</span><span class="sxs-lookup"><span data-stu-id="5265d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5265d-111">为期</span><span class="sxs-lookup"><span data-stu-id="5265d-111">day</span></span>|<span data-ttu-id="5265d-112">String</span><span class="sxs-lookup"><span data-stu-id="5265d-112">String</span></span>| <span data-ttu-id="5265d-113">此实例所代表的星期中的一天。</span><span class="sxs-lookup"><span data-stu-id="5265d-113">The day of the week represented by this instance.</span></span> <span data-ttu-id="5265d-114">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="5265d-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="5265d-115">因此</span><span class="sxs-lookup"><span data-stu-id="5265d-115">timeSlots</span></span>|<span data-ttu-id="5265d-116">[bookingWorkTimeSlot](bookingworktimeslot.md)集合</span><span class="sxs-lookup"><span data-stu-id="5265d-116">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="5265d-117">一天中的开始/结束时间的列表。</span><span class="sxs-lookup"><span data-stu-id="5265d-117">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5265d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5265d-118">JSON representation</span></span>

<span data-ttu-id="5265d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5265d-119">The following is a JSON representation of the resource.</span></span>

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
