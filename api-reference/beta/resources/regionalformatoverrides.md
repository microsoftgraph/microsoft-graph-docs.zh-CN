---
title: regionalFormatOverrides 资源类型
description: 表示日历、日期和时间的区域格式替代的资源。
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 437b67f6a99017bb20096dbd20451b7662145cbd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777594"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="69cc4-103">regionalFormatOverrides 资源类型</span><span class="sxs-lookup"><span data-stu-id="69cc4-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="69cc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69cc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69cc4-105">表示日历、 日期和时间的格式替代的字符串的集合。</span><span class="sxs-lookup"><span data-stu-id="69cc4-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="69cc4-106">属性</span><span class="sxs-lookup"><span data-stu-id="69cc4-106">Properties</span></span>

|<span data-ttu-id="69cc4-107">属性</span><span class="sxs-lookup"><span data-stu-id="69cc4-107">Property</span></span>             |<span data-ttu-id="69cc4-108">类型</span><span class="sxs-lookup"><span data-stu-id="69cc4-108">Type</span></span>                 |<span data-ttu-id="69cc4-109">说明</span><span class="sxs-lookup"><span data-stu-id="69cc4-109">Description</span></span>                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|<span data-ttu-id="69cc4-110">calendar</span><span class="sxs-lookup"><span data-stu-id="69cc4-110">calendar</span></span>             |<span data-ttu-id="69cc4-111">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-111">String</span></span>               |<span data-ttu-id="69cc4-112">要使用的日历，例如公历。</span><span class="sxs-lookup"><span data-stu-id="69cc4-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="69cc4-113">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-113">Returned by default.</span></span>|                   
|<span data-ttu-id="69cc4-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="69cc4-114">firstDayOfWeek</span></span>       |<span data-ttu-id="69cc4-115">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-115">String</span></span>               |<span data-ttu-id="69cc4-116">一周的第一天，例如星期日。</span><span class="sxs-lookup"><span data-stu-id="69cc4-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="69cc4-117">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-117">Returned by default.</span></span>|
|<span data-ttu-id="69cc4-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="69cc4-118">shortDateFormat</span></span>      |<span data-ttu-id="69cc4-119">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-119">String</span></span>               |<span data-ttu-id="69cc4-120">用于显示日期的短日期时间格式。</span><span class="sxs-lookup"><span data-stu-id="69cc4-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="69cc4-121">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-121">Returned by default.</span></span>|
|<span data-ttu-id="69cc4-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="69cc4-122">longDateFormat</span></span>       |<span data-ttu-id="69cc4-123">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-123">String</span></span>               |<span data-ttu-id="69cc4-124">用于显示日期的长日期时间格式。</span><span class="sxs-lookup"><span data-stu-id="69cc4-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="69cc4-125">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-125">Returned by default.</span></span>|
|<span data-ttu-id="69cc4-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="69cc4-126">shortTimeFormat</span></span>      |<span data-ttu-id="69cc4-127">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-127">String</span></span>               |<span data-ttu-id="69cc4-128">用于显示时间的时间的短时间格式。</span><span class="sxs-lookup"><span data-stu-id="69cc4-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="69cc4-129">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-129">Returned by default.</span></span>|
|<span data-ttu-id="69cc4-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="69cc4-130">longTimeFormat</span></span>       |<span data-ttu-id="69cc4-131">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-131">String</span></span>               |<span data-ttu-id="69cc4-132">用于显示时间的长期格式。</span><span class="sxs-lookup"><span data-stu-id="69cc4-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="69cc4-133">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-133">Returned by default.</span></span>|
|<span data-ttu-id="69cc4-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="69cc4-134">timeZone</span></span>             |<span data-ttu-id="69cc4-135">String</span><span class="sxs-lookup"><span data-stu-id="69cc4-135">String</span></span>               |<span data-ttu-id="69cc4-136">用于显示时间的时间区。</span><span class="sxs-lookup"><span data-stu-id="69cc4-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="69cc4-137">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="69cc4-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69cc4-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69cc4-138">JSON representation</span></span>

<span data-ttu-id="69cc4-139">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="69cc4-139">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.regionalFormatOverrides"
}-->

```json
{
    "calendar": "string",
    "firstDayOfWeek": "string",
    "shortDateFormat": "string",
    "longDateFormat": "string",
    "shortTimeFormat": "string",
    "longTimeFormat": "string",
    "timeZone": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalFormatOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


