---
title: activityStatistics 资源类型
description: 表示在工作活动上花费的时间, 包括电子邮件、会议、焦点工作、聊天和呼叫。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450721"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="8366f-103">activityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="8366f-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8366f-104">表示用户在工作时间内和工作时间以外的各种工作活动所花费的时间, 用于请求中的指定时间范围, 这将使用一天的聚合周期。</span><span class="sxs-lookup"><span data-stu-id="8366f-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="8366f-105">以下类型的统计信息派生自**activityStatistics**:</span><span class="sxs-lookup"><span data-stu-id="8366f-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="8366f-106">Call</span><span class="sxs-lookup"><span data-stu-id="8366f-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="8366f-107">聊天</span><span class="sxs-lookup"><span data-stu-id="8366f-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="8366f-108">Email</span><span class="sxs-lookup"><span data-stu-id="8366f-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="8366f-109">焦点</span><span class="sxs-lookup"><span data-stu-id="8366f-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="8366f-110">要求</span><span class="sxs-lookup"><span data-stu-id="8366f-110">Meeting</span></span>](meetingactivitystatistics.md)

### <a name="activity-id-property"></a><span data-ttu-id="8366f-111">"活动 id" 属性</span><span class="sxs-lookup"><span data-stu-id="8366f-111">Activity id property</span></span>

<span data-ttu-id="8366f-112">在 HTTP 请求中, 若要获取某个日期范围内的特定类型的活动统计信息, 可以将此信息表示为以下格式的用户的 activityStatistics 集合的 ID, 其中`{startdate}`和`{enddate}`在 ISO 8601 日历中表示日期格式, `{activity}`可以是 "通话"、"聊天"、"电子邮件"、"焦点" 或 "会议":</span><span class="sxs-lookup"><span data-stu-id="8366f-112">In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":</span></span>

```
{activity}_{startdate}_{enddate}
```

<span data-ttu-id="8366f-113">例如, ID "email_2019-08-10 _2019-12" 表示指定用户的 emailActivityStatistics 介于2019年8月10日和 2019 12 月12日之间。</span><span class="sxs-lookup"><span data-stu-id="8366f-113">For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="8366f-114">方法</span><span class="sxs-lookup"><span data-stu-id="8366f-114">Methods</span></span>

| <span data-ttu-id="8366f-115">方法</span><span class="sxs-lookup"><span data-stu-id="8366f-115">Method</span></span>       | <span data-ttu-id="8366f-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="8366f-116">Return Type</span></span> | <span data-ttu-id="8366f-117">说明</span><span class="sxs-lookup"><span data-stu-id="8366f-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8366f-118">获取 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="8366f-118">Get activityStatistics</span></span>](../api/activitystatistics-get.md) | [<span data-ttu-id="8366f-119">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="8366f-119">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="8366f-120">在指定的时间范围内获取用户的指定活动的统计信息的属性。</span><span class="sxs-lookup"><span data-stu-id="8366f-120">Get the properties for a specified activity's statistics for a user, for the specified time range.</span></span> |
| [<span data-ttu-id="8366f-121">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="8366f-121">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="8366f-122">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="8366f-122">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="8366f-123">在最后一个完整的星期检索用户的活动统计信息集合的属性。</span><span class="sxs-lookup"><span data-stu-id="8366f-123">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span>|

## <a name="properties"></a><span data-ttu-id="8366f-124">属性</span><span class="sxs-lookup"><span data-stu-id="8366f-124">Properties</span></span>

| <span data-ttu-id="8366f-125">属性</span><span class="sxs-lookup"><span data-stu-id="8366f-125">Property</span></span>     | <span data-ttu-id="8366f-126">类型</span><span class="sxs-lookup"><span data-stu-id="8366f-126">Type</span></span>        | <span data-ttu-id="8366f-127">说明</span><span class="sxs-lookup"><span data-stu-id="8366f-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8366f-128">activity</span><span class="sxs-lookup"><span data-stu-id="8366f-128">activity</span></span>|<span data-ttu-id="8366f-129">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="8366f-129">analyticsActivityType</span></span>| <span data-ttu-id="8366f-130">返回其统计信息的活动的类型。</span><span class="sxs-lookup"><span data-stu-id="8366f-130">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="8366f-131">可能的值为: `call`、 `chat`、 `email` `focus`、和`meeting`。</span><span class="sxs-lookup"><span data-stu-id="8366f-131">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span>|
|<span data-ttu-id="8366f-132">duration</span><span class="sxs-lookup"><span data-stu-id="8366f-132">duration</span></span>|<span data-ttu-id="8366f-133">持续时间</span><span class="sxs-lookup"><span data-stu-id="8366f-133">Duration</span></span>|<span data-ttu-id="8366f-134">活动所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="8366f-134">Total hours spent on the activity.</span></span> <span data-ttu-id="8366f-135">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="8366f-135">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="8366f-136">endDate</span><span class="sxs-lookup"><span data-stu-id="8366f-136">endDate</span></span>|<span data-ttu-id="8366f-137">Date</span><span class="sxs-lookup"><span data-stu-id="8366f-137">Date</span></span>|<span data-ttu-id="8366f-138">活动结束的日期, 以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="8366f-138">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="8366f-139">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="8366f-139">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="8366f-140">id</span><span class="sxs-lookup"><span data-stu-id="8366f-140">id</span></span>|<span data-ttu-id="8366f-141">String</span><span class="sxs-lookup"><span data-stu-id="8366f-141">String</span></span>| <span data-ttu-id="8366f-142">活动的只读 ID, 表示`{activity}_{startdate}_{enddate}`为。</span><span class="sxs-lookup"><span data-stu-id="8366f-142">Read-only ID for the activity, which represents `{activity}_{startdate}_{enddate}`.</span></span>|
|<span data-ttu-id="8366f-143">startDate</span><span class="sxs-lookup"><span data-stu-id="8366f-143">startDate</span></span>|<span data-ttu-id="8366f-144">日期</span><span class="sxs-lookup"><span data-stu-id="8366f-144">Date</span></span>|<span data-ttu-id="8366f-145">活动启动的日期, 以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="8366f-145">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="8366f-146">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="8366f-146">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="8366f-147">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="8366f-147">timeZoneUsed</span></span>|<span data-ttu-id="8366f-148">String</span><span class="sxs-lookup"><span data-stu-id="8366f-148">String</span></span>|<span data-ttu-id="8366f-149">用户在 Microsoft Outlook 中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="8366f-149">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="8366f-150">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="8366f-150">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="8366f-151">关系</span><span class="sxs-lookup"><span data-stu-id="8366f-151">Relationships</span></span>

<span data-ttu-id="8366f-152">无</span><span class="sxs-lookup"><span data-stu-id="8366f-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8366f-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8366f-153">JSON representation</span></span>

<span data-ttu-id="8366f-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8366f-154">The following is a JSON representation of the resource.</span></span>

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 