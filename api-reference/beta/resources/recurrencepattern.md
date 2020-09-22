---
title: recurrencePattern 资源类型
description: 描述了定期事件的重复发生频率。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: ab3b33a00467dffb5a65865be3c0d3cdbc5c2dcd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073535"
---
# <a name="recurrencepattern-resource-type"></a><span data-ttu-id="f8346-103">recurrencePattern 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8346-103">recurrencePattern resource type</span></span>

<span data-ttu-id="f8346-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8346-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8346-105">描述了定期[事件](event.md)的重复发生频率。</span><span class="sxs-lookup"><span data-stu-id="f8346-105">Describes the frequency by which a recurring [event](event.md) repeats.</span></span>

<span data-ttu-id="f8346-106">可以使用下面的 6 种方法之一（具体视方案而定），指定定期事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="f8346-106">You can specify the recurrence pattern of a recurring event in one of 6 ways depending on your scenario.</span></span> <span data-ttu-id="f8346-107">对于每种类型的模式，请指定时间间隔。</span><span class="sxs-lookup"><span data-stu-id="f8346-107">For each pattern type, specify the amount of time between occurrences.</span></span> <span data-ttu-id="f8346-108">在为事件指定的日期范围内，实际发生的定期事件始终遵循此模式。</span><span class="sxs-lookup"><span data-stu-id="f8346-108">The actual occurrences of the recurring event always follow this pattern falling within the date range that you specify for the event.</span></span> <span data-ttu-id="f8346-109">定期事件始终由 **recurrencePattern**（事件的重复发生频率）和 [recurrenceRange](recurrencerange.md)（事件在哪个日期范围内重复发生）进行定义。</span><span class="sxs-lookup"><span data-stu-id="f8346-109">A recurring event is always defined by its **recurrencePattern** (how frequently the event repeats), and its [recurrenceRange](recurrencerange.md) (over how long the event repeats).</span></span>

<span data-ttu-id="f8346-110">**type** 属性可用于指定不同类型的 **recurrencePattern**，**interval** 属性可用于指定时间间隔，可以是天数、周数、月数或年数，具体视 **type** 而定。</span><span class="sxs-lookup"><span data-stu-id="f8346-110">Use the **type** property to specify the different types of **recurrencePattern**, and the **interval** property to specify the time between occurrences, which can be in number of days, weeks, months, or years, depending on the **type**.</span></span> <span data-ttu-id="f8346-111">请注意每种类型的必需属性，如下表所述。</span><span class="sxs-lookup"><span data-stu-id="f8346-111">Note which properties are required for each type, as described in the following table.</span></span>

> <span data-ttu-id="f8346-112">**注意**：仅添加定期模式需要的属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-112">**Note** Include only the properties that you need for a recurrence pattern.</span></span> <span data-ttu-id="f8346-113">如果添加的任何属性没有受支持的值，则会引发错误。</span><span class="sxs-lookup"><span data-stu-id="f8346-113">Any property that you include that does not have a supported value would result in an error.</span></span>

