---
title: regionalFormatOverrides 资源类型
description: 表示日历、日期和时间的区域格式替代的资源。
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 2ed130135571faeced90a638e9334a7e2a185a5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073505"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="83e11-103">regionalFormatOverrides 资源类型</span><span class="sxs-lookup"><span data-stu-id="83e11-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="83e11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83e11-105">表示日历、日期和时间的格式重写的字符串的集合。</span><span class="sxs-lookup"><span data-stu-id="83e11-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="83e11-106">属性</span><span class="sxs-lookup"><span data-stu-id="83e11-106">Properties</span></span>

|<span data-ttu-id="83e11-107">属性</span><span class="sxs-lookup"><span data-stu-id="83e11-107">Property</span></span>             |<span data-ttu-id="83e11-108">类型</span><span class="sxs-lookup"><span data-stu-id="83e11-108">Type</span></span>                 |<span data-ttu-id="83e11-109">说明</span><span class="sxs-lookup"><span data-stu-id="83e11-109">Description</span></span>                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|<span data-ttu-id="83e11-110">calendar</span><span class="sxs-lookup"><span data-stu-id="83e11-110">calendar</span></span>             |<span data-ttu-id="83e11-111">String</span><span class="sxs-lookup"><span data-stu-id="83e11-111">String</span></span>               |<span data-ttu-id="83e11-112">要使用的日历，例如公历。</span><span class="sxs-lookup"><span data-stu-id="83e11-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="83e11-113">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-113">Returned by default.</span></span>|                   
|<span data-ttu-id="83e11-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="83e11-114">firstDayOfWeek</span></span>       |<span data-ttu-id="83e11-115">String</span><span class="sxs-lookup"><span data-stu-id="83e11-115">String</span></span>               |<span data-ttu-id="83e11-116">要使用的一周的第一天（例如，星期日）。</span><span class="sxs-lookup"><span data-stu-id="83e11-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="83e11-117">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-117">Returned by default.</span></span>|
|<span data-ttu-id="83e11-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="83e11-118">shortDateFormat</span></span>      |<span data-ttu-id="83e11-119">String</span><span class="sxs-lookup"><span data-stu-id="83e11-119">String</span></span>               |<span data-ttu-id="83e11-120">要用于显示日期的短日期时间格式。</span><span class="sxs-lookup"><span data-stu-id="83e11-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="83e11-121">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-121">Returned by default.</span></span>|
|<span data-ttu-id="83e11-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="83e11-122">longDateFormat</span></span>       |<span data-ttu-id="83e11-123">String</span><span class="sxs-lookup"><span data-stu-id="83e11-123">String</span></span>               |<span data-ttu-id="83e11-124">用于显示日期的长日期时间格式。</span><span class="sxs-lookup"><span data-stu-id="83e11-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="83e11-125">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-125">Returned by default.</span></span>|
|<span data-ttu-id="83e11-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="83e11-126">shortTimeFormat</span></span>      |<span data-ttu-id="83e11-127">String</span><span class="sxs-lookup"><span data-stu-id="83e11-127">String</span></span>               |<span data-ttu-id="83e11-128">用于显示时间的短时间格式。</span><span class="sxs-lookup"><span data-stu-id="83e11-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="83e11-129">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-129">Returned by default.</span></span>|
|<span data-ttu-id="83e11-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="83e11-130">longTimeFormat</span></span>       |<span data-ttu-id="83e11-131">String</span><span class="sxs-lookup"><span data-stu-id="83e11-131">String</span></span>               |<span data-ttu-id="83e11-132">用于显示时间的长时间格式。</span><span class="sxs-lookup"><span data-stu-id="83e11-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="83e11-133">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-133">Returned by default.</span></span>|
|<span data-ttu-id="83e11-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="83e11-134">timeZone</span></span>             |<span data-ttu-id="83e11-135">String</span><span class="sxs-lookup"><span data-stu-id="83e11-135">String</span></span>               |<span data-ttu-id="83e11-136">要用于显示时间的时区。</span><span class="sxs-lookup"><span data-stu-id="83e11-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="83e11-137">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="83e11-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83e11-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83e11-138">JSON representation</span></span>

<span data-ttu-id="83e11-139">下面是资源的 JSON 定义。</span><span class="sxs-lookup"><span data-stu-id="83e11-139">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "",
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


