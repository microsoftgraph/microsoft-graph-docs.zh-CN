# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="fa57a-101">在 Outlook 中将重复约会安排为定期事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="fa57a-102">定期事件是 Outlook 日历的重要组成部分。</span><span class="sxs-lookup"><span data-stu-id="fa57a-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="fa57a-103">无论是与经理每周进行的一对一会议，还是每月第二个星期二的部门评审会议，定期规则只需要创建一次事件，然后让服务器填充系列中的其他内容，从而使过程变得简单。</span><span class="sxs-lookup"><span data-stu-id="fa57a-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="fa57a-104">使定期事件得以“扩展”为单个事件的关键信息点在于定期规则。</span><span class="sxs-lookup"><span data-stu-id="fa57a-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="fa57a-105">此规则同时指定事件重复的频率和持续时间。</span><span class="sxs-lookup"><span data-stu-id="fa57a-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="fa57a-106">Outlook REST API 在[事件资源](../api-reference/v1.0/resources/event.md)的**重复周期**属性中模拟定期规则。</span><span class="sxs-lookup"><span data-stu-id="fa57a-106">The Outlook REST APIs model recurrence rules in the **** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="fa57a-107">每个重复周期由两部分组成：定期模式（频率）和定期范围（持续时间）。</span><span class="sxs-lookup"><span data-stu-id="fa57a-107">Each  is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="fa57a-108">定期模式</span><span class="sxs-lookup"><span data-stu-id="fa57a-108">Recurrence patterns</span></span>

<span data-ttu-id="fa57a-109">重复的第一部分是模式。</span><span class="sxs-lookup"><span data-stu-id="fa57a-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="fa57a-110">它指定事件重复的频率。</span><span class="sxs-lookup"><span data-stu-id="fa57a-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="fa57a-111">例如，一个事件可以“每 3 天”、“每周四”或“每年的 7 月 22 日”重复一次。</span><span class="sxs-lookup"><span data-stu-id="fa57a-111">For example, an event could repeat "every 3 days", "every Thursday", or "on July 22 every year".</span></span> <span data-ttu-id="fa57a-112">在 API 中，模式由 [recurrencePattern 资源](../api-reference/v1.0/resources/recurrencepattern.md)表示。</span><span class="sxs-lookup"><span data-stu-id="fa57a-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="fa57a-113">**recurrencePattern** 的特定字段是必需、可选还是忽略取决于模式的类型。</span><span class="sxs-lookup"><span data-stu-id="fa57a-113">Depending on the type of pattern, certain fields of the **** are required, optional, or ignored.</span></span>

> <span data-ttu-id="fa57a-114">**注意**：即使将字段忽略，仍需验证该字段。</span><span class="sxs-lookup"><span data-stu-id="fa57a-114">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="fa57a-115">如果字段包含一组可能值的列表，那么使用允许集以外的值会导致错误，即使此字段已被忽略也是如此。</span><span class="sxs-lookup"><span data-stu-id="fa57a-115">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="fa57a-116">让我们来看看每个可能的模式类型。</span><span class="sxs-lookup"><span data-stu-id="fa57a-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="fa57a-117">每天</span><span class="sxs-lookup"><span data-stu-id="fa57a-117">Daily</span></span>

<span data-ttu-id="fa57a-118">每天定期模式会导致事件基于每次事件之间的天数重复。</span><span class="sxs-lookup"><span data-stu-id="fa57a-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-119">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-119">Relevant properties</span></span>

| <span data-ttu-id="fa57a-120">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-120">Property</span></span> | <span data-ttu-id="fa57a-121">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-121">Relevance</span></span> | <span data-ttu-id="fa57a-122">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-123">**interval**</span><span class="sxs-lookup"><span data-stu-id="fa57a-123">**interval**</span></span> | <span data-ttu-id="fa57a-124">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-124">Required</span></span> | <span data-ttu-id="fa57a-125">指定每次事件之间的天数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="fa57a-126">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-126">**type**</span></span> | <span data-ttu-id="fa57a-127">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-127">Required</span></span> | <span data-ttu-id="fa57a-128">必须设置为 `daily`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-129">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-129">Examples</span></span>

- <span data-ttu-id="fa57a-130">每天重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="fa57a-131">每三天重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="fa57a-132">每周</span><span class="sxs-lookup"><span data-stu-id="fa57a-132">Weekly</span></span>

