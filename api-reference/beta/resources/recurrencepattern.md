---
title: recurrencePattern 资源类型
description: 描述了定期事件的重复发生频率。
localization_priority: Normal
ms.openlocfilehash: 4798ce7fc33fd6dec7aec1b8c333ae66c917e373
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512260"
---
# <a name="recurrencepattern-resource-type"></a><span data-ttu-id="0303f-103">recurrencePattern 资源类型</span><span class="sxs-lookup"><span data-stu-id="0303f-103">recurrencePattern resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0303f-104">描述了定期[事件](event.md)的重复发生频率。</span><span class="sxs-lookup"><span data-stu-id="0303f-104">Describes the frequency by which a recurring [event](event.md) repeats.</span></span>

<span data-ttu-id="0303f-105">可以使用下面的 6 种方法之一（具体视方案而定），指定定期事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="0303f-105">You can specify the recurrence pattern of a recurring event in one of 6 ways depending on your scenario.</span></span> <span data-ttu-id="0303f-106">对于每种类型的模式，请指定时间间隔。</span><span class="sxs-lookup"><span data-stu-id="0303f-106">For each pattern type, specify the amount of time between occurrences.</span></span> <span data-ttu-id="0303f-107">在为事件指定的日期范围内，实际发生的定期事件始终遵循此模式。</span><span class="sxs-lookup"><span data-stu-id="0303f-107">The actual occurrences of the recurring event always follow this pattern falling within the date range that you specify for the event.</span></span> <span data-ttu-id="0303f-108">定期事件始终由 **recurrencePattern**（事件的重复发生频率）和 [recurrenceRange](recurrencerange.md)（事件在哪个日期范围内重复发生）进行定义。</span><span class="sxs-lookup"><span data-stu-id="0303f-108">A recurring event is always defined by its **recurrencePattern** (how frequently the event repeats), and its [recurrenceRange](recurrencerange.md) (over how long the event repeats).</span></span>

<span data-ttu-id="0303f-109">**type** 属性可用于指定不同类型的 **recurrencePattern**，**interval** 属性可用于指定时间间隔，可以是天数、周数、月数或年数，具体视 **type** 而定。</span><span class="sxs-lookup"><span data-stu-id="0303f-109">Use the **type** property to specify the different types of **recurrencePattern**, and the **interval** property to specify the time between occurrences, which can be in number of days, weeks, months, or years, depending on the **type**.</span></span> <span data-ttu-id="0303f-110">请注意每种类型的必需属性，如下表所述。</span><span class="sxs-lookup"><span data-stu-id="0303f-110">Note which properties are required for each type, as described in the following table.</span></span>

> <span data-ttu-id="0303f-111">**注意**：仅添加定期模式需要的属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-111">**Note** Include only the properties that you need for a recurrence pattern.</span></span> <span data-ttu-id="0303f-112">如果添加的任何属性没有受支持的值，则会引发错误。</span><span class="sxs-lookup"><span data-stu-id="0303f-112">Any property that you include that does not have a supported value would result in an error.</span></span>