| <span data-ttu-id="f8346-114">定期模式类型</span><span class="sxs-lookup"><span data-stu-id="f8346-114">Type of recurrence pattern</span></span> | <span data-ttu-id="f8346-115">type 属性值</span><span class="sxs-lookup"><span data-stu-id="f8346-115">Value of type property</span></span> | <span data-ttu-id="f8346-116">说明</span><span class="sxs-lookup"><span data-stu-id="f8346-116">Description</span></span> | <span data-ttu-id="f8346-117">示例</span><span class="sxs-lookup"><span data-stu-id="f8346-117">Example</span></span> | <span data-ttu-id="f8346-118">必需属性</span><span class="sxs-lookup"><span data-stu-id="f8346-118">Required properties</span></span> |
|:---------------|:--------|:--------|:--------|:----------|
| <span data-ttu-id="f8346-119">每天</span><span class="sxs-lookup"><span data-stu-id="f8346-119">Daily</span></span> | `daily` | <span data-ttu-id="f8346-120">事件按 **interval** 指定的时间间隔天数重复发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-120">Event repeats based on the number of days specified by **interval** between occurrences.</span></span> | <span data-ttu-id="f8346-121">事件每 3 天重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="f8346-121">Repeat event every 3 days.</span></span> | <span data-ttu-id="f8346-122">**type**、**interval**</span><span class="sxs-lookup"><span data-stu-id="f8346-122">**type**, **interval**</span></span> |
| <span data-ttu-id="f8346-123">每周</span><span class="sxs-lookup"><span data-stu-id="f8346-123">Weekly</span></span> | `weekly` | <span data-ttu-id="f8346-124">事件按时间间隔周数在一周内的一天或几天重复发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-124">Event repeats on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span> | <span data-ttu-id="f8346-125">事件每两个星期一和星期二重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="f8346-125">Repeat event Monday and Tuesday of every other week.</span></span> | <span data-ttu-id="f8346-126">**type**、**interval**、**daysOfWeek**、**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="f8346-126">**type**, **interval**, **daysOfWeek**, **firstDayOfWeek**</span></span> |
| <span data-ttu-id="f8346-127">绝对每月</span><span class="sxs-lookup"><span data-stu-id="f8346-127">Absolute monthly</span></span> | `absoluteMonthly` | <span data-ttu-id="f8346-128">事件按时间间隔月数在相应月份的指定一天（例如 15 号）重复发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-128">Event repeats on the specified day of the month (e.g. the 15th), based on the number of months between occurrences.</span></span> | <span data-ttu-id="f8346-129">事件每季度（每 3 个月）的 15 号重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="f8346-129">Repeat event quarterly (every 3 months) on the 15th.</span></span> | <span data-ttu-id="f8346-130">**type**、**interval**、**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="f8346-130">**type**, **interval**, **dayOfMonth**</span></span> |
| <span data-ttu-id="f8346-131">相对每月</span><span class="sxs-lookup"><span data-stu-id="f8346-131">Relative monthly</span></span> | `relativeMonthly` | <span data-ttu-id="f8346-132">事件按时间间隔月数在一周内的指定一天或几天（相应月份的同一相对位置）重复发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-132">Event repeats on the specified day or days of the week, in the same relative position in the month, based on the number of months between occurrences.</span></span> | <span data-ttu-id="f8346-133">事件每 3 个月的第二个星期四或星期五重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="f8346-133">Repeat event on the second Thursday or Friday every three months.</span></span> | <span data-ttu-id="f8346-134">**type**、**interval**、**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="f8346-134">**type**, **interval**, **daysOfWeek**</span></span> |
| <span data-ttu-id="f8346-135">绝对每年</span><span class="sxs-lookup"><span data-stu-id="f8346-135">Absolute yearly</span></span> | `absoluteYearly` | <span data-ttu-id="f8346-136">事件按时间间隔年数在指定月份的一天重复发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-136">Event repeats on the specified day and month, based on the number of years between occurrences.</span></span> | <span data-ttu-id="f8346-137">事件每 3 年在 3 月 15 日重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="f8346-137">Repeat event on the 15th of March every 3 years.</span></span> | <span data-ttu-id="f8346-138">**type**、**interval**、**dayOfMonth**、**month**</span><span class="sxs-lookup"><span data-stu-id="f8346-138">**type**, **interval**, **dayOfMonth**, **month**</span></span> |
| <span data-ttu-id="f8346-139">相对每年</span><span class="sxs-lookup"><span data-stu-id="f8346-139">Relative yearly</span></span> | `relativeYearly` | <span data-ttu-id="f8346-140">事件按时间间隔年数在一周内的指定一天或几天（相应年份和月份的同一相对位置）重复发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-140">Event repeats on the specified day or days of the week, in the same relative position in a specific month of the year, based on the number of years between occurrences.</span></span> | <span data-ttu-id="f8346-141">事件每 3 年在 11 月的第二个星期四或星期五重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="f8346-141">Repeat event on the second Thursday or Friday of every November every 3 years.</span></span> | <span data-ttu-id="f8346-142">**type**、**interval**、**daysOfWeek**、**month**</span><span class="sxs-lookup"><span data-stu-id="f8346-142">**type**, **interval**, **daysOfWeek**, **month**</span></span> |


