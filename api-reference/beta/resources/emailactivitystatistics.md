---
title: emailActivityStatistics 资源类型
description: 表示有关用户的电子邮件活动的其他信息
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ff75545b7f591a920ed4a1ffd65bff40cff8439b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450725"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="e786f-103">emailActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="e786f-103">emailActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e786f-104">表示有关用户在 Microsoft Outlook 的电子邮件活动中所用时间的数据。</span><span class="sxs-lookup"><span data-stu-id="e786f-104">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="e786f-105">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="e786f-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e786f-106">属性</span><span class="sxs-lookup"><span data-stu-id="e786f-106">Properties</span></span>

| <span data-ttu-id="e786f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e786f-107">Property</span></span>     | <span data-ttu-id="e786f-108">类型</span><span class="sxs-lookup"><span data-stu-id="e786f-108">Type</span></span>        | <span data-ttu-id="e786f-109">说明</span><span class="sxs-lookup"><span data-stu-id="e786f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e786f-110">activity</span><span class="sxs-lookup"><span data-stu-id="e786f-110">activity</span></span>|<span data-ttu-id="e786f-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="e786f-111">analyticsActivityType</span></span>| <span data-ttu-id="e786f-112">返回其统计信息的电子邮件活动。</span><span class="sxs-lookup"><span data-stu-id="e786f-112">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="e786f-113">duration</span><span class="sxs-lookup"><span data-stu-id="e786f-113">duration</span></span>|<span data-ttu-id="e786f-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="e786f-114">Duration</span></span>|<span data-ttu-id="e786f-115">在电子邮件上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="e786f-115">Total hours spent on emails.</span></span> <span data-ttu-id="e786f-116">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="e786f-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="e786f-117">endDate</span><span class="sxs-lookup"><span data-stu-id="e786f-117">endDate</span></span>|<span data-ttu-id="e786f-118">Date</span><span class="sxs-lookup"><span data-stu-id="e786f-118">Date</span></span>|<span data-ttu-id="e786f-119">电子邮件活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="e786f-119">Date when the email activity ended.</span></span> <span data-ttu-id="e786f-120">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="e786f-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="e786f-121">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="e786f-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="e786f-122">id</span><span class="sxs-lookup"><span data-stu-id="e786f-122">id</span></span>|<span data-ttu-id="e786f-123">String</span><span class="sxs-lookup"><span data-stu-id="e786f-123">String</span></span>| <span data-ttu-id="e786f-124">电子邮件活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="e786f-124">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="e786f-125">startDate</span><span class="sxs-lookup"><span data-stu-id="e786f-125">startDate</span></span>|<span data-ttu-id="e786f-126">日期</span><span class="sxs-lookup"><span data-stu-id="e786f-126">Date</span></span>|<span data-ttu-id="e786f-127">电子邮件活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="e786f-127">Date when the email activity started.</span></span> <span data-ttu-id="e786f-128">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="e786f-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="e786f-129">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="e786f-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="e786f-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="e786f-130">timeZoneUsed</span></span>|<span data-ttu-id="e786f-131">String</span><span class="sxs-lookup"><span data-stu-id="e786f-131">String</span></span>|<span data-ttu-id="e786f-132">用户在 Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="e786f-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="e786f-133">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="e786f-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="e786f-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="e786f-134">afterHours</span></span>|<span data-ttu-id="e786f-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="e786f-135">Duration</span></span>|<span data-ttu-id="e786f-136">在工作时间之外的电子邮件上花费的总小时数, 基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="e786f-136">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="e786f-137">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="e786f-137">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="e786f-138">readEmail</span><span class="sxs-lookup"><span data-stu-id="e786f-138">readEmail</span></span>|<span data-ttu-id="e786f-139">持续时间</span><span class="sxs-lookup"><span data-stu-id="e786f-139">Duration</span></span>|<span data-ttu-id="e786f-140">阅读电子邮件所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="e786f-140">Total hours spent reading email.</span></span> <span data-ttu-id="e786f-141">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="e786f-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="e786f-142">sentEmail</span><span class="sxs-lookup"><span data-stu-id="e786f-142">sentEmail</span></span>|<span data-ttu-id="e786f-143">持续时间</span><span class="sxs-lookup"><span data-stu-id="e786f-143">Duration</span></span>|<span data-ttu-id="e786f-144">撰写和发送电子邮件所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="e786f-144">Total hours spent writing and sending email.</span></span> <span data-ttu-id="e786f-145">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="e786f-145">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e786f-146">关系</span><span class="sxs-lookup"><span data-stu-id="e786f-146">Relationships</span></span>

<span data-ttu-id="e786f-147">无</span><span class="sxs-lookup"><span data-stu-id="e786f-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e786f-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e786f-148">JSON representation</span></span>

<span data-ttu-id="e786f-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e786f-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->