| <span data-ttu-id="0303f-113">定期模式类型</span><span class="sxs-lookup"><span data-stu-id="0303f-113">Type of recurrence pattern</span></span> | <span data-ttu-id="0303f-114">type 属性值</span><span class="sxs-lookup"><span data-stu-id="0303f-114">Value of type property</span></span> | <span data-ttu-id="0303f-115">说明</span><span class="sxs-lookup"><span data-stu-id="0303f-115">Description</span></span> | <span data-ttu-id="0303f-116">示例</span><span class="sxs-lookup"><span data-stu-id="0303f-116">Example</span></span> | <span data-ttu-id="0303f-117">必需属性</span><span class="sxs-lookup"><span data-stu-id="0303f-117">Required properties</span></span> |
|:---------------|:--------|:--------|:--------|:----------|
| <span data-ttu-id="0303f-118">每天</span><span class="sxs-lookup"><span data-stu-id="0303f-118">Daily</span></span> | `daily` | <span data-ttu-id="0303f-119">事件按 **interval** 指定的时间间隔天数重复发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-119">Event repeats based on the number of days specified by **interval** between occurrences.</span></span> | <span data-ttu-id="0303f-120">事件每 3 天重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="0303f-120">Repeat event every 3 days.</span></span> | <span data-ttu-id="0303f-121">**type**、**interval**</span><span class="sxs-lookup"><span data-stu-id="0303f-121">**type**, **interval**</span></span> |
| <span data-ttu-id="0303f-122">每周</span><span class="sxs-lookup"><span data-stu-id="0303f-122">Weekly</span></span> | `weekly` | <span data-ttu-id="0303f-123">事件按时间间隔周数在一周内的一天或几天重复发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-123">Event repeats on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span> | <span data-ttu-id="0303f-124">事件每两个星期一和星期二重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="0303f-124">Repeat event Monday and Tuesday of every other week.</span></span> | <span data-ttu-id="0303f-125">**type**、**interval**、**daysOfWeek**、**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0303f-125">**type**, **interval**, **daysOfWeek**, **firstDayOfWeek**</span></span> |
| <span data-ttu-id="0303f-126">绝对每月</span><span class="sxs-lookup"><span data-stu-id="0303f-126">Absolute monthly</span></span> | `absoluteMonthly` | <span data-ttu-id="0303f-127">事件按时间间隔月数在相应月份的指定一天（例如 15 号）重复发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-127">Event repeats on the specified day of the month (e.g. the 15th), based on the number of months between occurrences.</span></span> | <span data-ttu-id="0303f-128">事件每季度（每 3 个月）的 15 号重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="0303f-128">Repeat event quarterly (every 3 months) on the 15th.</span></span> | <span data-ttu-id="0303f-129">**type**、**interval**、**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="0303f-129">**type**, **interval**, **dayOfMonth**</span></span> |
| <span data-ttu-id="0303f-130">相对每月</span><span class="sxs-lookup"><span data-stu-id="0303f-130">Relative monthly</span></span> | `relativeMonthly` | <span data-ttu-id="0303f-131">事件按时间间隔月数在一周内的指定一天或几天（相应月份的同一相对位置）重复发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-131">Event repeats on the specified day or days of the week, in the same relative position in the month, based on the number of months between occurrences.</span></span> | <span data-ttu-id="0303f-132">事件每 3 个月的第二个星期四或星期五重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="0303f-132">Repeat event on the second Thursday or Friday every three months.</span></span> | <span data-ttu-id="0303f-133">**type**、**interval**、**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="0303f-133">**type**, **interval**, **daysOfWeek**</span></span> |
| <span data-ttu-id="0303f-134">绝对每年</span><span class="sxs-lookup"><span data-stu-id="0303f-134">Absolute yearly</span></span> | `absoluteYearly` | <span data-ttu-id="0303f-135">事件按时间间隔年数在指定月份的一天重复发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-135">Event repeats on the specified day and month, based on the number of years between occurrences.</span></span> | <span data-ttu-id="0303f-136">事件每 3 年在 3 月 15 日重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="0303f-136">Repeat event on the 15th of March every 3 years.</span></span> | <span data-ttu-id="0303f-137">**type**、**interval**、**dayOfMonth**、**month**</span><span class="sxs-lookup"><span data-stu-id="0303f-137">**type**, **interval**, **dayOfMonth**, **month**</span></span> |
| <span data-ttu-id="0303f-138">相对每年</span><span class="sxs-lookup"><span data-stu-id="0303f-138">Relative yearly</span></span> | `relativeYearly` | <span data-ttu-id="0303f-139">事件按时间间隔年数在一周内的指定一天或几天（相应年份和月份的同一相对位置）重复发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-139">Event repeats on the specified day or days of the week, in the same relative position in a specific month of the year, based on the number of years between occurrences.</span></span> | <span data-ttu-id="0303f-140">事件每 3 年在 11 月的第二个星期四或星期五重复发生一次。</span><span class="sxs-lookup"><span data-stu-id="0303f-140">Repeat event on the second Thursday or Friday of every November every 3 years.</span></span> | <span data-ttu-id="0303f-141">**type**、**interval**、**daysOfWeek**、**month**</span><span class="sxs-lookup"><span data-stu-id="0303f-141">**type**, **interval**, **daysOfWeek**, **month**</span></span> |


