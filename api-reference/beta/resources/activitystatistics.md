---
title: activityStatistics 资源类型
description: 表示在工作活动上花费的时间，包括电子邮件、会议、焦点工作、聊天和呼叫。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 18d675b38dd3155b5a06c67fc3164fd315d7c0b2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162496"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="a4592-103">activityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4592-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4592-104">表示用户在工作时间内和工作时间以外的各种工作活动所花费的时间，用于请求中的指定时间范围，这将使用一天的聚合周期。</span><span class="sxs-lookup"><span data-stu-id="a4592-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="a4592-105">以下类型的统计信息派生自**activityStatistics**：</span><span class="sxs-lookup"><span data-stu-id="a4592-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="a4592-106">Call</span><span class="sxs-lookup"><span data-stu-id="a4592-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="a4592-107">参与</span><span class="sxs-lookup"><span data-stu-id="a4592-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="a4592-108">电子邮件</span><span class="sxs-lookup"><span data-stu-id="a4592-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="a4592-109">焦点</span><span class="sxs-lookup"><span data-stu-id="a4592-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="a4592-110">要求</span><span class="sxs-lookup"><span data-stu-id="a4592-110">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="a4592-111">方法</span><span class="sxs-lookup"><span data-stu-id="a4592-111">Methods</span></span>

| <span data-ttu-id="a4592-112">方法</span><span class="sxs-lookup"><span data-stu-id="a4592-112">Method</span></span>       | <span data-ttu-id="a4592-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4592-113">Return Type</span></span> | <span data-ttu-id="a4592-114">说明</span><span class="sxs-lookup"><span data-stu-id="a4592-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a4592-115">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="a4592-115">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="a4592-116">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="a4592-116">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="a4592-117">在最后一个完整的星期检索用户的活动统计信息集合的属性。</span><span class="sxs-lookup"><span data-stu-id="a4592-117">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4592-118">属性</span><span class="sxs-lookup"><span data-stu-id="a4592-118">Properties</span></span>

| <span data-ttu-id="a4592-119">属性</span><span class="sxs-lookup"><span data-stu-id="a4592-119">Property</span></span>     | <span data-ttu-id="a4592-120">类型</span><span class="sxs-lookup"><span data-stu-id="a4592-120">Type</span></span>        | <span data-ttu-id="a4592-121">说明</span><span class="sxs-lookup"><span data-stu-id="a4592-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4592-122">activity</span><span class="sxs-lookup"><span data-stu-id="a4592-122">activity</span></span>|<span data-ttu-id="a4592-123">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="a4592-123">analyticsActivityType</span></span>| <span data-ttu-id="a4592-124">返回其统计信息的活动的类型。</span><span class="sxs-lookup"><span data-stu-id="a4592-124">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="a4592-125">可能的值为： `call`、 `chat`、 `email` `focus`、和`meeting`。</span><span class="sxs-lookup"><span data-stu-id="a4592-125">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span>|
|<span data-ttu-id="a4592-126">duration</span><span class="sxs-lookup"><span data-stu-id="a4592-126">duration</span></span>|<span data-ttu-id="a4592-127">持续时间</span><span class="sxs-lookup"><span data-stu-id="a4592-127">Duration</span></span>|<span data-ttu-id="a4592-128">活动所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="a4592-128">Total hours spent on the activity.</span></span> <span data-ttu-id="a4592-129">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="a4592-129">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="a4592-130">endDate</span><span class="sxs-lookup"><span data-stu-id="a4592-130">endDate</span></span>|<span data-ttu-id="a4592-131">Date</span><span class="sxs-lookup"><span data-stu-id="a4592-131">Date</span></span>|<span data-ttu-id="a4592-132">活动结束的日期，以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="a4592-132">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="a4592-133">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="a4592-133">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="a4592-134">id</span><span class="sxs-lookup"><span data-stu-id="a4592-134">id</span></span>|<span data-ttu-id="a4592-135">String</span><span class="sxs-lookup"><span data-stu-id="a4592-135">String</span></span>| <span data-ttu-id="a4592-136">活动的只读 ID，表示`{activity}_{startdate}_{enddate}`为。</span><span class="sxs-lookup"><span data-stu-id="a4592-136">Read-only ID for the activity, which represents `{activity}_{startdate}_{enddate}`.</span></span>|
|<span data-ttu-id="a4592-137">startDate</span><span class="sxs-lookup"><span data-stu-id="a4592-137">startDate</span></span>|<span data-ttu-id="a4592-138">日期</span><span class="sxs-lookup"><span data-stu-id="a4592-138">Date</span></span>|<span data-ttu-id="a4592-139">活动启动的日期，以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="a4592-139">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="a4592-140">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="a4592-140">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="a4592-141">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="a4592-141">timeZoneUsed</span></span>|<span data-ttu-id="a4592-142">String</span><span class="sxs-lookup"><span data-stu-id="a4592-142">String</span></span>|<span data-ttu-id="a4592-143">用户在 Microsoft Outlook 中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="a4592-143">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="a4592-144">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="a4592-144">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4592-145">关系</span><span class="sxs-lookup"><span data-stu-id="a4592-145">Relationships</span></span>

<span data-ttu-id="a4592-146">无</span><span class="sxs-lookup"><span data-stu-id="a4592-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4592-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4592-147">JSON representation</span></span>

<span data-ttu-id="a4592-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4592-148">The following is a JSON representation of the resource.</span></span>

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