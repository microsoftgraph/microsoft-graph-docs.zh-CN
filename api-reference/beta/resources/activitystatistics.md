---
title: activityStatistics 资源类型
description: 表示在工作活动上花费的时间，包括电子邮件、会议、焦点工作、聊天和呼叫。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3d2e626535d579b77c27125500d7247401f26915
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280615"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="81b81-103">activityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="81b81-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81b81-104">表示用户在工作时间内和工作时间以外的各种工作活动所花费的时间，用于请求中的指定时间范围，这将使用一天的聚合周期。</span><span class="sxs-lookup"><span data-stu-id="81b81-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="81b81-105">以下类型的统计信息派生自**activityStatistics**：</span><span class="sxs-lookup"><span data-stu-id="81b81-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="81b81-106">Call</span><span class="sxs-lookup"><span data-stu-id="81b81-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="81b81-107">参与</span><span class="sxs-lookup"><span data-stu-id="81b81-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="81b81-108">电子邮件</span><span class="sxs-lookup"><span data-stu-id="81b81-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="81b81-109">焦点</span><span class="sxs-lookup"><span data-stu-id="81b81-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="81b81-110">要求</span><span class="sxs-lookup"><span data-stu-id="81b81-110">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="81b81-111">方法</span><span class="sxs-lookup"><span data-stu-id="81b81-111">Methods</span></span>

| <span data-ttu-id="81b81-112">方法</span><span class="sxs-lookup"><span data-stu-id="81b81-112">Method</span></span>       | <span data-ttu-id="81b81-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="81b81-113">Return Type</span></span> | <span data-ttu-id="81b81-114">说明</span><span class="sxs-lookup"><span data-stu-id="81b81-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="81b81-115">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="81b81-115">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="81b81-116">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="81b81-116">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="81b81-117">在最后一个完整的星期检索用户的活动统计信息集合的属性。</span><span class="sxs-lookup"><span data-stu-id="81b81-117">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span> |

## <a name="properties"></a><span data-ttu-id="81b81-118">属性</span><span class="sxs-lookup"><span data-stu-id="81b81-118">Properties</span></span>

| <span data-ttu-id="81b81-119">属性</span><span class="sxs-lookup"><span data-stu-id="81b81-119">Property</span></span>     | <span data-ttu-id="81b81-120">类型</span><span class="sxs-lookup"><span data-stu-id="81b81-120">Type</span></span>        | <span data-ttu-id="81b81-121">说明</span><span class="sxs-lookup"><span data-stu-id="81b81-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81b81-122">activity</span><span class="sxs-lookup"><span data-stu-id="81b81-122">activity</span></span> |<span data-ttu-id="81b81-123">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="81b81-123">analyticsActivityType</span></span> |<span data-ttu-id="81b81-124">返回其统计信息的活动的类型。</span><span class="sxs-lookup"><span data-stu-id="81b81-124">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="81b81-125">可能的值为： `call`、 `chat`、 `email` `focus`、和`meeting`。</span><span class="sxs-lookup"><span data-stu-id="81b81-125">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span> |
|<span data-ttu-id="81b81-126">duration</span><span class="sxs-lookup"><span data-stu-id="81b81-126">duration</span></span> |<span data-ttu-id="81b81-127">持续时间</span><span class="sxs-lookup"><span data-stu-id="81b81-127">Duration</span></span> |<span data-ttu-id="81b81-128">活动所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="81b81-128">Total hours spent on the activity.</span></span> <span data-ttu-id="81b81-129">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="81b81-129">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="81b81-130">endDate</span><span class="sxs-lookup"><span data-stu-id="81b81-130">endDate</span></span> |<span data-ttu-id="81b81-131">Date</span><span class="sxs-lookup"><span data-stu-id="81b81-131">Date</span></span> |<span data-ttu-id="81b81-132">活动结束的日期，以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="81b81-132">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="81b81-133">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="81b81-133">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="81b81-134">id</span><span class="sxs-lookup"><span data-stu-id="81b81-134">id</span></span> |<span data-ttu-id="81b81-135">String</span><span class="sxs-lookup"><span data-stu-id="81b81-135">String</span></span> |<span data-ttu-id="81b81-136">活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="81b81-136">Read-only ID for the activity.</span></span> <span data-ttu-id="81b81-137">请勿为您的方案分析或自定义值。</span><span class="sxs-lookup"><span data-stu-id="81b81-137">Do not parse or customize the value for your scenarios.</span></span> |
|<span data-ttu-id="81b81-138">startDate</span><span class="sxs-lookup"><span data-stu-id="81b81-138">startDate</span></span> |<span data-ttu-id="81b81-139">日期</span><span class="sxs-lookup"><span data-stu-id="81b81-139">Date</span></span> |<span data-ttu-id="81b81-140">活动启动的日期，以 ISO 8601 格式表示的日历日期。</span><span class="sxs-lookup"><span data-stu-id="81b81-140">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="81b81-141">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="81b81-141">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="81b81-142">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="81b81-142">timeZoneUsed</span></span> |<span data-ttu-id="81b81-143">String</span><span class="sxs-lookup"><span data-stu-id="81b81-143">String</span></span> |<span data-ttu-id="81b81-144">用户在 Microsoft Outlook 中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="81b81-144">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="81b81-145">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="81b81-145">For example, the property value could be "Pacific Standard Time."</span></span> |

## <a name="relationships"></a><span data-ttu-id="81b81-146">关系</span><span class="sxs-lookup"><span data-stu-id="81b81-146">Relationships</span></span>

<span data-ttu-id="81b81-147">无</span><span class="sxs-lookup"><span data-stu-id="81b81-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81b81-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81b81-148">JSON representation</span></span>

<span data-ttu-id="81b81-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81b81-149">The following is a JSON representation of the resource.</span></span>

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