---
title: daylightTimeZoneOffset 资源类型
description: 指定时区何时从标准时间切换到夏令时。
localization_priority: Normal
ms.openlocfilehash: 160163d6f574eb75746fa751e383c06696006e43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507584"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="a612c-103">daylightTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="a612c-103">daylightTimeZoneOffset resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a612c-104">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="a612c-104">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="a612c-105">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="a612c-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="a612c-106">**bias** 为 300</span><span class="sxs-lookup"><span data-stu-id="a612c-106">**bias** is 300</span></span>
- <span data-ttu-id="a612c-107">**daylightBias** 为 -100</span><span class="sxs-lookup"><span data-stu-id="a612c-107">**daylightBias** is -100</span></span>
- <span data-ttu-id="a612c-108">**dayOccurrence** 为 4</span><span class="sxs-lookup"><span data-stu-id="a612c-108">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="a612c-109">**dayOfWeek** 为“sunday”</span><span class="sxs-lookup"><span data-stu-id="a612c-109">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="a612c-110">**month** 为 5</span><span class="sxs-lookup"><span data-stu-id="a612c-110">**month** is 5</span></span>
- <span data-ttu-id="a612c-111">**time** 为 02:00:00 _ **year** 为 0，意味着夏令时的时长比 UTC 早 +300-100=200 分钟。</span><span class="sxs-lookup"><span data-stu-id="a612c-111">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="a612c-112">从夏令时到标准时间的时区切换出现在每年五月第四个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="a612c-112">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="a612c-113">属性</span><span class="sxs-lookup"><span data-stu-id="a612c-113">Properties</span></span>
| <span data-ttu-id="a612c-114">属性</span><span class="sxs-lookup"><span data-stu-id="a612c-114">Property</span></span>     | <span data-ttu-id="a612c-115">类型</span><span class="sxs-lookup"><span data-stu-id="a612c-115">Type</span></span>   |<span data-ttu-id="a612c-116">说明</span><span class="sxs-lookup"><span data-stu-id="a612c-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a612c-117">daylightBias</span><span class="sxs-lookup"><span data-stu-id="a612c-117">daylightBias</span></span> | <span data-ttu-id="a612c-118">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="a612c-118">Edm.Int32</span></span> | <span data-ttu-id="a612c-119">夏时制与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="a612c-119">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="a612c-120">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="a612c-120">This value is in minutes.</span></span>  |
| <span data-ttu-id="a612c-121">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="a612c-121">dayOccurrence</span></span> | <span data-ttu-id="a612c-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="a612c-122">Edm.Int32</span></span> | <span data-ttu-id="a612c-123">表示从标准时间到夏令时的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="a612c-123">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="a612c-124">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a612c-124">dayOfWeek</span></span> | <span data-ttu-id="a612c-125">string</span><span class="sxs-lookup"><span data-stu-id="a612c-125">string</span></span> | <span data-ttu-id="a612c-126">表示从标准时间到夏令时的切换出现时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="a612c-126">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="a612c-127">month</span><span class="sxs-lookup"><span data-stu-id="a612c-127">month</span></span> | <span data-ttu-id="a612c-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="a612c-128">Edm.Int32</span></span> | <span data-ttu-id="a612c-129">表示从标准时间到夏令时的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="a612c-129">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="a612c-130">time</span><span class="sxs-lookup"><span data-stu-id="a612c-130">time</span></span> | <span data-ttu-id="a612c-131">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a612c-131">Edm.TimeOfDay</span></span> | <span data-ttu-id="a612c-132">表示从标准时间到夏令时的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="a612c-132">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="a612c-133">year</span><span class="sxs-lookup"><span data-stu-id="a612c-133">year</span></span> | <span data-ttu-id="a612c-134">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="a612c-134">Edm.Int32</span></span> | <span data-ttu-id="a612c-135">表示从标准时间到夏令时的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="a612c-135">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="a612c-136">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="a612c-136">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a612c-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a612c-137">JSON representation</span></span>

<span data-ttu-id="a612c-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a612c-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/daylighttimezoneoffset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
