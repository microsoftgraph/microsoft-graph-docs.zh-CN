---
title: recurrenceRange 资源类型
description: '描述了定期事件在哪个日期范围内重复发生。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: 472518b6fdc250cfc2fe2c4223d1854eae9b9124
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136549"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="58ea1-103">recurrenceRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="58ea1-103">recurrenceRange resource type</span></span>

<span data-ttu-id="58ea1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58ea1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58ea1-105">描述了定期[事件](event.md)在哪个日期范围内重复发生。</span><span class="sxs-lookup"><span data-stu-id="58ea1-105">Describes a date range over which a recurring [event](event.md) repeats.</span></span>

<span data-ttu-id="58ea1-106">可以使用下面的 3 种方法之一（具体视方案而定），指定定期事件的日期范围。</span><span class="sxs-lookup"><span data-stu-id="58ea1-106">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="58ea1-107">虽然必须始终指定日期范围的 **startDate** 值，但定期事件的结束日期可以有多种指定方法。可以指定定期事件在特定日期前结束、没有结束日期或在重复发生特定次数后结束。</span><span class="sxs-lookup"><span data-stu-id="58ea1-107">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="58ea1-108">请注意，在日期范围内，实际发生的定期事件始终遵循为事件指定的定期模式。</span><span class="sxs-lookup"><span data-stu-id="58ea1-108">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="58ea1-109">定期事件始终由 [recurrencePattern](recurrencepattern.md)（事件的重复发生频率）和 **recurrenceRange**（事件在哪个日期范围内重复发生）进行定义。</span><span class="sxs-lookup"><span data-stu-id="58ea1-109">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="58ea1-110">属性</span><span class="sxs-lookup"><span data-stu-id="58ea1-110">Properties</span></span>

| <span data-ttu-id="58ea1-111">属性</span><span class="sxs-lookup"><span data-stu-id="58ea1-111">Property</span></span>     | <span data-ttu-id="58ea1-112">类型</span><span class="sxs-lookup"><span data-stu-id="58ea1-112">Type</span></span>   |<span data-ttu-id="58ea1-113">说明</span><span class="sxs-lookup"><span data-stu-id="58ea1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58ea1-114">endDate</span><span class="sxs-lookup"><span data-stu-id="58ea1-114">endDate</span></span>|<span data-ttu-id="58ea1-115">Date</span><span class="sxs-lookup"><span data-stu-id="58ea1-115">Date</span></span>|<span data-ttu-id="58ea1-116">定期模式的停止应用日期。</span><span class="sxs-lookup"><span data-stu-id="58ea1-116">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="58ea1-117">会议的最后一次发生时间可能不是此日期，具体视事件的定期模式而定。</span><span class="sxs-lookup"><span data-stu-id="58ea1-117">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="58ea1-118">如果 **type** 为 `endDate`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="58ea1-118">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="58ea1-119">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="58ea1-119">numberOfOccurrences</span></span>|<span data-ttu-id="58ea1-120">Int32</span><span class="sxs-lookup"><span data-stu-id="58ea1-120">Int32</span></span>|<span data-ttu-id="58ea1-121">事件重复发生次数。</span><span class="sxs-lookup"><span data-stu-id="58ea1-121">The number of times to repeat the event.</span></span> <span data-ttu-id="58ea1-122">如果 **type** 为 `numbered`，此为必需属性，且必须为正数。</span><span class="sxs-lookup"><span data-stu-id="58ea1-122">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="58ea1-123">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="58ea1-123">recurrenceTimeZone</span></span>|<span data-ttu-id="58ea1-124">String</span><span class="sxs-lookup"><span data-stu-id="58ea1-124">String</span></span> |<span data-ttu-id="58ea1-125">**startDate** 和 **endDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="58ea1-125">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="58ea1-126">此为可选属性。</span><span class="sxs-lookup"><span data-stu-id="58ea1-126">Optional.</span></span> <span data-ttu-id="58ea1-127">如果未指定，使用的是事件时区。</span><span class="sxs-lookup"><span data-stu-id="58ea1-127">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="58ea1-128">startDate</span><span class="sxs-lookup"><span data-stu-id="58ea1-128">startDate</span></span>|<span data-ttu-id="58ea1-129">Date</span><span class="sxs-lookup"><span data-stu-id="58ea1-129">Date</span></span>|<span data-ttu-id="58ea1-130">定期模式的开始应用日期。</span><span class="sxs-lookup"><span data-stu-id="58ea1-130">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="58ea1-131">会议的第一次发生时间可能是此日期，也可能晚于此日期，具体视事件的定期模式而定。</span><span class="sxs-lookup"><span data-stu-id="58ea1-131">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="58ea1-132">必须与定期 [事件](event.md)的 **start** 属性值相同。</span><span class="sxs-lookup"><span data-stu-id="58ea1-132">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="58ea1-133">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="58ea1-133">Required.</span></span>|
|<span data-ttu-id="58ea1-134">type</span><span class="sxs-lookup"><span data-stu-id="58ea1-134">type</span></span>|<span data-ttu-id="58ea1-135">字符串</span><span class="sxs-lookup"><span data-stu-id="58ea1-135">String</span></span>|<span data-ttu-id="58ea1-136">定期范围。</span><span class="sxs-lookup"><span data-stu-id="58ea1-136">The recurrence range.</span></span> <span data-ttu-id="58ea1-137">可取值为：`endDate`、`noEnd`、`numbered`。</span><span class="sxs-lookup"><span data-stu-id="58ea1-137">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="58ea1-138">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="58ea1-138">Required.</span></span>|