<span data-ttu-id="fa57a-133">每周定期模式使事件基于每组事件之间的周数，在每周的同一天或几天重复。</span><span class="sxs-lookup"><span data-stu-id="fa57a-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-134">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-134">Relevant properties</span></span>

| <span data-ttu-id="fa57a-135">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-135">Property</span></span> | <span data-ttu-id="fa57a-136">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-136">Relevance</span></span> | <span data-ttu-id="fa57a-137">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="fa57a-138">**daysOfWeek**</span></span> | <span data-ttu-id="fa57a-139">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-139">Required</span></span> | <span data-ttu-id="fa57a-140">指定事件发生在每周的哪一天/哪几天。</span><span class="sxs-lookup"><span data-stu-id="fa57a-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="fa57a-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="fa57a-141">**firstdayofweek**</span></span> | <span data-ttu-id="fa57a-142">可选</span><span class="sxs-lookup"><span data-stu-id="fa57a-142">Optional</span></span> | <span data-ttu-id="fa57a-143">指定将哪一天视为一周的第一天。</span><span class="sxs-lookup"><span data-stu-id="fa57a-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="fa57a-144">默认值为：`Sunday`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="fa57a-145">**interval**</span><span class="sxs-lookup"><span data-stu-id="fa57a-145">**Interval**</span></span> | <span data-ttu-id="fa57a-146">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-146">Required</span></span> | <span data-ttu-id="fa57a-147">指定每组事件之间的周数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="fa57a-148">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-148">**type**</span></span> | <span data-ttu-id="fa57a-149">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-149">Required</span></span> | <span data-ttu-id="fa57a-150">必须设置为 `weekly`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-151">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-151">Examples</span></span>

- <span data-ttu-id="fa57a-152">每周四重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="fa57a-153">每隔一个周一和周二重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-153">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="fa57a-154">绝对每月</span><span class="sxs-lookup"><span data-stu-id="fa57a-154">Absolute monthly</span></span>

<span data-ttu-id="fa57a-155">绝对每月模式使事件在每个月的同一天（例如，15日）重复，它基于每次事件之间的月数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-155">The absolute monthly pattern causes an event to repeat on the same day of the month (e.g. the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-156">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-156">Relevant properties</span></span>

| <span data-ttu-id="fa57a-157">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-157">Property</span></span> | <span data-ttu-id="fa57a-158">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-158">Relevance</span></span> | <span data-ttu-id="fa57a-159">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="fa57a-160">**dayOfMonth**</span></span> | <span data-ttu-id="fa57a-161">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-161">Required</span></span> | <span data-ttu-id="fa57a-162">指定事件发生在每月的哪一天。</span><span class="sxs-lookup"><span data-stu-id="fa57a-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="fa57a-163">**interval**</span><span class="sxs-lookup"><span data-stu-id="fa57a-163">**Interval**</span></span> | <span data-ttu-id="fa57a-164">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-164">Required</span></span> | <span data-ttu-id="fa57a-165">指定每次事件之间的月数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="fa57a-166">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-166">**type**</span></span> | <span data-ttu-id="fa57a-167">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-167">Required</span></span> | <span data-ttu-id="fa57a-168">必须设置为 `absoluteMonthly`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-169">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-169">Examples</span></span>

- <span data-ttu-id="fa57a-170">在每月的 15 号重复此事件。</span><span class="sxs-lookup"><span data-stu-id="fa57a-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="fa57a-171">按季度（每 3 个月）在 7 号重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="fa57a-172">相对每月</span><span class="sxs-lookup"><span data-stu-id="fa57a-172">Relative monthly</span></span>

<span data-ttu-id="fa57a-173">相对每月模式使事件基于每次事件之间的月数，在每个月同一相对位置中每周的同一天重复。</span><span class="sxs-lookup"><span data-stu-id="fa57a-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="fa57a-174">例如，“每月的第二个星期三”。</span><span class="sxs-lookup"><span data-stu-id="fa57a-174">For example, "every second Wednesday of the month".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-175">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-175">Relevant properties</span></span>

