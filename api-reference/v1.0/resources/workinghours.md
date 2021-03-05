---
title: workingHours 资源类型
description: 表示特定时区用户一周的工作天数和小时数。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c6ebab4fe505e93bc9a4980aeb1e7999aa5a78f0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473439"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="b85a2-103">workingHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="b85a2-103">workingHours resource type</span></span>

<span data-ttu-id="b85a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b85a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b85a2-105">表示特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="b85a2-105">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="b85a2-106">在处理活动或资源规划应用场景中，访问用户的工作时间会有所帮助。</span><span class="sxs-lookup"><span data-stu-id="b85a2-106">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="b85a2-107">可以[获取](../api/user-get-mailboxsettings.md#example-3)用户的工作时间，并将其[设置](../api/user-update-mailboxsettings.md#example-2)为用户[邮箱设置](mailboxsettings.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="b85a2-107">You can [get](../api/user-get-mailboxsettings.md#example-3) and [set](../api/user-update-mailboxsettings.md#example-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="b85a2-108">可以选择以不同于在 Outlook 客户端设置时区的方式，为你的工作时间设置时区。</span><span class="sxs-lookup"><span data-stu-id="b85a2-108">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="b85a2-109">在某些情况下这很有用，比如当你在一个与平常工作时区不同的地方旅行时。</span><span class="sxs-lookup"><span data-stu-id="b85a2-109">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="b85a2-110">可以将 Outlook 客户端设置</span><span class="sxs-lookup"><span data-stu-id="b85a2-110">You can set the Outlook client</span></span>  
<span data-ttu-id="b85a2-111">为目标时区，以便在你访问时 Outlook 时间值显示为本地时间。</span><span class="sxs-lookup"><span data-stu-id="b85a2-111">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="b85a2-112">当其他人在你通常的工作地点申请与你进行工作会议时，他们仍然可以在相应的时区遵守你的工作时间。</span><span class="sxs-lookup"><span data-stu-id="b85a2-112">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="b85a2-113">属性</span><span class="sxs-lookup"><span data-stu-id="b85a2-113">Properties</span></span>
| <span data-ttu-id="b85a2-114">属性</span><span class="sxs-lookup"><span data-stu-id="b85a2-114">Property</span></span>     | <span data-ttu-id="b85a2-115">类型</span><span class="sxs-lookup"><span data-stu-id="b85a2-115">Type</span></span>   |<span data-ttu-id="b85a2-116">说明</span><span class="sxs-lookup"><span data-stu-id="b85a2-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b85a2-117">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="b85a2-117">daysOfWeek</span></span> | <span data-ttu-id="b85a2-118">dayOfWeek 集合</span><span class="sxs-lookup"><span data-stu-id="b85a2-118">dayOfWeek collection</span></span> | <span data-ttu-id="b85a2-119">用户一周工作的天数。</span><span class="sxs-lookup"><span data-stu-id="b85a2-119">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="b85a2-120">startTime</span><span class="sxs-lookup"><span data-stu-id="b85a2-120">startTime</span></span> | <span data-ttu-id="b85a2-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b85a2-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="b85a2-122">一天中用户开始工作的时间。</span><span class="sxs-lookup"><span data-stu-id="b85a2-122">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="b85a2-123">endTime</span><span class="sxs-lookup"><span data-stu-id="b85a2-123">endTime</span></span> | <span data-ttu-id="b85a2-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b85a2-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="b85a2-125">一天中用户停止工作的时间。</span><span class="sxs-lookup"><span data-stu-id="b85a2-125">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="b85a2-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="b85a2-126">timeZone</span></span> | [<span data-ttu-id="b85a2-127">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="b85a2-127">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="b85a2-128">工作时间应用的时区。</span><span class="sxs-lookup"><span data-stu-id="b85a2-128">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b85a2-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b85a2-129">JSON representation</span></span>

<span data-ttu-id="b85a2-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b85a2-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "String (timeofday)",
  "endTime": "String (timeofday)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->

