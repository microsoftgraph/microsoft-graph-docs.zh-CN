---
title: regionalFormatOverrides 资源类型
description: 表示日历、日期和时间的区域格式替代的资源。
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2b4046ad8ec6b2d646d1dc2d93cbe7bed205cbad
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516064"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="3085e-103">regionalFormatOverrides 资源类型</span><span class="sxs-lookup"><span data-stu-id="3085e-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="3085e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3085e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3085e-105">表示日历、日期和时间的格式替代的字符串集合。</span><span class="sxs-lookup"><span data-stu-id="3085e-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="3085e-106">属性</span><span class="sxs-lookup"><span data-stu-id="3085e-106">Properties</span></span>

|<span data-ttu-id="3085e-107">属性</span><span class="sxs-lookup"><span data-stu-id="3085e-107">Property</span></span>             |<span data-ttu-id="3085e-108">类型</span><span class="sxs-lookup"><span data-stu-id="3085e-108">Type</span></span>                     |<span data-ttu-id="3085e-109">说明</span><span class="sxs-lookup"><span data-stu-id="3085e-109">Description</span></span>                                                    |
|---------------------|-------------------------|---------------------------------------------------------------|
|<span data-ttu-id="3085e-110">calendar</span><span class="sxs-lookup"><span data-stu-id="3085e-110">calendar</span></span>             |<span data-ttu-id="3085e-111">String</span><span class="sxs-lookup"><span data-stu-id="3085e-111">String</span></span>                   |<span data-ttu-id="3085e-112">要使用的日历，例如公历。</span><span class="sxs-lookup"><span data-stu-id="3085e-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="3085e-113">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-113">Returned by default.</span></span>|                   
|<span data-ttu-id="3085e-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="3085e-114">firstDayOfWeek</span></span>       |<span data-ttu-id="3085e-115">microsoft.graph.dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="3085e-115">microsoft.graph.dayOfWeek</span></span>|<span data-ttu-id="3085e-116">一周的第一天，例如，星期日。</span><span class="sxs-lookup"><span data-stu-id="3085e-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="3085e-117">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-117">Returned by default.</span></span>|
|<span data-ttu-id="3085e-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="3085e-118">shortDateFormat</span></span>      |<span data-ttu-id="3085e-119">String</span><span class="sxs-lookup"><span data-stu-id="3085e-119">String</span></span>                   |<span data-ttu-id="3085e-120">用于显示日期的短日期时间格式。</span><span class="sxs-lookup"><span data-stu-id="3085e-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="3085e-121">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-121">Returned by default.</span></span>|
|<span data-ttu-id="3085e-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="3085e-122">longDateFormat</span></span>       |<span data-ttu-id="3085e-123">String</span><span class="sxs-lookup"><span data-stu-id="3085e-123">String</span></span>                   |<span data-ttu-id="3085e-124">用于显示日期的长日期时间格式。</span><span class="sxs-lookup"><span data-stu-id="3085e-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="3085e-125">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-125">Returned by default.</span></span>|
|<span data-ttu-id="3085e-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="3085e-126">shortTimeFormat</span></span>      |<span data-ttu-id="3085e-127">String</span><span class="sxs-lookup"><span data-stu-id="3085e-127">String</span></span>                   |<span data-ttu-id="3085e-128">用于显示时间的时间短格式。</span><span class="sxs-lookup"><span data-stu-id="3085e-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="3085e-129">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-129">Returned by default.</span></span>|
|<span data-ttu-id="3085e-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="3085e-130">longTimeFormat</span></span>       |<span data-ttu-id="3085e-131">String</span><span class="sxs-lookup"><span data-stu-id="3085e-131">String</span></span>                   |<span data-ttu-id="3085e-132">用于显示时间的长期格式。</span><span class="sxs-lookup"><span data-stu-id="3085e-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="3085e-133">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-133">Returned by default.</span></span>|
|<span data-ttu-id="3085e-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="3085e-134">timeZone</span></span>             |<span data-ttu-id="3085e-135">String</span><span class="sxs-lookup"><span data-stu-id="3085e-135">String</span></span>                   |<span data-ttu-id="3085e-136">用于显示时间的时间区。</span><span class="sxs-lookup"><span data-stu-id="3085e-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="3085e-137">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3085e-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3085e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3085e-138">JSON representation</span></span>

<span data-ttu-id="3085e-139">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="3085e-139">The following is a JSON definition of the resource.</span></span>

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