## <a name="properties"></a><span data-ttu-id="0303f-142">属性</span><span class="sxs-lookup"><span data-stu-id="0303f-142">Properties</span></span>
| <span data-ttu-id="0303f-143">属性</span><span class="sxs-lookup"><span data-stu-id="0303f-143">Property</span></span>     | <span data-ttu-id="0303f-144">类型</span><span class="sxs-lookup"><span data-stu-id="0303f-144">Type</span></span>   |<span data-ttu-id="0303f-145">说明</span><span class="sxs-lookup"><span data-stu-id="0303f-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0303f-146">dayOfMonth</span><span class="sxs-lookup"><span data-stu-id="0303f-146">dayOfMonth</span></span>|<span data-ttu-id="0303f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0303f-147">Int32</span></span>|<span data-ttu-id="0303f-148">事件在相应月份的多少号发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-148">The day of the month on which the event occurs.</span></span> <span data-ttu-id="0303f-149">如果 **type** 为 `absoluteMonthly` 或 `absoluteYearly`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-149">Required if **type** is `absoluteMonthly` or `absoluteYearly`.</span></span> |
|<span data-ttu-id="0303f-150">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="0303f-150">daysOfWeek</span></span>|<span data-ttu-id="0303f-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="0303f-151">String collection</span></span>|<span data-ttu-id="0303f-152">事件在星期几（一系列值）发生。</span><span class="sxs-lookup"><span data-stu-id="0303f-152">A collection of the days of the week on which the event occurs.</span></span> <span data-ttu-id="0303f-153">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="0303f-153">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span> <br><span data-ttu-id="0303f-154">如果 **type** 为 `relativeMonthly` 或 `relativeYearly`，且 **daysOfWeek** 指定超过一天，事件遵循相应模式的第一天规则。</span><span class="sxs-lookup"><span data-stu-id="0303f-154">If **type** is `relativeMonthly` or `relativeYearly`, and **daysOfWeek** specifies more than one day, the event falls on the first day that satisfies the pattern.</span></span> <br> <span data-ttu-id="0303f-155">如果 **type** 为 `weekly`、`relativeMonthly` 或 `relativeYearly`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-155">Required if **type** is `weekly`, `relativeMonthly`, or `relativeYearly`.</span></span>|
|<span data-ttu-id="0303f-156">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0303f-156">firstDayOfWeek</span></span>|<span data-ttu-id="0303f-157">String</span><span class="sxs-lookup"><span data-stu-id="0303f-157">String</span></span>|<span data-ttu-id="0303f-158">每周的第一天。</span><span class="sxs-lookup"><span data-stu-id="0303f-158">The first day of the week.</span></span> <span data-ttu-id="0303f-159">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="0303f-159">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span> <span data-ttu-id="0303f-160">默认值为 `sunday`。</span><span class="sxs-lookup"><span data-stu-id="0303f-160">Default is `sunday`.</span></span> <span data-ttu-id="0303f-161">如果 **type** 为 `weekly`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-161">Required if **type** is `weekly`.</span></span> |
|<span data-ttu-id="0303f-162">index</span><span class="sxs-lookup"><span data-stu-id="0303f-162">index</span></span>|<span data-ttu-id="0303f-163">String</span><span class="sxs-lookup"><span data-stu-id="0303f-163">String</span></span>|<span data-ttu-id="0303f-164">指定事件在 **daysOfsWeek** 中指定的第几个星期几实例发生，从相应月份的第一个实例开始计算。</span><span class="sxs-lookup"><span data-stu-id="0303f-164">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="0303f-165">可取值为：`first`、`second`、`third`、`fourth` 或 `last`。</span><span class="sxs-lookup"><span data-stu-id="0303f-165">Possible values are: `first`, `second`, `third`, `fourth`, `last`.</span></span> <span data-ttu-id="0303f-166">默认值为 `first`。</span><span class="sxs-lookup"><span data-stu-id="0303f-166">Default is `first`.</span></span> <span data-ttu-id="0303f-167">如果 **type** 为 `relativeMonthly` 或 `relativeYearly`，请使用此可选属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-167">Optional and used if **type** is `relativeMonthly` or `relativeYearly`.</span></span> |
|<span data-ttu-id="0303f-168">interval</span><span class="sxs-lookup"><span data-stu-id="0303f-168">interval</span></span>|<span data-ttu-id="0303f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0303f-169">Int32</span></span>|<span data-ttu-id="0303f-170">间隔的单元数，可以是天数、周数、月数或年数，具体视 **type** 而定。</span><span class="sxs-lookup"><span data-stu-id="0303f-170">The number of units between occurrences, where units can be in days, weeks, months, or years, depending on the **type**.</span></span> <span data-ttu-id="0303f-171">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-171">Required.</span></span> |
|<span data-ttu-id="0303f-172">month</span><span class="sxs-lookup"><span data-stu-id="0303f-172">month</span></span>|<span data-ttu-id="0303f-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0303f-173">Int32</span></span>|<span data-ttu-id="0303f-174">事件发生的月份。</span><span class="sxs-lookup"><span data-stu-id="0303f-174">The month in which the event occurs.</span></span>  <span data-ttu-id="0303f-175">这是一个介于 1 到 12 之间的数字。</span><span class="sxs-lookup"><span data-stu-id="0303f-175">This is a number from 1 to 12.</span></span>|
|<span data-ttu-id="0303f-176">type</span><span class="sxs-lookup"><span data-stu-id="0303f-176">type</span></span>|<span data-ttu-id="0303f-177">字符串</span><span class="sxs-lookup"><span data-stu-id="0303f-177">String</span></span>|<span data-ttu-id="0303f-178">定期模式类型：`daily`、`weekly`、`absoluteMonthly`、`relativeMonthly`、`absoluteYearly` 或 `relativeYearly`。</span><span class="sxs-lookup"><span data-stu-id="0303f-178">The recurrence pattern type: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`.</span></span> <span data-ttu-id="0303f-179">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="0303f-179">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0303f-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0303f-180">JSON representation</span></span>

<span data-ttu-id="0303f-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0303f-181">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/recurrencepattern.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
