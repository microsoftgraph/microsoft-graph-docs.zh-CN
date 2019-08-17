---
title: meetingActivityStatistics 资源类型
description: 表示有关用户的会议活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa0e4b12ed260c0f6660544e7f48cfe1ca9cd3dc
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450723"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="4585f-103">meetingActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="4585f-103">meetingActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4585f-104">表示有关用户在 Microsoft Outlook、Microsoft 团队或 Skype for Business 会议中所用时间的数据。</span><span class="sxs-lookup"><span data-stu-id="4585f-104">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="4585f-105">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="4585f-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="4585f-106">属性</span><span class="sxs-lookup"><span data-stu-id="4585f-106">Properties</span></span>

| <span data-ttu-id="4585f-107">属性</span><span class="sxs-lookup"><span data-stu-id="4585f-107">Property</span></span>     | <span data-ttu-id="4585f-108">类型</span><span class="sxs-lookup"><span data-stu-id="4585f-108">Type</span></span>        | <span data-ttu-id="4585f-109">说明</span><span class="sxs-lookup"><span data-stu-id="4585f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4585f-110">activity</span><span class="sxs-lookup"><span data-stu-id="4585f-110">activity</span></span>|<span data-ttu-id="4585f-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="4585f-111">analyticsActivityType</span></span>| <span data-ttu-id="4585f-112">为其返回统计信息的会议活动。</span><span class="sxs-lookup"><span data-stu-id="4585f-112">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="4585f-113">duration</span><span class="sxs-lookup"><span data-stu-id="4585f-113">duration</span></span>|<span data-ttu-id="4585f-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-114">Duration</span></span>|<span data-ttu-id="4585f-115">会议上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="4585f-115">Total hours spent on meetings.</span></span> <span data-ttu-id="4585f-116">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4585f-117">endDate</span><span class="sxs-lookup"><span data-stu-id="4585f-117">endDate</span></span>|<span data-ttu-id="4585f-118">Date</span><span class="sxs-lookup"><span data-stu-id="4585f-118">Date</span></span>|<span data-ttu-id="4585f-119">会议活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="4585f-119">Date when the meeting activity ended.</span></span> <span data-ttu-id="4585f-120">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="4585f-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="4585f-121">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="4585f-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="4585f-122">id</span><span class="sxs-lookup"><span data-stu-id="4585f-122">id</span></span>|<span data-ttu-id="4585f-123">String</span><span class="sxs-lookup"><span data-stu-id="4585f-123">String</span></span>| <span data-ttu-id="4585f-124">会议活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="4585f-124">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="4585f-125">startDate</span><span class="sxs-lookup"><span data-stu-id="4585f-125">startDate</span></span>|<span data-ttu-id="4585f-126">日期</span><span class="sxs-lookup"><span data-stu-id="4585f-126">Date</span></span>|<span data-ttu-id="4585f-127">会议活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="4585f-127">Date when the meeting activity started.</span></span> <span data-ttu-id="4585f-128">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="4585f-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="4585f-129">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="4585f-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="4585f-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="4585f-130">timeZoneUsed</span></span>|<span data-ttu-id="4585f-131">String</span><span class="sxs-lookup"><span data-stu-id="4585f-131">String</span></span>|<span data-ttu-id="4585f-132">用户在 Outlook 日历中设置的 Outlook 时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="4585f-132">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="4585f-133">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="4585f-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="4585f-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="4585f-134">afterHours</span></span>|<span data-ttu-id="4585f-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-135">Duration</span></span>|<span data-ttu-id="4585f-136">在会议上花费的时间超出工作时间, 基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-136">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="4585f-137">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-137">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4585f-138">存在</span><span class="sxs-lookup"><span data-stu-id="4585f-138">conflicting</span></span>|<span data-ttu-id="4585f-139">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-139">Duration</span></span>|<span data-ttu-id="4585f-140">在冲突会议中花费的时间 (会议与接受人员的人以及将人员的状态设置为 "忙碌" 的其他会议重叠)。</span><span class="sxs-lookup"><span data-stu-id="4585f-140">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="4585f-141">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4585f-142">long</span><span class="sxs-lookup"><span data-stu-id="4585f-142">long</span></span>|<span data-ttu-id="4585f-143">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-143">Duration</span></span>|<span data-ttu-id="4585f-144">长会议花费的时间 (持续时间超过一个小时)。</span><span class="sxs-lookup"><span data-stu-id="4585f-144">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="4585f-145">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-145">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4585f-146">多</span><span class="sxs-lookup"><span data-stu-id="4585f-146">multitasking</span></span>|<span data-ttu-id="4585f-147">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-147">Duration</span></span>|<span data-ttu-id="4585f-148">人员在会议中花费的时间, 在这种情况下, 用户进行了多任务处理 (读取/发送的电子邮件数量超过最少, 并/或发送的邮件数超过团队或 Skype for Business 中的最少邮件数)。</span><span class="sxs-lookup"><span data-stu-id="4585f-148">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="4585f-149">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-149">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4585f-150">有条不紊</span><span class="sxs-lookup"><span data-stu-id="4585f-150">organized</span></span>|<span data-ttu-id="4585f-151">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-151">Duration</span></span>|<span data-ttu-id="4585f-152">由用户组织的会议所用的时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-152">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="4585f-153">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-153">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4585f-154">重复性</span><span class="sxs-lookup"><span data-stu-id="4585f-154">recurring</span></span>|<span data-ttu-id="4585f-155">持续时间</span><span class="sxs-lookup"><span data-stu-id="4585f-155">Duration</span></span>|<span data-ttu-id="4585f-156">对定期会议花费的时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-156">Time spent on recurring meetings.</span></span> <span data-ttu-id="4585f-157">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="4585f-157">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4585f-158">关系</span><span class="sxs-lookup"><span data-stu-id="4585f-158">Relationships</span></span>

<span data-ttu-id="4585f-159">无</span><span class="sxs-lookup"><span data-stu-id="4585f-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4585f-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4585f-160">JSON representation</span></span>

<span data-ttu-id="4585f-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4585f-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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