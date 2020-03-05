---
title: activityStatistics 资源类型
description: 表示在工作活动上花费的时间，包括电子邮件、会议、焦点工作、聊天和呼叫。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 69b90ae911ca956dedf3a7675d7666c7faa4b906
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508427"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="13f94-103">activityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="13f94-103">activityStatistics resource type</span></span>

<span data-ttu-id="13f94-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="13f94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13f94-105">表示用户在工作时间内和工作时间以外的各种工作活动所花费的时间，用于请求中的指定时间范围，这将使用一天的聚合周期。</span><span class="sxs-lookup"><span data-stu-id="13f94-105">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="13f94-106">以下类型的统计信息派生自**activityStatistics**：</span><span class="sxs-lookup"><span data-stu-id="13f94-106">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="13f94-107">通话</span><span class="sxs-lookup"><span data-stu-id="13f94-107">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="13f94-108">聊天</span><span class="sxs-lookup"><span data-stu-id="13f94-108">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="13f94-109">电子邮件</span><span class="sxs-lookup"><span data-stu-id="13f94-109">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="13f94-110">焦点</span><span class="sxs-lookup"><span data-stu-id="13f94-110">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="13f94-111">要求</span><span class="sxs-lookup"><span data-stu-id="13f94-111">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="13f94-112">方法</span><span class="sxs-lookup"><span data-stu-id="13f94-112">Methods</span></span>

| <span data-ttu-id="13f94-113">方法</span><span class="sxs-lookup"><span data-stu-id="13f94-113">Method</span></span>       | <span data-ttu-id="13f94-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="13f94-114">Return Type</span></span> | <span data-ttu-id="13f94-115">说明</span><span class="sxs-lookup"><span data-stu-id="13f94-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="13f94-116">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="13f94-116">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="13f94-117">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="13f94-117">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="13f94-118">在最后一个完整的星期检索用户的活动统计信息集合的属性。</span><span class="sxs-lookup"><span data-stu-id="13f94-118">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span> |

## <a name="properties"></a><span data-ttu-id="13f94-119">属性</span><span class="sxs-lookup"><span data-stu-id="13f94-119">Properties</span></span>

| <span data-ttu-id="13f94-120">属性</span><span class="sxs-lookup"><span data-stu-id="13f94-120">Property</span></span>     | <span data-ttu-id="13f94-121">类型</span><span class="sxs-lookup"><span data-stu-id="13f94-121">Type</span></span>        | <span data-ttu-id="13f94-122">说明</span><span class="sxs-lookup"><span data-stu-id="13f94-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13f94-123">activity</span><span class="sxs-lookup"><span data-stu-id="13f94-123">activity</span></span> |<span data-ttu-id="13f94-124">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="13f94-124">analyticsActivityType</span></span> |<span data-ttu-id="13f94-125">返回其统计信息的活动的类型。</span><span class="sxs-lookup"><span data-stu-id="13f94-125">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="13f94-126">可能的值为： `call`、 `chat`、 `email` `focus`、和`meeting`。</span><span class="sxs-lookup"><span data-stu-id="13f94-126">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span> |
|<span data-ttu-id="13f94-127">duration</span><span class="sxs-lookup"><span data-stu-id="13f94-127">duration</span></span> |<span data-ttu-id="13f94-128">持续时间</span><span class="sxs-lookup"><span data-stu-id="13f94-128">Duration</span></span> |<span data-ttu-id="13f94-129">活动所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="13f94-129">Total hours spent on the activity.</span></span> <span data-ttu-id="13f94-130">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="13f94-130">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="13f94-131">endDate</span><span class="sxs-lookup"><span data-stu-id="13f94-131">endDate</span></span> |<span data-ttu-id="13f94-132">Date</span><span class="sxs-lookup"><span data-stu-id="13f94-132">Date</span></span> |<span data-ttu-id="13f94-133">活动结束的日期，以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="13f94-133">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="13f94-134">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="13f94-134">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="13f94-135">id</span><span class="sxs-lookup"><span data-stu-id="13f94-135">id</span></span> |<span data-ttu-id="13f94-136">String</span><span class="sxs-lookup"><span data-stu-id="13f94-136">String</span></span> |<span data-ttu-id="13f94-137">活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="13f94-137">Read-only ID for the activity.</span></span> <span data-ttu-id="13f94-138">请勿为您的方案分析或自定义值。</span><span class="sxs-lookup"><span data-stu-id="13f94-138">Do not parse or customize the value for your scenarios.</span></span> |
|<span data-ttu-id="13f94-139">startDate</span><span class="sxs-lookup"><span data-stu-id="13f94-139">startDate</span></span> |<span data-ttu-id="13f94-140">日期</span><span class="sxs-lookup"><span data-stu-id="13f94-140">Date</span></span> |<span data-ttu-id="13f94-141">活动启动的日期，以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="13f94-141">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="13f94-142">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="13f94-142">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="13f94-143">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="13f94-143">timeZoneUsed</span></span> |<span data-ttu-id="13f94-144">String</span><span class="sxs-lookup"><span data-stu-id="13f94-144">String</span></span> |<span data-ttu-id="13f94-145">用户在 Microsoft Outlook 中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="13f94-145">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="13f94-146">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="13f94-146">For example, the property value could be "Pacific Standard Time."</span></span> |

## <a name="relationships"></a><span data-ttu-id="13f94-147">关系</span><span class="sxs-lookup"><span data-stu-id="13f94-147">Relationships</span></span>

<span data-ttu-id="13f94-148">无</span><span class="sxs-lookup"><span data-stu-id="13f94-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13f94-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13f94-149">JSON representation</span></span>

<span data-ttu-id="13f94-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13f94-150">The following is a JSON representation of the resource.</span></span>

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