| <span data-ttu-id="fa57a-176">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-176">Property</span></span> | <span data-ttu-id="fa57a-177">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-177">Relevance</span></span> | <span data-ttu-id="fa57a-178">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="fa57a-179">**daysOfWeek**</span></span> | <span data-ttu-id="fa57a-180">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-180">Required</span></span> | <span data-ttu-id="fa57a-181">指定事件发生在一周的哪一天/哪几天。</span><span class="sxs-lookup"><span data-stu-id="fa57a-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="fa57a-182">相对每月事件每月仅发生一次，因此，如果指定多个值，事件会在满足模式的第一天发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="fa57a-183">**index**</span><span class="sxs-lookup"><span data-stu-id="fa57a-183">**Index**</span></span> | <span data-ttu-id="fa57a-184">可选</span><span class="sxs-lookup"><span data-stu-id="fa57a-184">Optional</span></span> | <span data-ttu-id="fa57a-185">指定事件在 **daysOfsWeek** 中指定的允许天数的哪个实例上发生，从当月的第一个实例开始计数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="fa57a-186">可能的值是：`first`、`second`、`third`、`fourth` 和 `last`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="fa57a-187">默认值为：`first`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-187">Default value: `first`.</span></span> |
| <span data-ttu-id="fa57a-188">**interval**</span><span class="sxs-lookup"><span data-stu-id="fa57a-188">**Interval**</span></span> | <span data-ttu-id="fa57a-189">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-189">Required</span></span> | <span data-ttu-id="fa57a-190">指定每次事件之间的月数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="fa57a-191">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-191">**type**</span></span> | <span data-ttu-id="fa57a-192">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-192">Required</span></span> | <span data-ttu-id="fa57a-193">必须设置为 `relativeMonthly`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-194">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-194">Examples</span></span>

- <span data-ttu-id="fa57a-195">在每月的第二个星期三重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="fa57a-196">在每月的第一个星期四或星期五重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="fa57a-197">绝对每年</span><span class="sxs-lookup"><span data-stu-id="fa57a-197">Absolute yearly</span></span>

<span data-ttu-id="fa57a-198">绝对每年模式使事件在每年的同一月份的同一天（例如，4 月 15 日）重复，它基于每次事件之间的年数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-198">The absolute yearly pattern causes an event to repeat on the same month and day (e.g. April 15th), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-199">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-199">Relevant properties</span></span>

| <span data-ttu-id="fa57a-200">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-200">Property</span></span> | <span data-ttu-id="fa57a-201">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-201">Relevance</span></span> | <span data-ttu-id="fa57a-202">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="fa57a-203">**dayOfMonth**</span></span> | <span data-ttu-id="fa57a-204">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-204">Required</span></span> | <span data-ttu-id="fa57a-205">指定事件发生在每月的哪一天。</span><span class="sxs-lookup"><span data-stu-id="fa57a-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="fa57a-206">**month**</span><span class="sxs-lookup"><span data-stu-id="fa57a-206">**month**</span></span> | <span data-ttu-id="fa57a-207">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-207">Required</span></span> | <span data-ttu-id="fa57a-208">指定事件发生的月份。</span><span class="sxs-lookup"><span data-stu-id="fa57a-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="fa57a-209">**interval**</span><span class="sxs-lookup"><span data-stu-id="fa57a-209">**Interval**</span></span> | <span data-ttu-id="fa57a-210">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-210">Required</span></span> | <span data-ttu-id="fa57a-211">指定每次事件之间的年数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="fa57a-212">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-212">**type**</span></span> | <span data-ttu-id="fa57a-213">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-213">Required</span></span> | <span data-ttu-id="fa57a-214">必须设置为 `absoluteYearly`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="fa57a-215">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-215">Example</span></span>

- <span data-ttu-id="fa57a-216">在每年的 4 月 15 日重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="fa57a-217">相对每年</span><span class="sxs-lookup"><span data-stu-id="fa57a-217">Relative yearly</span></span>

<span data-ttu-id="fa57a-218">相对每年模式使事件基于每次事件之间的年数，在特定月份同一相对位置中每周的同一天重复。</span><span class="sxs-lookup"><span data-stu-id="fa57a-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="fa57a-219">例如，“每个 11 月的最后一个星期三”。</span><span class="sxs-lookup"><span data-stu-id="fa57a-219">For example, "every last Wednesday of November".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-220">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-220">Relevant properties</span></span>

