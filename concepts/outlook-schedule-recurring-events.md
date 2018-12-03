---
title: 在 Outlook 中将重复约会安排为定期事件
description: 定期事件是 Outlook 日历的重要组成部分。 无论是与经理每周进行的一对一会议，还是每月第二个星期二的部门评审会议，定期规则只需要创建一次事件，然后让服务器填充系列中的其他内容，从而使过程变得简单。
ms.openlocfilehash: 1af082a32d79f6011e93a7fc0c5fc9d553d16712
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091759"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="6ea56-104">在 Outlook 中将重复约会安排为定期事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-104">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="6ea56-105">定期事件是 Outlook 日历的重要组成部分。</span><span class="sxs-lookup"><span data-stu-id="6ea56-105">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="6ea56-106">无论是与经理每周进行的一对一会议，还是每月第二个星期二的部门评审会议，定期规则只需要创建一次事件，然后让服务器填充系列中的其他内容，从而使过程变得简单。</span><span class="sxs-lookup"><span data-stu-id="6ea56-106">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="6ea56-107">使定期事件得以“扩展”为单个事件的关键信息点在于定期规则。</span><span class="sxs-lookup"><span data-stu-id="6ea56-107">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="6ea56-108">此规则同时指定事件重复的频率和持续时间。</span><span class="sxs-lookup"><span data-stu-id="6ea56-108">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="6ea56-109">Outlook REST API 在[事件资源](/graph/api/resources/event?view=graph-rest-1.0)的**重复周期**属性中模拟定期规则。</span><span class="sxs-lookup"><span data-stu-id="6ea56-109">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> 

<span data-ttu-id="6ea56-110">每个重复周期由两部分组成：定期模式（频率）和定期范围（持续时间）。</span><span class="sxs-lookup"><span data-stu-id="6ea56-110">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="6ea56-111">定期模式</span><span class="sxs-lookup"><span data-stu-id="6ea56-111">Recurrence patterns</span></span>

