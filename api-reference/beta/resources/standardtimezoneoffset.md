---
title: standardTimeZoneOffset 资源类型
description: 指定时区何时从夏令时切换到标准时间。
ms.openlocfilehash: 167ff45f4ccf1615c1560c3f2ba130cdc7747043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044822"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="b6511-103">standardTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6511-103">standardTimeZoneOffset resource type</span></span>

> <span data-ttu-id="b6511-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6511-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6511-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6511-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6511-106">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="b6511-106">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="b6511-107">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="b6511-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="b6511-108">**dayOccurrence** 为 3</span><span class="sxs-lookup"><span data-stu-id="b6511-108">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="b6511-109">**dayOfWeek** 为“Sunday”</span><span class="sxs-lookup"><span data-stu-id="b6511-109">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="b6511-110">**month** 为 10</span><span class="sxs-lookup"><span data-stu-id="b6511-110">**month** is 10</span></span>
- <span data-ttu-id="b6511-111">**time** 为 02:00:00 _ **year** 为 0，这意味着从夏令时切换到标准时间出现在每年十月第三个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="b6511-111">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="b6511-112">属性</span><span class="sxs-lookup"><span data-stu-id="b6511-112">Properties</span></span>
| <span data-ttu-id="b6511-113">属性</span><span class="sxs-lookup"><span data-stu-id="b6511-113">Property</span></span>     | <span data-ttu-id="b6511-114">类型</span><span class="sxs-lookup"><span data-stu-id="b6511-114">Type</span></span>   |<span data-ttu-id="b6511-115">说明</span><span class="sxs-lookup"><span data-stu-id="b6511-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6511-116">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="b6511-116">dayOccurrence</span></span> | <span data-ttu-id="b6511-117">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b6511-117">Edm.Int32</span></span> | <span data-ttu-id="b6511-118">表示从夏令时到标准时间的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="b6511-118">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="b6511-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b6511-119">dayOfWeek</span></span> | <span data-ttu-id="b6511-120">string</span><span class="sxs-lookup"><span data-stu-id="b6511-120">string</span></span> | <span data-ttu-id="b6511-121">表示从夏令时切换为标准时间时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="b6511-121">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="b6511-122">month</span><span class="sxs-lookup"><span data-stu-id="b6511-122">month</span></span> | <span data-ttu-id="b6511-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b6511-123">Edm.Int32</span></span> | <span data-ttu-id="b6511-124">表示从夏令时到标准时间的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="b6511-124">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="b6511-125">time</span><span class="sxs-lookup"><span data-stu-id="b6511-125">time</span></span> | <span data-ttu-id="b6511-126">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b6511-126">Edm.TimeOfDay</span></span> | <span data-ttu-id="b6511-127">表示从夏令时到标准时间的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="b6511-127">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="b6511-128">year</span><span class="sxs-lookup"><span data-stu-id="b6511-128">year</span></span> | <span data-ttu-id="b6511-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b6511-129">Edm.Int32</span></span> | <span data-ttu-id="b6511-130">表示从夏令时到标准时间的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="b6511-130">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="b6511-131">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="b6511-131">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6511-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6511-132">JSON representation</span></span>

<span data-ttu-id="b6511-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6511-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->