| <span data-ttu-id="fa57a-221">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-221">Property</span></span> | <span data-ttu-id="fa57a-222">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-222">Relevance</span></span> | <span data-ttu-id="fa57a-223">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="fa57a-224">**daysOfWeek**</span></span> | <span data-ttu-id="fa57a-225">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-225">Required</span></span> | <span data-ttu-id="fa57a-226">指定事件发生在一周的哪一天/哪几天。</span><span class="sxs-lookup"><span data-stu-id="fa57a-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="fa57a-227">相对每年事件每年仅发生一次，因此，如果指定多个值，事件会在满足模式的第一天发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="fa57a-228">**index**</span><span class="sxs-lookup"><span data-stu-id="fa57a-228">**Index**</span></span> | <span data-ttu-id="fa57a-229">可选</span><span class="sxs-lookup"><span data-stu-id="fa57a-229">Optional</span></span> | <span data-ttu-id="fa57a-230">指定事件在 **daysOfsWeek** 中指定的允许天数的哪个实例上发生，从当月的第一个实例开始计数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="fa57a-231">可能的值是：`first`、`second`、`third`、`fourth` 和 `last`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="fa57a-232">默认值为：`first`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-232">Default value: `first`.</span></span> |
| <span data-ttu-id="fa57a-233">**month**</span><span class="sxs-lookup"><span data-stu-id="fa57a-233">**month**</span></span> | <span data-ttu-id="fa57a-234">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-234">Required</span></span> | <span data-ttu-id="fa57a-235">指定事件发生的月份。</span><span class="sxs-lookup"><span data-stu-id="fa57a-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="fa57a-236">**interval**</span><span class="sxs-lookup"><span data-stu-id="fa57a-236">**Interval**</span></span> | <span data-ttu-id="fa57a-237">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-237">Required</span></span> | <span data-ttu-id="fa57a-238">指定每次事件之间的年数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="fa57a-239">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-239">**type**</span></span> | <span data-ttu-id="fa57a-240">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-240">Required</span></span> | <span data-ttu-id="fa57a-241">必须设置为 `relativeMonthly`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-242">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-242">Examples</span></span>

- <span data-ttu-id="fa57a-243">每年 11 月的最后一个星期三重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="fa57a-244">定期范围</span><span class="sxs-lookup"><span data-stu-id="fa57a-244">Recurrence ranges</span></span>

<span data-ttu-id="fa57a-245">重复的第二部分是范围。</span><span class="sxs-lookup"><span data-stu-id="fa57a-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="fa57a-246">它指定模式重复的持续时间。</span><span class="sxs-lookup"><span data-stu-id="fa57a-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="fa57a-247">例如，一个事件可以在发生 10 次后于特定日期结束，也可以不结束。</span><span class="sxs-lookup"><span data-stu-id="fa57a-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="fa57a-248">在 API 中，由 [recurrenceRange 资源](../api-reference/v1.0/resources/recurrencepattern.md)表示范围。</span><span class="sxs-lookup"><span data-stu-id="fa57a-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="fa57a-249">**recurrenceRange** 的特定字段是必需还是忽略取决于范围的类型。</span><span class="sxs-lookup"><span data-stu-id="fa57a-249">Depending on the type of range, certain fields of the **** are required or ignored.</span></span>

> <span data-ttu-id="fa57a-250">**注意**：即使将字段忽略，仍需验证该字段。</span><span class="sxs-lookup"><span data-stu-id="fa57a-250">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="fa57a-251">如果字段包含一组可能值的列表，那么使用允许集以外的值会导致错误，即使此字段已被忽略也是如此。</span><span class="sxs-lookup"><span data-stu-id="fa57a-251">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="fa57a-252">让我们来看看每个可能的范围类型。</span><span class="sxs-lookup"><span data-stu-id="fa57a-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="fa57a-253">编号的范围</span><span class="sxs-lookup"><span data-stu-id="fa57a-253">Numbered range</span></span>

<span data-ttu-id="fa57a-254">编号的范围使事件（基于模式）从开始日期起按固定次数发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-255">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-255">Relevant properties</span></span>

| <span data-ttu-id="fa57a-256">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-256">Property</span></span> | <span data-ttu-id="fa57a-257">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-257">Relevance</span></span> | <span data-ttu-id="fa57a-258">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="fa57a-259">**numberOfOccurences**</span></span> | <span data-ttu-id="fa57a-260">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-260">Required</span></span> | <span data-ttu-id="fa57a-261">指定事件发生的次数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="fa57a-262">必须是正整数。</span><span class="sxs-lookup"><span data-stu-id="fa57a-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="fa57a-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="fa57a-263">**recurrenceTimeZone**</span></span> | <span data-ttu-id="fa57a-264">可选</span><span class="sxs-lookup"><span data-stu-id="fa57a-264">Optional</span></span> | <span data-ttu-id="fa57a-265">指定 **startDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="fa57a-265">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="fa57a-266">如果未指定，将使用事件时区。</span><span class="sxs-lookup"><span data-stu-id="fa57a-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="fa57a-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="fa57a-267">**startDate**</span></span> | <span data-ttu-id="fa57a-268">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-268">Required</span></span> | <span data-ttu-id="fa57a-269">指定开始应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="fa57a-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="fa57a-270">**startDate** 的值必须与[事件资源](../api-reference/v1.0/resources/event.md)上的 **start** 属性的日期值对应。</span><span class="sxs-lookup"><span data-stu-id="fa57a-270">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="fa57a-271">请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-271">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="fa57a-272">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-272">**type**</span></span> | <span data-ttu-id="fa57a-273">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-273">Required</span></span> | <span data-ttu-id="fa57a-274">必须设置为 `numbered`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-275">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-275">Examples</span></span>

