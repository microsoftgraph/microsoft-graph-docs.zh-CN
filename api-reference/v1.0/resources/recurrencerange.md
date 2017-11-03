# <a name="recurrencerange-resource-type"></a><span data-ttu-id="81064-101">recurrenceRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="81064-101">recurrenceRange resource type</span></span>

<span data-ttu-id="81064-102">描述了定期[事件](event.md)在哪个日期范围内重复发生。</span><span class="sxs-lookup"><span data-stu-id="81064-102">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="81064-103">可以使用下面的 3 种方法之一（具体视方案而定），指定定期事件的日期范围。</span><span class="sxs-lookup"><span data-stu-id="81064-103">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="81064-104">虽然必须始终指定日期范围的 **startDate** 值，但定期事件的结束日期可以有多种指定方法。可以指定定期事件在特定日期前结束、没有结束日期或在重复发生特定次数后结束。</span><span class="sxs-lookup"><span data-stu-id="81064-104">While you must always specify a **startDate** value for the date range, you can, for example, specify a recurring event that ends by a specific date, or that doesn't end, or that ends after 5 occurrences.</span></span> <span data-ttu-id="81064-105">请注意，在日期范围内，实际发生的定期事件始终遵循为事件指定的定期模式。</span><span class="sxs-lookup"><span data-stu-id="81064-105">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="81064-106">定期事件始终由 [recurrencePattern](recurrencepattern.md)（事件的重复发生频率）和 **recurrenceRange**（事件在哪个日期范围内重复发生）进行定义。</span><span class="sxs-lookup"><span data-stu-id="81064-106">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

<span data-ttu-id="81064-107">**type** 属性可用于指定不同类型的 **recurrenceRange**。</span><span class="sxs-lookup"><span data-stu-id="81064-107">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="81064-108">请注意每种类型的必需属性，如下表所述。</span><span class="sxs-lookup"><span data-stu-id="81064-108">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="81064-109">定期范围类型</span><span class="sxs-lookup"><span data-stu-id="81064-109">Type of recurrence range</span></span> | <span data-ttu-id="81064-110">type 属性值</span><span class="sxs-lookup"><span data-stu-id="81064-110">Value of type property</span></span> | <span data-ttu-id="81064-111">说明</span><span class="sxs-lookup"><span data-stu-id="81064-111">Description</span></span> | <span data-ttu-id="81064-112">示例</span><span class="sxs-lookup"><span data-stu-id="81064-112">Example</span></span> | <span data-ttu-id="81064-113">必需属性</span><span class="sxs-lookup"><span data-stu-id="81064-113">Required properties</span></span> |
|:---------------|:--------|:--------|:--------|:----------|
|<span data-ttu-id="81064-114">有结束日期的范围</span><span class="sxs-lookup"><span data-stu-id="81064-114">Range with end date</span></span> | `endDate` | <span data-ttu-id="81064-115">事件在 **startDate** 到 **endDate**（含边界值）之间遵循相应的定期模式重复发生。</span><span class="sxs-lookup"><span data-stu-id="81064-115">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate**.</span></span> | <span data-ttu-id="81064-116">事件在日期范围 2017 年 6 月 1 日到 2017 年 6 月 15 日之间重复发生。</span><span class="sxs-lookup"><span data-stu-id="81064-116">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="81064-117">**type**、**startDate**、**endDate**</span><span class="sxs-lookup"><span data-stu-id="81064-117">**type**, **startDate**, **endDate**</span></span> | 
|<span data-ttu-id="81064-118">无结束日期的范围</span><span class="sxs-lookup"><span data-stu-id="81064-118">Range without an end date</span></span> | `noEnd` | <span data-ttu-id="81064-119">事件从 **startDate** 起遵循相应的定期模式重复发生。</span><span class="sxs-lookup"><span data-stu-id="81064-119">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="81064-120">事件在从 2017 年 6 月 1 日起的无限期日期范围内重复发生。</span><span class="sxs-lookup"><span data-stu-id="81064-120">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="81064-121">**type**、**startDate**</span><span class="sxs-lookup"><span data-stu-id="81064-121">**type**, **startDate**</span></span> |
|<span data-ttu-id="81064-122">指定了特定发生次数的范围</span><span class="sxs-lookup"><span data-stu-id="81064-122">Range with specific number of occurrences</span></span> | `numbered` | <span data-ttu-id="81064-123">从 **startDate** 起，事件遵循定期模式重复发生 **numberOfOccurrences** 次。</span><span class="sxs-lookup"><span data-stu-id="81064-123">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="81064-124">事件在从 2017 年 6 月 1 日起的日期范围内重复发生 10 次。</span><span class="sxs-lookup"><span data-stu-id="81064-124">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="81064-125">**type**、**startDate**、**numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="81064-125">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="properties"></a><span data-ttu-id="81064-126">属性</span><span class="sxs-lookup"><span data-stu-id="81064-126">Properties</span></span>