## <a name="properties"></a><span data-ttu-id="f8346-143">属性</span><span class="sxs-lookup"><span data-stu-id="f8346-143">Properties</span></span>
| <span data-ttu-id="f8346-144">属性</span><span class="sxs-lookup"><span data-stu-id="f8346-144">Property</span></span>     | <span data-ttu-id="f8346-145">类型</span><span class="sxs-lookup"><span data-stu-id="f8346-145">Type</span></span>   |<span data-ttu-id="f8346-146">说明</span><span class="sxs-lookup"><span data-stu-id="f8346-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8346-147">dayOfMonth</span><span class="sxs-lookup"><span data-stu-id="f8346-147">dayOfMonth</span></span>|<span data-ttu-id="f8346-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f8346-148">Int32</span></span>|<span data-ttu-id="f8346-149">事件在相应月份的多少号发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-149">The day of the month on which the event occurs.</span></span> <span data-ttu-id="f8346-150">如果 **type** 为 `absoluteMonthly` 或 `absoluteYearly`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-150">Required if **type** is `absoluteMonthly` or `absoluteYearly`.</span></span> |
|<span data-ttu-id="f8346-151">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="f8346-151">daysOfWeek</span></span>|<span data-ttu-id="f8346-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8346-152">String collection</span></span>|<span data-ttu-id="f8346-153">事件在星期几（一系列值）发生。</span><span class="sxs-lookup"><span data-stu-id="f8346-153">A collection of the days of the week on which the event occurs.</span></span> <span data-ttu-id="f8346-154">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="f8346-154">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span> <br><span data-ttu-id="f8346-155">如果 **type** 为 `relativeMonthly` 或 `relativeYearly`，且 **daysOfWeek** 指定超过一天，事件遵循相应模式的第一天规则。</span><span class="sxs-lookup"><span data-stu-id="f8346-155">If **type** is `relativeMonthly` or `relativeYearly`, and **daysOfWeek** specifies more than one day, the event falls on the first day that satisfies the pattern.</span></span> <br> <span data-ttu-id="f8346-156">如果 **type** 为 `weekly`、`relativeMonthly` 或 `relativeYearly`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-156">Required if **type** is `weekly`, `relativeMonthly`, or `relativeYearly`.</span></span>|
|<span data-ttu-id="f8346-157">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="f8346-157">firstDayOfWeek</span></span>|<span data-ttu-id="f8346-158">String</span><span class="sxs-lookup"><span data-stu-id="f8346-158">String</span></span>|<span data-ttu-id="f8346-159">每周的第一天。</span><span class="sxs-lookup"><span data-stu-id="f8346-159">The first day of the week.</span></span> <span data-ttu-id="f8346-160">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="f8346-160">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span> <span data-ttu-id="f8346-161">默认值为 `sunday`。</span><span class="sxs-lookup"><span data-stu-id="f8346-161">Default is `sunday`.</span></span> <span data-ttu-id="f8346-162">如果 **type** 为 `weekly`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-162">Required if **type** is `weekly`.</span></span> |
|<span data-ttu-id="f8346-163">index</span><span class="sxs-lookup"><span data-stu-id="f8346-163">index</span></span>|<span data-ttu-id="f8346-164">String</span><span class="sxs-lookup"><span data-stu-id="f8346-164">String</span></span>|<span data-ttu-id="f8346-165">指定事件在 **daysOfsWeek** 中指定的第几个星期几实例发生，从相应月份的第一个实例开始计算。</span><span class="sxs-lookup"><span data-stu-id="f8346-165">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="f8346-166">可取值为：`first`、`second`、`third`、`fourth` 或 `last`。</span><span class="sxs-lookup"><span data-stu-id="f8346-166">Possible values are: `first`, `second`, `third`, `fourth`, `last`.</span></span> <span data-ttu-id="f8346-167">默认值为 `first`。</span><span class="sxs-lookup"><span data-stu-id="f8346-167">Default is `first`.</span></span> <span data-ttu-id="f8346-168">如果 **type** 为 `relativeMonthly` 或 `relativeYearly`，请使用此可选属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-168">Optional and used if **type** is `relativeMonthly` or `relativeYearly`.</span></span> |
|<span data-ttu-id="f8346-169">interval</span><span class="sxs-lookup"><span data-stu-id="f8346-169">interval</span></span>|<span data-ttu-id="f8346-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f8346-170">Int32</span></span>|<span data-ttu-id="f8346-171">间隔的单元数，可以是天数、周数、月数或年数，具体视 **type** 而定。</span><span class="sxs-lookup"><span data-stu-id="f8346-171">The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the **type**.</span></span> <span data-ttu-id="f8346-172">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-172">Required.</span></span> |
|<span data-ttu-id="f8346-173">month</span><span class="sxs-lookup"><span data-stu-id="f8346-173">month</span></span>|<span data-ttu-id="f8346-174">Int32</span><span class="sxs-lookup"><span data-stu-id="f8346-174">Int32</span></span>|<span data-ttu-id="f8346-175">事件发生的月份。</span><span class="sxs-lookup"><span data-stu-id="f8346-175">The month in which the event occurs.</span></span>  <span data-ttu-id="f8346-176">这是一个介于 1 到 12 之间的数字。</span><span class="sxs-lookup"><span data-stu-id="f8346-176">This is a number from 1 to 12.</span></span>|
|<span data-ttu-id="f8346-177">type</span><span class="sxs-lookup"><span data-stu-id="f8346-177">type</span></span>|<span data-ttu-id="f8346-178">String</span><span class="sxs-lookup"><span data-stu-id="f8346-178">String</span></span>|<span data-ttu-id="f8346-179">定期模式类型：`daily`、`weekly`、`absoluteMonthly`、`relativeMonthly`、`absoluteYearly` 或 `relativeYearly`。</span><span class="sxs-lookup"><span data-stu-id="f8346-179">The recurrence pattern type: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`.</span></span> <span data-ttu-id="f8346-180">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-180">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8346-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8346-181">JSON representation</span></span>

<span data-ttu-id="f8346-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8346-182">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