- <span data-ttu-id="fa57a-276">此事件重复 10 次</span><span class="sxs-lookup"><span data-stu-id="fa57a-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="fa57a-277">结束日期范围</span><span class="sxs-lookup"><span data-stu-id="fa57a-277">End date range</span></span>

<span data-ttu-id="fa57a-278">结束日期范围使事件在开始日期和结束日期之间匹配适用模式的所有天数发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-279">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-279">Relevant properties</span></span>

| <span data-ttu-id="fa57a-280">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-280">Property</span></span> | <span data-ttu-id="fa57a-281">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-281">Relevance</span></span> | <span data-ttu-id="fa57a-282">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="fa57a-283">**endDate**</span></span> | <span data-ttu-id="fa57a-284">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-284">Required</span></span> | <span data-ttu-id="fa57a-285">指定停止应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="fa57a-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="fa57a-286">请注意，如果日期不符合模式，最后一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-286">Note: the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="fa57a-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="fa57a-287">**recurrenceTimeZone**</span></span> | <span data-ttu-id="fa57a-288">可选</span><span class="sxs-lookup"><span data-stu-id="fa57a-288">Optional</span></span> | <span data-ttu-id="fa57a-289">指定 **startDate** 和 **endDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="fa57a-289">Specifies the time zone for the **** and **** properties.</span></span> <span data-ttu-id="fa57a-290">如果未指定，将使用事件时区。</span><span class="sxs-lookup"><span data-stu-id="fa57a-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="fa57a-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="fa57a-291">**startDate**</span></span> | <span data-ttu-id="fa57a-292">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-292">Required</span></span> | <span data-ttu-id="fa57a-293">指定开始应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="fa57a-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="fa57a-294">**startDate** 的值必须与[事件资源](../api-reference/v1.0/resources/event.md)上的 **start** 属性的日期值对应。</span><span class="sxs-lookup"><span data-stu-id="fa57a-294">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="fa57a-295">请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-295">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="fa57a-296">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-296">**type**</span></span> | <span data-ttu-id="fa57a-297">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-297">Required</span></span> | <span data-ttu-id="fa57a-298">必须设置为 **endDate**。</span><span class="sxs-lookup"><span data-stu-id="fa57a-298">Must be set to ****.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-299">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-299">Examples</span></span>

- <span data-ttu-id="fa57a-300">从 2017 年 7 月 1 日到 2017 年 7 月 31 日重复此事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-300">Repeat this event from July 1 2017 to July 31 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="fa57a-301">无结束范围</span><span class="sxs-lookup"><span data-stu-id="fa57a-301">No end range</span></span>

<span data-ttu-id="fa57a-302">无结束区域使事件在开始日期后匹配适用模式的所有天数发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="fa57a-303">相关属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-303">Relevant properties</span></span>

| <span data-ttu-id="fa57a-304">属性</span><span class="sxs-lookup"><span data-stu-id="fa57a-304">Property</span></span> | <span data-ttu-id="fa57a-305">相关性</span><span class="sxs-lookup"><span data-stu-id="fa57a-305">Relevance</span></span> | <span data-ttu-id="fa57a-306">说明</span><span class="sxs-lookup"><span data-stu-id="fa57a-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="fa57a-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="fa57a-307">**recurrenceTimeZone**</span></span> | <span data-ttu-id="fa57a-308">可选</span><span class="sxs-lookup"><span data-stu-id="fa57a-308">Optional</span></span> | <span data-ttu-id="fa57a-309">指定 **startDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="fa57a-309">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="fa57a-310">如果未指定，将使用事件时区。</span><span class="sxs-lookup"><span data-stu-id="fa57a-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="fa57a-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="fa57a-311">**startDate**</span></span> | <span data-ttu-id="fa57a-312">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-312">Required</span></span> | <span data-ttu-id="fa57a-313">指定开始应用模式的日期。</span><span class="sxs-lookup"><span data-stu-id="fa57a-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="fa57a-314">**startDate** 的值必须与[事件资源](../api-reference/v1.0/resources/event.md)上的 **start** 属性的日期值对应。</span><span class="sxs-lookup"><span data-stu-id="fa57a-314">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="fa57a-315">请注意，如果日期不符合模式，第一次会议可能不会在此日期发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-315">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="fa57a-316">**type**</span><span class="sxs-lookup"><span data-stu-id="fa57a-316">**type**</span></span> | <span data-ttu-id="fa57a-317">必需</span><span class="sxs-lookup"><span data-stu-id="fa57a-317">Required</span></span> | <span data-ttu-id="fa57a-318">必须设置为 `noEnd`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="fa57a-319">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-319">Examples</span></span>