| <span data-ttu-id="81064-127">属性</span><span class="sxs-lookup"><span data-stu-id="81064-127">Property</span></span>     | <span data-ttu-id="81064-128">类型</span><span class="sxs-lookup"><span data-stu-id="81064-128">Type</span></span>   |<span data-ttu-id="81064-129">说明</span><span class="sxs-lookup"><span data-stu-id="81064-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81064-130">endDate</span><span class="sxs-lookup"><span data-stu-id="81064-130">endDate</span></span>|<span data-ttu-id="81064-131">Date</span><span class="sxs-lookup"><span data-stu-id="81064-131">Date</span></span>|<span data-ttu-id="81064-132">定期模式的停止应用日期。</span><span class="sxs-lookup"><span data-stu-id="81064-132">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="81064-133">会议的最后一次发生时间可能不是此日期，具体视事件的定期模式而定。</span><span class="sxs-lookup"><span data-stu-id="81064-133">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="81064-134">如果 **type** 为 `endDate`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="81064-134">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="81064-135">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="81064-135">numberOfOccurrences</span></span>|<span data-ttu-id="81064-136">Int32</span><span class="sxs-lookup"><span data-stu-id="81064-136">Int32</span></span>|<span data-ttu-id="81064-137">事件重复发生次数。</span><span class="sxs-lookup"><span data-stu-id="81064-137">The number of times to repeat the event.</span></span> <span data-ttu-id="81064-138">如果 **type** 为 `numbered`，此为必需属性，且必须为正数。</span><span class="sxs-lookup"><span data-stu-id="81064-138">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="81064-139">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="81064-139">recurrenceTimeZone</span></span>|<span data-ttu-id="81064-140">String</span><span class="sxs-lookup"><span data-stu-id="81064-140">String</span></span> |<span data-ttu-id="81064-141">**startDate** 和 **endDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="81064-141">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="81064-142">此为可选属性。</span><span class="sxs-lookup"><span data-stu-id="81064-142">Optional.</span></span> <span data-ttu-id="81064-143">如果未指定，使用的是事件时区。</span><span class="sxs-lookup"><span data-stu-id="81064-143">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="81064-144">startDate</span><span class="sxs-lookup"><span data-stu-id="81064-144">startDate</span></span>|<span data-ttu-id="81064-145">Date</span><span class="sxs-lookup"><span data-stu-id="81064-145">Date</span></span>|<span data-ttu-id="81064-146">定期模式的开始应用日期。</span><span class="sxs-lookup"><span data-stu-id="81064-146">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="81064-147">会议的第一次发生时间可能是此日期，也可能晚于此日期，具体视事件的定期模式而定。</span><span class="sxs-lookup"><span data-stu-id="81064-147">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="81064-148">必须与定期[事件](event.md)的 **start** 属性值相同。</span><span class="sxs-lookup"><span data-stu-id="81064-148">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="81064-149">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="81064-149">Required.</span></span>|
|<span data-ttu-id="81064-150">type</span><span class="sxs-lookup"><span data-stu-id="81064-150">type</span></span>|<span data-ttu-id="81064-151">String</span><span class="sxs-lookup"><span data-stu-id="81064-151">String</span></span>|<span data-ttu-id="81064-152">定期范围。</span><span class="sxs-lookup"><span data-stu-id="81064-152">The recurrence range.</span></span> <span data-ttu-id="81064-153">可取值为：`endDate`、`noEnd`、`numbered`。</span><span class="sxs-lookup"><span data-stu-id="81064-153">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="81064-154">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="81064-154">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81064-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81064-155">JSON representation</span></span>

<span data-ttu-id="81064-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81064-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
