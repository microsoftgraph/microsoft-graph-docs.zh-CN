---
title: workingHours 资源类型
description: 表示特定时区用户一周的工作天数和小时数。
localization_priority: Normal
ms.openlocfilehash: d34da38ad1a007f6c63154cb496006585df95c13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885735"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="42ad6-103">workingHours 资源类型</span><span class="sxs-lookup"><span data-stu-id="42ad6-103">workingHours resource type</span></span>

> <span data-ttu-id="42ad6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42ad6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42ad6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42ad6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42ad6-106">表示特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="42ad6-106">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="42ad6-107">在处理活动或资源规划应用场景中，访问用户的工作时间会有所帮助。</span><span class="sxs-lookup"><span data-stu-id="42ad6-107">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="42ad6-108">可以[获取](../api/user-get-mailboxsettings.md#request-3)用户的工作时间，并将其[设置](../api/user-update-mailboxsettings.md#request-2)为用户[邮箱设置](mailboxsettings.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="42ad6-108">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="42ad6-109">可以选择以不同于在 Outlook 客户端设置时区的方式，为你的工作时间设置时区。</span><span class="sxs-lookup"><span data-stu-id="42ad6-109">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="42ad6-110">在某些情况下这很有用，比如当你在一个与平常工作时区不同的地方旅行时。</span><span class="sxs-lookup"><span data-stu-id="42ad6-110">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="42ad6-111">可以将 Outlook 客户端设置</span><span class="sxs-lookup"><span data-stu-id="42ad6-111">You can set the Outlook client</span></span>  
<span data-ttu-id="42ad6-112">为目标时区，以便在你访问时 Outlook 时间值显示为本地时间。</span><span class="sxs-lookup"><span data-stu-id="42ad6-112">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="42ad6-113">当其他人在你通常的工作地点申请与你进行工作会议时，他们仍然可以在相应的时区遵守你的工作时间。</span><span class="sxs-lookup"><span data-stu-id="42ad6-113">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="42ad6-114">属性</span><span class="sxs-lookup"><span data-stu-id="42ad6-114">Properties</span></span>
| <span data-ttu-id="42ad6-115">属性</span><span class="sxs-lookup"><span data-stu-id="42ad6-115">Property</span></span>     | <span data-ttu-id="42ad6-116">类型</span><span class="sxs-lookup"><span data-stu-id="42ad6-116">Type</span></span>   |<span data-ttu-id="42ad6-117">说明</span><span class="sxs-lookup"><span data-stu-id="42ad6-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42ad6-118">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="42ad6-118">daysOfWeek</span></span> | <span data-ttu-id="42ad6-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="42ad6-119">String collection</span></span> | <span data-ttu-id="42ad6-120">用户一周工作的天数。</span><span class="sxs-lookup"><span data-stu-id="42ad6-120">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="42ad6-121">startTime</span><span class="sxs-lookup"><span data-stu-id="42ad6-121">startTime</span></span> | <span data-ttu-id="42ad6-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="42ad6-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="42ad6-123">一天中用户开始工作的时间。</span><span class="sxs-lookup"><span data-stu-id="42ad6-123">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="42ad6-124">endTime</span><span class="sxs-lookup"><span data-stu-id="42ad6-124">endTime</span></span> | <span data-ttu-id="42ad6-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="42ad6-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="42ad6-126">一天中用户停止工作的时间。</span><span class="sxs-lookup"><span data-stu-id="42ad6-126">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="42ad6-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="42ad6-127">timeZone</span></span> | [<span data-ttu-id="42ad6-128">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="42ad6-128">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="42ad6-129">工作时间应用的时区。</span><span class="sxs-lookup"><span data-stu-id="42ad6-129">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="42ad6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42ad6-130">JSON representation</span></span>

<span data-ttu-id="42ad6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42ad6-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
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
  "tocPath": ""
}-->