<span data-ttu-id="58ea1-139">**type** 属性可用于指定不同类型的 **recurrenceRange**。</span><span class="sxs-lookup"><span data-stu-id="58ea1-139">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="58ea1-140">请注意每种类型的必需属性，如下表所述。</span><span class="sxs-lookup"><span data-stu-id="58ea1-140">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="58ea1-141">type 属性</span><span class="sxs-lookup"><span data-stu-id="58ea1-141">type property</span></span>  | <span data-ttu-id="58ea1-142">定期范围类型</span><span class="sxs-lookup"><span data-stu-id="58ea1-142">Type of recurrence range</span></span> | <span data-ttu-id="58ea1-143">说明</span><span class="sxs-lookup"><span data-stu-id="58ea1-143">Description</span></span> | <span data-ttu-id="58ea1-144">示例</span><span class="sxs-lookup"><span data-stu-id="58ea1-144">Example</span></span> | <span data-ttu-id="58ea1-145">必需属性</span><span class="sxs-lookup"><span data-stu-id="58ea1-145">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="58ea1-146">有结束日期的范围</span><span class="sxs-lookup"><span data-stu-id="58ea1-146">Range with end date</span></span> | <span data-ttu-id="58ea1-147">事件在 **startDate** 到 **endDate**（含边界值）之间遵循相应的定期模式重复发生。</span><span class="sxs-lookup"><span data-stu-id="58ea1-147">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="58ea1-148">事件在日期范围 2017 年 6 月 1 日到 2017 年 6 月 15 日之间重复发生。</span><span class="sxs-lookup"><span data-stu-id="58ea1-148">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="58ea1-149">**type**、**startDate**、**endDate**</span><span class="sxs-lookup"><span data-stu-id="58ea1-149">**type**, **startDate**, **endDate**</span></span> |
|`noEnd`   |<span data-ttu-id="58ea1-150">无结束日期的范围</span><span class="sxs-lookup"><span data-stu-id="58ea1-150">Range without an end date</span></span> | <span data-ttu-id="58ea1-151">事件从 **startDate** 起遵循相应的定期模式重复发生。</span><span class="sxs-lookup"><span data-stu-id="58ea1-151">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="58ea1-152">事件在从 2017 年 6 月 1 日起的无限期日期范围内重复发生。</span><span class="sxs-lookup"><span data-stu-id="58ea1-152">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="58ea1-153">**type**、**startDate**</span><span class="sxs-lookup"><span data-stu-id="58ea1-153">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="58ea1-154">指定了特定发生次数的范围</span><span class="sxs-lookup"><span data-stu-id="58ea1-154">Range with specific number of occurrences</span></span> | <span data-ttu-id="58ea1-155">从 **startDate** 起，事件遵循定期模式重复发生 **numberOfOccurrences** 次。</span><span class="sxs-lookup"><span data-stu-id="58ea1-155">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="58ea1-156">事件在从 2017 年 6 月 1 日起的日期范围内重复发生 10 次。</span><span class="sxs-lookup"><span data-stu-id="58ea1-156">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="58ea1-157">**type**、**startDate**、**numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="58ea1-157">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="58ea1-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58ea1-158">JSON representation</span></span>

<span data-ttu-id="58ea1-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58ea1-159">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
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
<!--
{
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ]
}
-->