<span data-ttu-id="6ea56-112">重复的第一部分是模式。</span><span class="sxs-lookup"><span data-stu-id="6ea56-112">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="6ea56-113">它指定事件重复的频率。</span><span class="sxs-lookup"><span data-stu-id="6ea56-113">This specifies how often the event repeats.</span></span> <span data-ttu-id="6ea56-114">例如，一个事件可以“每 3 天”、“每周四”或“每年的 7 月 22 日”重复一次。</span><span class="sxs-lookup"><span data-stu-id="6ea56-114">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="6ea56-115">在 API 中，模式由 [recurrencePattern 资源](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)表示。</span><span class="sxs-lookup"><span data-stu-id="6ea56-115">A pattern is represented in the API by the [recurrencePattern resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="6ea56-116">**recurrencePattern** 的特定字段是必需、可选还是忽略取决于模式的类型。</span><span class="sxs-lookup"><span data-stu-id="6ea56-116">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="6ea56-117">**注意**：即使将字段忽略，仍需验证该字段。</span><span class="sxs-lookup"><span data-stu-id="6ea56-117">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="6ea56-118">如果字段包含一组可能值的列表，那么使用允许集以外的值会导致错误，即使此字段已被忽略也是如此。</span><span class="sxs-lookup"><span data-stu-id="6ea56-118">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="6ea56-119">让我们来看看每个可能的模式类型。</span><span class="sxs-lookup"><span data-stu-id="6ea56-119">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="6ea56-120">每天</span><span class="sxs-lookup"><span data-stu-id="6ea56-120">Daily</span></span>

<span data-ttu-id="6ea56-121">每天定期模式会导致事件基于每次事件之间的天数重复。</span><span class="sxs-lookup"><span data-stu-id="6ea56-121">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-122">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-122">Relevant properties</span></span>

| <span data-ttu-id="6ea56-123">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-123">Property</span></span> | <span data-ttu-id="6ea56-124">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-124">Relevance</span></span> | <span data-ttu-id="6ea56-125">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-125">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-126">**interval**</span><span class="sxs-lookup"><span data-stu-id="6ea56-126">**interval**</span></span> | <span data-ttu-id="6ea56-127">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-127">Required</span></span> | <span data-ttu-id="6ea56-128">指定每次事件之间的天数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-128">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="6ea56-129">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-129">**type**</span></span> | <span data-ttu-id="6ea56-130">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-130">Required</span></span> | <span data-ttu-id="6ea56-131">必须设置为 `daily`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-131">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-132">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-132">Examples</span></span>

- <span data-ttu-id="6ea56-133">每天重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-133">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="6ea56-134">每三天重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-134">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="6ea56-135">每周</span><span class="sxs-lookup"><span data-stu-id="6ea56-135">Weekly</span></span>

<span data-ttu-id="6ea56-136">每周定期模式使事件基于每组事件之间的周数，在每周的同一天或几天重复。</span><span class="sxs-lookup"><span data-stu-id="6ea56-136">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-137">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-137">Relevant properties</span></span>

| <span data-ttu-id="6ea56-138">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-138">Property</span></span> | <span data-ttu-id="6ea56-139">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-139">Relevance</span></span> | <span data-ttu-id="6ea56-140">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-140">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-141">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="6ea56-141">**daysOfWeek**</span></span> | <span data-ttu-id="6ea56-142">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-142">Required</span></span> | <span data-ttu-id="6ea56-143">指定事件发生在每周的哪一天/哪几天。</span><span class="sxs-lookup"><span data-stu-id="6ea56-143">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="6ea56-144">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="6ea56-144">**firstDayOfWeek**</span></span> | <span data-ttu-id="6ea56-145">可选</span><span class="sxs-lookup"><span data-stu-id="6ea56-145">Optional</span></span> | <span data-ttu-id="6ea56-146">指定将哪一天视为一周的第一天。</span><span class="sxs-lookup"><span data-stu-id="6ea56-146">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="6ea56-147">默认值为：`Sunday`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-147">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="6ea56-148">**interval**</span><span class="sxs-lookup"><span data-stu-id="6ea56-148">**interval**</span></span> | <span data-ttu-id="6ea56-149">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-149">Required</span></span> | <span data-ttu-id="6ea56-150">指定每组事件之间的周数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-150">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="6ea56-151">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-151">**type**</span></span> | <span data-ttu-id="6ea56-152">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-152">Required</span></span> | <span data-ttu-id="6ea56-153">必须设置为 `weekly`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-153">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-154">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-154">Examples</span></span>

- <span data-ttu-id="6ea56-155">每周四重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-155">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="6ea56-156">每隔一个周一和周二重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-156">Repeat this event every other Monday and Tuesday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a><span data-ttu-id="6ea56-157">绝对每月</span><span class="sxs-lookup"><span data-stu-id="6ea56-157">Absolute monthly</span></span>

<span data-ttu-id="6ea56-158">绝对每月模式使事件在每个月的同一天（例如，15日）重复，它基于每次事件之间的月数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-158">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-159">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-159">Relevant properties</span></span>

| <span data-ttu-id="6ea56-160">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-160">Property</span></span> | <span data-ttu-id="6ea56-161">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-161">Relevance</span></span> | <span data-ttu-id="6ea56-162">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-162">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-163">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="6ea56-163">**dayOfMonth**</span></span> | <span data-ttu-id="6ea56-164">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-164">Required</span></span> | <span data-ttu-id="6ea56-165">指定事件发生在每月的哪一天。</span><span class="sxs-lookup"><span data-stu-id="6ea56-165">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="6ea56-166">**interval**</span><span class="sxs-lookup"><span data-stu-id="6ea56-166">**interval**</span></span> | <span data-ttu-id="6ea56-167">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-167">Required</span></span> | <span data-ttu-id="6ea56-168">指定每次事件之间的月数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-168">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="6ea56-169">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-169">**type**</span></span> | <span data-ttu-id="6ea56-170">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-170">Required</span></span> | <span data-ttu-id="6ea56-171">必须设置为 `absoluteMonthly`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-171">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-172">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-172">Examples</span></span>

- <span data-ttu-id="6ea56-173">在每月的 15 号重复此事件。</span><span class="sxs-lookup"><span data-stu-id="6ea56-173">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="6ea56-174">按季度（每 3 个月）在 7 号重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-174">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="6ea56-175">相对每月</span><span class="sxs-lookup"><span data-stu-id="6ea56-175">Relative monthly</span></span>

<span data-ttu-id="6ea56-176">相对每月模式使事件基于每次事件之间的月数，在每个月同一相对位置中每周的同一天重复。</span><span class="sxs-lookup"><span data-stu-id="6ea56-176">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="6ea56-177">例如，“每月的第二个星期三”。</span><span class="sxs-lookup"><span data-stu-id="6ea56-177">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-178">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-178">Relevant properties</span></span>

| <span data-ttu-id="6ea56-179">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-179">Property</span></span> | <span data-ttu-id="6ea56-180">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-180">Relevance</span></span> | <span data-ttu-id="6ea56-181">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-181">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-182">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="6ea56-182">**daysOfWeek**</span></span> | <span data-ttu-id="6ea56-183">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-183">Required</span></span> | <span data-ttu-id="6ea56-184">指定事件发生在一周的哪一天/哪几天。</span><span class="sxs-lookup"><span data-stu-id="6ea56-184">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="6ea56-185">相对每月事件每月仅发生一次，因此，如果指定多个值，事件会在满足模式的第一天发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-185">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="6ea56-186">**index**</span><span class="sxs-lookup"><span data-stu-id="6ea56-186">**index**</span></span> | <span data-ttu-id="6ea56-187">可选</span><span class="sxs-lookup"><span data-stu-id="6ea56-187">Optional</span></span> | <span data-ttu-id="6ea56-188">指定事件在 **daysOfsWeek** 中指定的允许天数的哪个实例上发生，从当月的第一个实例开始计数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-188">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="6ea56-189">可能的值是：`first`、`second`、`third`、`fourth` 和 `last`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-189">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="6ea56-190">默认值为：`first`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-190">Default value: `first`.</span></span> |
| <span data-ttu-id="6ea56-191">**interval**</span><span class="sxs-lookup"><span data-stu-id="6ea56-191">**interval**</span></span> | <span data-ttu-id="6ea56-192">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-192">Required</span></span> | <span data-ttu-id="6ea56-193">指定每次事件之间的月数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-193">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="6ea56-194">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-194">**type**</span></span> | <span data-ttu-id="6ea56-195">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-195">Required</span></span> | <span data-ttu-id="6ea56-196">必须设置为 `relativeMonthly`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-196">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-197">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-197">Examples</span></span>

- <span data-ttu-id="6ea56-198">在每月的第二个星期三重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-198">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="6ea56-199">在每月的第一个星期四或星期五重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-199">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="6ea56-200">绝对每年</span><span class="sxs-lookup"><span data-stu-id="6ea56-200">Absolute yearly</span></span>

<span data-ttu-id="6ea56-201">绝对每年模式使事件在每年的同一月份的同一天（例如，4 月 15 日）重复，它基于每次事件之间的年数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-201">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-202">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-202">Relevant properties</span></span>

| <span data-ttu-id="6ea56-203">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-203">Property</span></span> | <span data-ttu-id="6ea56-204">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-204">Relevance</span></span> | <span data-ttu-id="6ea56-205">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-205">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-206">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="6ea56-206">**dayOfMonth**</span></span> | <span data-ttu-id="6ea56-207">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-207">Required</span></span> | <span data-ttu-id="6ea56-208">指定事件发生在每月的哪一天。</span><span class="sxs-lookup"><span data-stu-id="6ea56-208">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="6ea56-209">**month**</span><span class="sxs-lookup"><span data-stu-id="6ea56-209">**month**</span></span> | <span data-ttu-id="6ea56-210">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-210">Required</span></span> | <span data-ttu-id="6ea56-211">指定事件发生的月份。</span><span class="sxs-lookup"><span data-stu-id="6ea56-211">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="6ea56-212">**interval**</span><span class="sxs-lookup"><span data-stu-id="6ea56-212">**interval**</span></span> | <span data-ttu-id="6ea56-213">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-213">Required</span></span> | <span data-ttu-id="6ea56-214">指定每次事件之间的年数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-214">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="6ea56-215">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-215">**type**</span></span> | <span data-ttu-id="6ea56-216">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-216">Required</span></span> | <span data-ttu-id="6ea56-217">必须设置为 `absoluteYearly`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-217">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="6ea56-218">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-218">Example</span></span>

- <span data-ttu-id="6ea56-219">在每年的 4 月 15 日重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-219">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="6ea56-220">相对每年</span><span class="sxs-lookup"><span data-stu-id="6ea56-220">Relative yearly</span></span>

<span data-ttu-id="6ea56-221">相对每年模式使事件基于每次事件之间的年数，在特定月份同一相对位置中每周的同一天重复。</span><span class="sxs-lookup"><span data-stu-id="6ea56-221">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="6ea56-222">例如，“每个 11 月的最后一个星期三”。</span><span class="sxs-lookup"><span data-stu-id="6ea56-222">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-223">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-223">Relevant properties</span></span>

| <span data-ttu-id="6ea56-224">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-224">Property</span></span> | <span data-ttu-id="6ea56-225">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-225">Relevance</span></span> | <span data-ttu-id="6ea56-226">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-226">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-227">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="6ea56-227">**daysOfWeek**</span></span> | <span data-ttu-id="6ea56-228">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-228">Required</span></span> | <span data-ttu-id="6ea56-229">指定事件发生在一周的哪一天/哪几天。</span><span class="sxs-lookup"><span data-stu-id="6ea56-229">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="6ea56-230">相对每年事件每年仅发生一次，因此，如果指定多个值，事件会在满足模式的第一天发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-230">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="6ea56-231">**index**</span><span class="sxs-lookup"><span data-stu-id="6ea56-231">**index**</span></span> | <span data-ttu-id="6ea56-232">可选</span><span class="sxs-lookup"><span data-stu-id="6ea56-232">Optional</span></span> | <span data-ttu-id="6ea56-233">指定事件在 **daysOfsWeek** 中指定的允许天数的哪个实例上发生，从当月的第一个实例开始计数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-233">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="6ea56-234">可能的值是：`first`、`second`、`third`、`fourth` 和 `last`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-234">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="6ea56-235">默认值为：`first`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-235">Default value: `first`.</span></span> |
| <span data-ttu-id="6ea56-236">**month**</span><span class="sxs-lookup"><span data-stu-id="6ea56-236">**month**</span></span> | <span data-ttu-id="6ea56-237">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-237">Required</span></span> | <span data-ttu-id="6ea56-238">指定事件发生的月份。</span><span class="sxs-lookup"><span data-stu-id="6ea56-238">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="6ea56-239">**interval**</span><span class="sxs-lookup"><span data-stu-id="6ea56-239">**interval**</span></span> | <span data-ttu-id="6ea56-240">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-240">Required</span></span> | <span data-ttu-id="6ea56-241">指定每次事件之间的年数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-241">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="6ea56-242">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-242">**type**</span></span> | <span data-ttu-id="6ea56-243">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-243">Required</span></span> | <span data-ttu-id="6ea56-244">必须设置为 `relativeMonthly`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-244">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-245">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-245">Examples</span></span>

- <span data-ttu-id="6ea56-246">每年 11 月的最后一个星期三重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-246">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="6ea56-247">定期范围</span><span class="sxs-lookup"><span data-stu-id="6ea56-247">Recurrence ranges</span></span>

<span data-ttu-id="6ea56-248">重复的第二部分是范围。</span><span class="sxs-lookup"><span data-stu-id="6ea56-248">The second part of a recurrence is the range.</span></span> <span data-ttu-id="6ea56-249">它指定模式重复的持续时间。</span><span class="sxs-lookup"><span data-stu-id="6ea56-249">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="6ea56-250">例如，一个事件可以在发生 10 次后于特定日期结束，也可以不结束。</span><span class="sxs-lookup"><span data-stu-id="6ea56-250">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="6ea56-251">在 API 中，由 [recurrenceRange 资源](/graph/api/resources/recurrencepattern?view=graph-rest-1.0)表示范围。</span><span class="sxs-lookup"><span data-stu-id="6ea56-251">A range is represented in the API by the [recurrenceRange resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="6ea56-252">**recurrenceRange** 的特定字段是必需还是忽略取决于范围的类型。</span><span class="sxs-lookup"><span data-stu-id="6ea56-252">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="6ea56-253">**注意**：即使将字段忽略，仍需验证该字段。</span><span class="sxs-lookup"><span data-stu-id="6ea56-253">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="6ea56-254">如果字段包含一组可能值的列表，那么使用允许集以外的值会导致错误，即使此字段已被忽略也是如此。</span><span class="sxs-lookup"><span data-stu-id="6ea56-254">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="6ea56-255">让我们来看看每个可能的范围类型。</span><span class="sxs-lookup"><span data-stu-id="6ea56-255">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="6ea56-256">编号的范围</span><span class="sxs-lookup"><span data-stu-id="6ea56-256">Numbered range</span></span>

<span data-ttu-id="6ea56-257">编号的范围使事件（基于模式）从开始日期起按固定次数发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-257">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-258">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-258">Relevant properties</span></span>

| <span data-ttu-id="6ea56-259">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-259">Property</span></span> | <span data-ttu-id="6ea56-260">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-260">Relevance</span></span> | <span data-ttu-id="6ea56-261">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-261">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-262">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="6ea56-262">**numberOfOccurences**</span></span> | <span data-ttu-id="6ea56-263">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-263">Required</span></span> | <span data-ttu-id="6ea56-264">指定事件发生的次数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-264">Specifies the number of occurrences.</span></span> <span data-ttu-id="6ea56-265">必须是正整数。</span><span class="sxs-lookup"><span data-stu-id="6ea56-265">Must be a positive integer.</span></span> |
| <span data-ttu-id="6ea56-266">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6ea56-266">**recurrenceTimeZone**</span></span> | <span data-ttu-id="6ea56-267">可选</span><span class="sxs-lookup"><span data-stu-id="6ea56-267">Optional</span></span> | <span data-ttu-id="6ea56-268">指定 **startDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="6ea56-268">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="6ea56-269">如果未指定，将使用事件时区。</span><span class="sxs-lookup"><span data-stu-id="6ea56-269">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="6ea56-270">**startDate**</span><span class="sxs-lookup"><span data-stu-id="6ea56-270">**startDate**</span></span> | <span data-ttu-id="6ea56-271">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-271">Required</span></span> | <span data-ttu-id="6ea56-272">指定开始应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="6ea56-272">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="6ea56-273">**startDate** 的值必须与[事件资源](/graph/api/resources/event?view=graph-rest-1.0)上的 **start** 属性的日期值对应。</span><span class="sxs-lookup"><span data-stu-id="6ea56-273">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="6ea56-274">请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-274">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="6ea56-275">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-275">**type**</span></span> | <span data-ttu-id="6ea56-276">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-276">Required</span></span> | <span data-ttu-id="6ea56-277">必须设置为 `numbered`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-277">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-278">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-278">Examples</span></span>

- <span data-ttu-id="6ea56-279">此事件重复 10 次</span><span class="sxs-lookup"><span data-stu-id="6ea56-279">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="6ea56-280">结束日期范围</span><span class="sxs-lookup"><span data-stu-id="6ea56-280">End date range</span></span>

<span data-ttu-id="6ea56-281">结束日期范围使事件在开始日期和结束日期之间匹配适用模式的所有天数发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-281">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-282">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-282">Relevant properties</span></span>

| <span data-ttu-id="6ea56-283">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-283">Property</span></span> | <span data-ttu-id="6ea56-284">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-284">Relevance</span></span> | <span data-ttu-id="6ea56-285">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-285">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-286">**endDate**</span><span class="sxs-lookup"><span data-stu-id="6ea56-286">**endDate**</span></span> | <span data-ttu-id="6ea56-287">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-287">Required</span></span> | <span data-ttu-id="6ea56-288">指定停止应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="6ea56-288">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="6ea56-289">请注意，如果日期不符合模式，最后一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-289">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="6ea56-290">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6ea56-290">**recurrenceTimeZone**</span></span> | <span data-ttu-id="6ea56-291">可选</span><span class="sxs-lookup"><span data-stu-id="6ea56-291">Optional</span></span> | <span data-ttu-id="6ea56-292">指定 **startDate** 和 **endDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="6ea56-292">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="6ea56-293">如果未指定，将使用事件时区。</span><span class="sxs-lookup"><span data-stu-id="6ea56-293">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="6ea56-294">**startDate**</span><span class="sxs-lookup"><span data-stu-id="6ea56-294">**startDate**</span></span> | <span data-ttu-id="6ea56-295">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-295">Required</span></span> | <span data-ttu-id="6ea56-296">指定开始应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="6ea56-296">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="6ea56-297">**startDate** 的值必须与[事件资源](/graph/api/resources/event?view=graph-rest-1.0)上的 **start** 属性的日期值对应。</span><span class="sxs-lookup"><span data-stu-id="6ea56-297">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="6ea56-298">请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-298">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="6ea56-299">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-299">**type**</span></span> | <span data-ttu-id="6ea56-300">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-300">Required</span></span> | <span data-ttu-id="6ea56-301">必须设置为 **endDate**。</span><span class="sxs-lookup"><span data-stu-id="6ea56-301">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-302">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-302">Examples</span></span>

- <span data-ttu-id="6ea56-303">从 2017 年 7 月 1 日到 2017 年 7 月 31 日重复此事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-303">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="6ea56-304">无结束范围</span><span class="sxs-lookup"><span data-stu-id="6ea56-304">No end range</span></span>

<span data-ttu-id="6ea56-305">无结束区域使事件在开始日期后匹配适用模式的所有天数发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-305">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="6ea56-306">相关属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-306">Relevant properties</span></span>

| <span data-ttu-id="6ea56-307">属性</span><span class="sxs-lookup"><span data-stu-id="6ea56-307">Property</span></span> | <span data-ttu-id="6ea56-308">相关性</span><span class="sxs-lookup"><span data-stu-id="6ea56-308">Relevance</span></span> | <span data-ttu-id="6ea56-309">说明</span><span class="sxs-lookup"><span data-stu-id="6ea56-309">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="6ea56-310">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6ea56-310">**recurrenceTimeZone**</span></span> | <span data-ttu-id="6ea56-311">可选</span><span class="sxs-lookup"><span data-stu-id="6ea56-311">Optional</span></span> | <span data-ttu-id="6ea56-312">指定 **startDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="6ea56-312">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="6ea56-313">如果未指定，将使用事件时区。</span><span class="sxs-lookup"><span data-stu-id="6ea56-313">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="6ea56-314">**startDate**</span><span class="sxs-lookup"><span data-stu-id="6ea56-314">**startDate**</span></span> | <span data-ttu-id="6ea56-315">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-315">Required</span></span> | <span data-ttu-id="6ea56-316">指定开始应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="6ea56-316">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="6ea56-317">**startDate** 的值必须与[事件资源](/graph/api/resources/event?view=graph-rest-1.0)上的 **start** 属性的日期值对应。</span><span class="sxs-lookup"><span data-stu-id="6ea56-317">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="6ea56-318">请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-318">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="6ea56-319">**type**</span><span class="sxs-lookup"><span data-stu-id="6ea56-319">**type**</span></span> | <span data-ttu-id="6ea56-320">必需</span><span class="sxs-lookup"><span data-stu-id="6ea56-320">Required</span></span> | <span data-ttu-id="6ea56-321">必须设置为 `noEnd`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-321">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="6ea56-322">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-322">Examples</span></span>

- <span data-ttu-id="6ea56-323">从 2017 年 5 月 15 日起重复此事件，无结束日期</span><span class="sxs-lookup"><span data-stu-id="6ea56-323">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="6ea56-324">使用模式和范围创建定期事件</span><span class="sxs-lookup"><span data-stu-id="6ea56-324">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="6ea56-325">我们已经分别查看了模式和范围，让我们再来了解一下它们如何协同工作以及如何与事件中的 **start** 和 **end** 属性交互。</span><span class="sxs-lookup"><span data-stu-id="6ea56-325">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="6ea56-326">创建定期规则</span><span class="sxs-lookup"><span data-stu-id="6ea56-326">Creating a recurrence rule</span></span>

<span data-ttu-id="6ea56-327">如要创建定期规则，必须同时指定模式和范围。</span><span class="sxs-lookup"><span data-stu-id="6ea56-327">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="6ea56-328">模式类型与范围类型可任意搭配使用。</span><span class="sxs-lookup"><span data-stu-id="6ea56-328">Any pattern type can work with any range type.</span></span> <span data-ttu-id="6ea56-329">以下是一些示例。</span><span class="sxs-lookup"><span data-stu-id="6ea56-329">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="6ea56-330">示例</span><span class="sxs-lookup"><span data-stu-id="6ea56-330">Examples</span></span>

- <span data-ttu-id="6ea56-331">**从 2017 年 9 月 4 日开始直到年底，在每周一的下午 1:00 - 1:30 会面**</span><span class="sxs-lookup"><span data-stu-id="6ea56-331">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="6ea56-332">`weekly` 定期模式类型可轻松实现“每周一”的要求。</span><span class="sxs-lookup"><span data-stu-id="6ea56-332">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="6ea56-333">“直到年底”的要求表示 `endDate` 定期范围类型。</span><span class="sxs-lookup"><span data-stu-id="6ea56-333">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  <span data-ttu-id="6ea56-334">由于 2017 年 12 月 31 日是周日，因此，此系列的最后一次事件将于 12 月 25 日星期一发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-334">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="6ea56-335">**从 2017 年 8 月 29 日开始，在每两个月的第一个星期四的下午 2:00 - 3:00 会面**</span><span class="sxs-lookup"><span data-stu-id="6ea56-335">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="6ea56-336">使用相对每月模式可实现“每两个月的第一个星期四”的要求。</span><span class="sxs-lookup"><span data-stu-id="6ea56-336">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="6ea56-337">“每两个月”部分表示应将 **interval** 设置为 `2`。</span><span class="sxs-lookup"><span data-stu-id="6ea56-337">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="6ea56-338">由于结束日期没有要求，可使用 `noEnd` 范围类型。</span><span class="sxs-lookup"><span data-stu-id="6ea56-338">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  <span data-ttu-id="6ea56-339">由于 **startDate** 的值在 8 月的第一个星期四之后，因此，此系列的第一次事件将在 9 月发生。</span><span class="sxs-lookup"><span data-stu-id="6ea56-339">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6ea56-340">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6ea56-340">Next steps</span></span>
    
<span data-ttu-id="6ea56-341">了解更多关于[与 Outlook 日历集成](outlook-calendar-concept-overview.md)的信息。</span><span class="sxs-lookup"><span data-stu-id="6ea56-341">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
