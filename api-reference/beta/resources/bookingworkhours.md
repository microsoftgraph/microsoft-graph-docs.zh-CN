---
title: bookingWorkHours 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 3346ee8eb20e381e1412dcfb16624954658c44fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045001"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="15385-104">bookingWorkHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="15385-104">bookingWorkHours resource type</span></span>

 > <span data-ttu-id="15385-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="15385-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15385-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="15385-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="15385-107">代表一组的一天的周， [bookingBusiness](bookingbusiness.md)或[bookingStaffMember](bookingstaffmember.md)中的工作时间。</span><span class="sxs-lookup"><span data-stu-id="15385-107">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="15385-108">属性</span><span class="sxs-lookup"><span data-stu-id="15385-108">Properties</span></span>
| <span data-ttu-id="15385-109">属性</span><span class="sxs-lookup"><span data-stu-id="15385-109">Property</span></span>     | <span data-ttu-id="15385-110">类型</span><span class="sxs-lookup"><span data-stu-id="15385-110">Type</span></span>   |<span data-ttu-id="15385-111">说明</span><span class="sxs-lookup"><span data-stu-id="15385-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15385-112">一天</span><span class="sxs-lookup"><span data-stu-id="15385-112">day</span></span>|<span data-ttu-id="15385-113">字符串</span><span class="sxs-lookup"><span data-stu-id="15385-113">String</span></span>| <span data-ttu-id="15385-114">此实例表示一周中的某一天。</span><span class="sxs-lookup"><span data-stu-id="15385-114">The day of the week represented by this instance.</span></span> <span data-ttu-id="15385-115">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="15385-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="15385-116">时间段</span><span class="sxs-lookup"><span data-stu-id="15385-116">timeSlots</span></span>|<span data-ttu-id="15385-117">[bookingWorkTimeSlot](bookingworktimeslot.md)集合</span><span class="sxs-lookup"><span data-stu-id="15385-117">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="15385-118">在一天开始/结束时间的列表。</span><span class="sxs-lookup"><span data-stu-id="15385-118">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15385-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15385-119">JSON representation</span></span>

<span data-ttu-id="15385-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15385-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->