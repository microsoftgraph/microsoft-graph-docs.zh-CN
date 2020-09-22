---
title: meetingActivityStatistics 资源类型
description: 表示有关用户的会议活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3d1f9c7ad147b6aa3f4d52c314931d5c40af2b47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971690"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="d414b-103">meetingActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="d414b-103">meetingActivityStatistics resource type</span></span>

<span data-ttu-id="d414b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d414b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d414b-105">表示有关用户在 Microsoft Outlook、Microsoft 团队或 Skype for Business 会议中所用时间的数据。</span><span class="sxs-lookup"><span data-stu-id="d414b-105">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="d414b-106">这基于 [activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="d414b-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="d414b-107">属性</span><span class="sxs-lookup"><span data-stu-id="d414b-107">Properties</span></span>

| <span data-ttu-id="d414b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d414b-108">Property</span></span>     | <span data-ttu-id="d414b-109">类型</span><span class="sxs-lookup"><span data-stu-id="d414b-109">Type</span></span>        | <span data-ttu-id="d414b-110">说明</span><span class="sxs-lookup"><span data-stu-id="d414b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d414b-111">activity</span><span class="sxs-lookup"><span data-stu-id="d414b-111">activity</span></span>|<span data-ttu-id="d414b-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="d414b-112">analyticsActivityType</span></span>| <span data-ttu-id="d414b-113">为其返回统计信息的会议活动。</span><span class="sxs-lookup"><span data-stu-id="d414b-113">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="d414b-114">duration</span><span class="sxs-lookup"><span data-stu-id="d414b-114">duration</span></span>|<span data-ttu-id="d414b-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-115">Duration</span></span>|<span data-ttu-id="d414b-116">会议上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="d414b-116">Total hours spent on meetings.</span></span> <span data-ttu-id="d414b-117">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="d414b-118">endDate</span><span class="sxs-lookup"><span data-stu-id="d414b-118">endDate</span></span>|<span data-ttu-id="d414b-119">日期</span><span class="sxs-lookup"><span data-stu-id="d414b-119">Date</span></span>|<span data-ttu-id="d414b-120">会议活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="d414b-120">Date when the meeting activity ended.</span></span> <span data-ttu-id="d414b-121">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="d414b-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="d414b-122">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="d414b-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="d414b-123">id</span><span class="sxs-lookup"><span data-stu-id="d414b-123">id</span></span>|<span data-ttu-id="d414b-124">String</span><span class="sxs-lookup"><span data-stu-id="d414b-124">String</span></span>| <span data-ttu-id="d414b-125">会议活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="d414b-125">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="d414b-126">startDate</span><span class="sxs-lookup"><span data-stu-id="d414b-126">startDate</span></span>|<span data-ttu-id="d414b-127">日期</span><span class="sxs-lookup"><span data-stu-id="d414b-127">Date</span></span>|<span data-ttu-id="d414b-128">会议活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="d414b-128">Date when the meeting activity started.</span></span> <span data-ttu-id="d414b-129">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="d414b-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="d414b-130">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="d414b-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="d414b-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="d414b-131">timeZoneUsed</span></span>|<span data-ttu-id="d414b-132">String</span><span class="sxs-lookup"><span data-stu-id="d414b-132">String</span></span>|<span data-ttu-id="d414b-133">用户在 Outlook 日历中设置的 Outlook 时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="d414b-133">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="d414b-134">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="d414b-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="d414b-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="d414b-135">afterHours</span></span>|<span data-ttu-id="d414b-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-136">Duration</span></span>|<span data-ttu-id="d414b-137">在会议上花费的时间超出工作时间，基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-137">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="d414b-138">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-138">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="d414b-139">存在</span><span class="sxs-lookup"><span data-stu-id="d414b-139">conflicting</span></span>|<span data-ttu-id="d414b-140">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-140">Duration</span></span>|<span data-ttu-id="d414b-141">与接受的人员和人员的状态设置为 "忙碌") 的其他会议 (的会议冲突会议所用的时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-141">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="d414b-142">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="d414b-143">long</span><span class="sxs-lookup"><span data-stu-id="d414b-143">long</span></span>|<span data-ttu-id="d414b-144">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-144">Duration</span></span>|<span data-ttu-id="d414b-145">长时间内会议花费的时间 (持续时间) 的一小时以上。</span><span class="sxs-lookup"><span data-stu-id="d414b-145">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="d414b-146">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-146">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="d414b-147">多</span><span class="sxs-lookup"><span data-stu-id="d414b-147">multitasking</span></span>|<span data-ttu-id="d414b-148">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-148">Duration</span></span>|<span data-ttu-id="d414b-149">在会议中，人员在多任务工作 (读取/发送的最少电子邮件数和/或发送的邮件数超过最少数量的电子邮件和/或在 Skype for business) 中所用的时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-149">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="d414b-150">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-150">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="d414b-151">有条不紊</span><span class="sxs-lookup"><span data-stu-id="d414b-151">organized</span></span>|<span data-ttu-id="d414b-152">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-152">Duration</span></span>|<span data-ttu-id="d414b-153">由用户组织的会议所用的时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-153">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="d414b-154">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-154">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="d414b-155">重复性</span><span class="sxs-lookup"><span data-stu-id="d414b-155">recurring</span></span>|<span data-ttu-id="d414b-156">持续时间</span><span class="sxs-lookup"><span data-stu-id="d414b-156">Duration</span></span>|<span data-ttu-id="d414b-157">对定期会议花费的时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-157">Time spent on recurring meetings.</span></span> <span data-ttu-id="d414b-158">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="d414b-158">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d414b-159">关系</span><span class="sxs-lookup"><span data-stu-id="d414b-159">Relationships</span></span>

<span data-ttu-id="d414b-160">无</span><span class="sxs-lookup"><span data-stu-id="d414b-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d414b-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d414b-161">JSON representation</span></span>

<span data-ttu-id="d414b-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d414b-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
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
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

