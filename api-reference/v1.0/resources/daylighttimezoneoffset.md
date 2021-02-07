---
title: daylightTimeZoneOffset 资源类型
description: 指定时区何时从标准时间切换到夏令时。
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 79e5af9a7a117d3747928d211229bbbd27d046bf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135144"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="7e6bc-103">daylightTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e6bc-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="7e6bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e6bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e6bc-105">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-105">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="7e6bc-106">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="7e6bc-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="7e6bc-107">**bias** 为 300</span><span class="sxs-lookup"><span data-stu-id="7e6bc-107">**bias** is 300</span></span>
- <span data-ttu-id="7e6bc-108">**daylightBias** 为 -100</span><span class="sxs-lookup"><span data-stu-id="7e6bc-108">**daylightBias** is -100</span></span>
- <span data-ttu-id="7e6bc-109">**dayOccurrence** 为 4</span><span class="sxs-lookup"><span data-stu-id="7e6bc-109">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="7e6bc-110">**dayOfWeek** 为“sunday”</span><span class="sxs-lookup"><span data-stu-id="7e6bc-110">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="7e6bc-111">**month** 为 5</span><span class="sxs-lookup"><span data-stu-id="7e6bc-111">**month** is 5</span></span>
- <span data-ttu-id="7e6bc-112">**time** 为 02:00:00 _ **year** 为 0，意味着夏令时的时长比 UTC 早 +300-100=200 分钟。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-112">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="7e6bc-113">从夏令时到标准时间的时区切换出现在每年五月第四个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-113">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="7e6bc-114">属性</span><span class="sxs-lookup"><span data-stu-id="7e6bc-114">Properties</span></span>
| <span data-ttu-id="7e6bc-115">属性</span><span class="sxs-lookup"><span data-stu-id="7e6bc-115">Property</span></span>     | <span data-ttu-id="7e6bc-116">类型</span><span class="sxs-lookup"><span data-stu-id="7e6bc-116">Type</span></span>   |<span data-ttu-id="7e6bc-117">说明</span><span class="sxs-lookup"><span data-stu-id="7e6bc-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e6bc-118">daylightBias</span><span class="sxs-lookup"><span data-stu-id="7e6bc-118">daylightBias</span></span> | <span data-ttu-id="7e6bc-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="7e6bc-119">Edm.Int32</span></span> | <span data-ttu-id="7e6bc-120">夏时制与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-120">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="7e6bc-121">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-121">This value is in minutes.</span></span>  |
| <span data-ttu-id="7e6bc-122">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="7e6bc-122">dayOccurrence</span></span> | <span data-ttu-id="7e6bc-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="7e6bc-123">Edm.Int32</span></span> | <span data-ttu-id="7e6bc-124">表示从标准时间到夏令时的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-124">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="7e6bc-125">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="7e6bc-125">dayOfWeek</span></span> | <span data-ttu-id="7e6bc-126">string</span><span class="sxs-lookup"><span data-stu-id="7e6bc-126">string</span></span> | <span data-ttu-id="7e6bc-127">表示从标准时间到夏令时的切换出现时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-127">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="7e6bc-128">month</span><span class="sxs-lookup"><span data-stu-id="7e6bc-128">month</span></span> | <span data-ttu-id="7e6bc-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="7e6bc-129">Edm.Int32</span></span> | <span data-ttu-id="7e6bc-130">表示从标准时间到夏令时的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-130">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="7e6bc-131">time</span><span class="sxs-lookup"><span data-stu-id="7e6bc-131">time</span></span> | <span data-ttu-id="7e6bc-132">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7e6bc-132">Edm.TimeOfDay</span></span> | <span data-ttu-id="7e6bc-133">表示从标准时间到夏令时的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-133">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="7e6bc-134">year</span><span class="sxs-lookup"><span data-stu-id="7e6bc-134">year</span></span> | <span data-ttu-id="7e6bc-135">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="7e6bc-135">Edm.Int32</span></span> | <span data-ttu-id="7e6bc-136">表示从标准时间到夏令时的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-136">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="7e6bc-137">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-137">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7e6bc-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e6bc-138">JSON representation</span></span>

<span data-ttu-id="7e6bc-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e6bc-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
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

