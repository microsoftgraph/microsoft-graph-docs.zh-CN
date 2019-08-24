---
title: meetingActivityStatistics 资源类型
description: 表示有关用户的会议活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 14d926a41680f1292b7599bd76b458705b426719
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622535"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="9e6b8-103">meetingActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e6b8-103">meetingActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e6b8-104">表示有关用户在 Microsoft Outlook、Microsoft 团队或 Skype for Business 会议中所用时间的数据。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-104">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="9e6b8-105">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="9e6b8-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e6b8-106">Properties</span></span>

| <span data-ttu-id="9e6b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e6b8-107">Property</span></span>     | <span data-ttu-id="9e6b8-108">类型</span><span class="sxs-lookup"><span data-stu-id="9e6b8-108">Type</span></span>        | <span data-ttu-id="9e6b8-109">说明</span><span class="sxs-lookup"><span data-stu-id="9e6b8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e6b8-110">activity</span><span class="sxs-lookup"><span data-stu-id="9e6b8-110">activity</span></span>|<span data-ttu-id="9e6b8-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="9e6b8-111">analyticsActivityType</span></span>| <span data-ttu-id="9e6b8-112">为其返回统计信息的会议活动。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-112">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="9e6b8-113">duration</span><span class="sxs-lookup"><span data-stu-id="9e6b8-113">duration</span></span>|<span data-ttu-id="9e6b8-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-114">Duration</span></span>|<span data-ttu-id="9e6b8-115">会议上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-115">Total hours spent on meetings.</span></span> <span data-ttu-id="9e6b8-116">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="9e6b8-117">endDate</span><span class="sxs-lookup"><span data-stu-id="9e6b8-117">endDate</span></span>|<span data-ttu-id="9e6b8-118">Date</span><span class="sxs-lookup"><span data-stu-id="9e6b8-118">Date</span></span>|<span data-ttu-id="9e6b8-119">会议活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-119">Date when the meeting activity ended.</span></span> <span data-ttu-id="9e6b8-120">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="9e6b8-121">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="9e6b8-122">id</span><span class="sxs-lookup"><span data-stu-id="9e6b8-122">id</span></span>|<span data-ttu-id="9e6b8-123">String</span><span class="sxs-lookup"><span data-stu-id="9e6b8-123">String</span></span>| <span data-ttu-id="9e6b8-124">会议活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-124">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="9e6b8-125">startDate</span><span class="sxs-lookup"><span data-stu-id="9e6b8-125">startDate</span></span>|<span data-ttu-id="9e6b8-126">日期</span><span class="sxs-lookup"><span data-stu-id="9e6b8-126">Date</span></span>|<span data-ttu-id="9e6b8-127">会议活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-127">Date when the meeting activity started.</span></span> <span data-ttu-id="9e6b8-128">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="9e6b8-129">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="9e6b8-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="9e6b8-130">timeZoneUsed</span></span>|<span data-ttu-id="9e6b8-131">String</span><span class="sxs-lookup"><span data-stu-id="9e6b8-131">String</span></span>|<span data-ttu-id="9e6b8-132">用户在 Outlook 日历中设置的 Outlook 时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-132">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="9e6b8-133">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="9e6b8-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="9e6b8-134">afterHours</span></span>|<span data-ttu-id="9e6b8-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-135">Duration</span></span>|<span data-ttu-id="9e6b8-136">在会议上花费的时间超出工作时间, 基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-136">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="9e6b8-137">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-137">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="9e6b8-138">存在</span><span class="sxs-lookup"><span data-stu-id="9e6b8-138">conflicting</span></span>|<span data-ttu-id="9e6b8-139">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-139">Duration</span></span>|<span data-ttu-id="9e6b8-140">在冲突会议中花费的时间 (会议与接受人员的人以及将人员的状态设置为 "忙碌" 的其他会议重叠)。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-140">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="9e6b8-141">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="9e6b8-142">long</span><span class="sxs-lookup"><span data-stu-id="9e6b8-142">long</span></span>|<span data-ttu-id="9e6b8-143">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-143">Duration</span></span>|<span data-ttu-id="9e6b8-144">长会议花费的时间 (持续时间超过一个小时)。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-144">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="9e6b8-145">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-145">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="9e6b8-146">多</span><span class="sxs-lookup"><span data-stu-id="9e6b8-146">multitasking</span></span>|<span data-ttu-id="9e6b8-147">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-147">Duration</span></span>|<span data-ttu-id="9e6b8-148">人员在会议中花费的时间, 在这种情况下, 用户进行了多任务处理 (读取/发送的电子邮件数量超过最少, 并/或发送的邮件数超过团队或 Skype for Business 中的最少邮件数)。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-148">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="9e6b8-149">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-149">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="9e6b8-150">有条不紊</span><span class="sxs-lookup"><span data-stu-id="9e6b8-150">organized</span></span>|<span data-ttu-id="9e6b8-151">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-151">Duration</span></span>|<span data-ttu-id="9e6b8-152">由用户组织的会议所用的时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-152">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="9e6b8-153">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-153">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="9e6b8-154">重复性</span><span class="sxs-lookup"><span data-stu-id="9e6b8-154">recurring</span></span>|<span data-ttu-id="9e6b8-155">持续时间</span><span class="sxs-lookup"><span data-stu-id="9e6b8-155">Duration</span></span>|<span data-ttu-id="9e6b8-156">对定期会议花费的时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-156">Time spent on recurring meetings.</span></span> <span data-ttu-id="9e6b8-157">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-157">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e6b8-158">关系</span><span class="sxs-lookup"><span data-stu-id="9e6b8-158">Relationships</span></span>

<span data-ttu-id="9e6b8-159">无</span><span class="sxs-lookup"><span data-stu-id="9e6b8-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e6b8-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e6b8-160">JSON representation</span></span>

<span data-ttu-id="9e6b8-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e6b8-161">The following is a JSON representation of the resource.</span></span>

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