- <span data-ttu-id="fa57a-320">从 2017 年 5 月 15 日起重复此事件，无结束日期</span><span class="sxs-lookup"><span data-stu-id="fa57a-320">Repeat this event from May 15 2017 forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="fa57a-321">使用模式和范围创建定期事件</span><span class="sxs-lookup"><span data-stu-id="fa57a-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="fa57a-322">我们已经分别查看了模式和范围，让我们再来了解一下它们如何协同工作以及如何与事件中的 **start** 和 **end** 属性交互。</span><span class="sxs-lookup"><span data-stu-id="fa57a-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **** and **** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="fa57a-323">创建定期规则</span><span class="sxs-lookup"><span data-stu-id="fa57a-323">Creating a recurrence rule</span></span>

<span data-ttu-id="fa57a-324">如要创建定期规则，必须同时指定模式和范围。</span><span class="sxs-lookup"><span data-stu-id="fa57a-324">In order to create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="fa57a-325">模式类型与范围类型可任意搭配使用。</span><span class="sxs-lookup"><span data-stu-id="fa57a-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="fa57a-326">以下是一些示例。</span><span class="sxs-lookup"><span data-stu-id="fa57a-326">Here are a few suggestions:</span></span>

#### <a name="examples"></a><span data-ttu-id="fa57a-327">示例</span><span class="sxs-lookup"><span data-stu-id="fa57a-327">Examples</span></span>

- <span data-ttu-id="fa57a-328">**从 2017 年 9 月 4 日开始直到年底，在每周一的下午 1:00 - 1:30 会面**</span><span class="sxs-lookup"><span data-stu-id="fa57a-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017 until the end of the year**</span></span>

  - <span data-ttu-id="fa57a-329">`weekly` 定期模式类型可轻松实现“每周一”的要求。</span><span class="sxs-lookup"><span data-stu-id="fa57a-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="fa57a-330">“直到年底”的要求表示 `endDate` 定期范围类型。</span><span class="sxs-lookup"><span data-stu-id="fa57a-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="fa57a-331">由于 2017 年 12 月 31 日是周日，因此，此系列的最后一次事件将于 12 月 25 日星期一发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-331">Because December 31, 2017 is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="fa57a-332">**从 2017 年 8 月 29 日开始，在每两个月的第一个星期四的下午 2:00 - 3:00 会面**</span><span class="sxs-lookup"><span data-stu-id="fa57a-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="fa57a-333">使用相对每月模式可实现“每两个月的第一个星期四”的要求。</span><span class="sxs-lookup"><span data-stu-id="fa57a-333">The "first Thursday of every other month" requirement is achievable using a relative monthly pattern.</span></span> <span data-ttu-id="fa57a-334">“每两个月”部分表示应将 **interval** 设置为 `2`。</span><span class="sxs-lookup"><span data-stu-id="fa57a-334">The "every other month" portion indicates the **** should be set to `2`.</span></span>
  - <span data-ttu-id="fa57a-335">由于结束日期没有要求，可使用 `noEnd` 范围类型。</span><span class="sxs-lookup"><span data-stu-id="fa57a-335">Since there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="fa57a-336">由于 **startDate** 的值在 8 月的第一个星期四之后，因此，此系列的第一次事件将在 9 月发生。</span><span class="sxs-lookup"><span data-stu-id="fa57a-336">Because the value of **** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa57a-337">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fa57a-337">Next steps</span></span>
    
<span data-ttu-id="fa57a-338">了解更多关于[与 Outlook 日历集成](outlook-calendar-concept-overview.md)的信息。</span><span class="sxs-lookup"><span data-stu-id="fa57a-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
