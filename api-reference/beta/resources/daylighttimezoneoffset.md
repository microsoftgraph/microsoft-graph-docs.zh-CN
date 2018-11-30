---
title: daylightTimeZoneOffset 资源类型
description: 指定时区何时从标准时间切换到夏令时。
ms.openlocfilehash: 1504a3c1bb1b2d6c691aadf1d073a95453f76d2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041857"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="2525e-103">daylightTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="2525e-103">daylightTimeZoneOffset resource type</span></span>

> <span data-ttu-id="2525e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2525e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2525e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2525e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2525e-106">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="2525e-106">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="2525e-107">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="2525e-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="2525e-108">**bias** 为 300</span><span class="sxs-lookup"><span data-stu-id="2525e-108">**bias** is 300</span></span>
- <span data-ttu-id="2525e-109">**daylightBias** 为 -100</span><span class="sxs-lookup"><span data-stu-id="2525e-109">**daylightBias** is -100</span></span>
- <span data-ttu-id="2525e-110">**dayOccurrence** 为 4</span><span class="sxs-lookup"><span data-stu-id="2525e-110">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="2525e-111">**dayOfWeek** 为“sunday”</span><span class="sxs-lookup"><span data-stu-id="2525e-111">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="2525e-112">**month** 为 5</span><span class="sxs-lookup"><span data-stu-id="2525e-112">**month** is 5</span></span>
- <span data-ttu-id="2525e-113">**time** 为 02:00:00 _ **year** 为 0，意味着夏令时的时长比 UTC 早 +300-100=200 分钟。</span><span class="sxs-lookup"><span data-stu-id="2525e-113">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="2525e-114">从夏令时到标准时间的时区切换出现在每年五月第四个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="2525e-114">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="2525e-115">属性</span><span class="sxs-lookup"><span data-stu-id="2525e-115">Properties</span></span>
| <span data-ttu-id="2525e-116">属性</span><span class="sxs-lookup"><span data-stu-id="2525e-116">Property</span></span>     | <span data-ttu-id="2525e-117">类型</span><span class="sxs-lookup"><span data-stu-id="2525e-117">Type</span></span>   |<span data-ttu-id="2525e-118">说明</span><span class="sxs-lookup"><span data-stu-id="2525e-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2525e-119">daylightBias</span><span class="sxs-lookup"><span data-stu-id="2525e-119">daylightBias</span></span> | <span data-ttu-id="2525e-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="2525e-120">Edm.Int32</span></span> | <span data-ttu-id="2525e-121">夏时制与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="2525e-121">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="2525e-122">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="2525e-122">This value is in minutes.</span></span>  |
| <span data-ttu-id="2525e-123">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="2525e-123">dayOccurrence</span></span> | <span data-ttu-id="2525e-124">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="2525e-124">Edm.Int32</span></span> | <span data-ttu-id="2525e-125">表示从标准时间到夏令时的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="2525e-125">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="2525e-126">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="2525e-126">dayOfWeek</span></span> | <span data-ttu-id="2525e-127">string</span><span class="sxs-lookup"><span data-stu-id="2525e-127">string</span></span> | <span data-ttu-id="2525e-128">表示从标准时间到夏令时的切换出现时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="2525e-128">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="2525e-129">month</span><span class="sxs-lookup"><span data-stu-id="2525e-129">month</span></span> | <span data-ttu-id="2525e-130">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="2525e-130">Edm.Int32</span></span> | <span data-ttu-id="2525e-131">表示从标准时间到夏令时的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="2525e-131">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="2525e-132">time</span><span class="sxs-lookup"><span data-stu-id="2525e-132">time</span></span> | <span data-ttu-id="2525e-133">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2525e-133">Edm.TimeOfDay</span></span> | <span data-ttu-id="2525e-134">表示从标准时间到夏令时的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="2525e-134">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="2525e-135">year</span><span class="sxs-lookup"><span data-stu-id="2525e-135">year</span></span> | <span data-ttu-id="2525e-136">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="2525e-136">Edm.Int32</span></span> | <span data-ttu-id="2525e-137">表示从标准时间到夏令时的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="2525e-137">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="2525e-138">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="2525e-138">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2525e-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2525e-139">JSON representation</span></span>

<span data-ttu-id="2525e-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2525e-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->