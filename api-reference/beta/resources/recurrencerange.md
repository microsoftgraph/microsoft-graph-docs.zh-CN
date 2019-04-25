---
title: recurrenceRange 资源类型
description: '描述了定期事件在哪个日期范围内重复发生。 '
localization_priority: Normal
ms.openlocfilehash: cee5a06d8f76264cd7c98924c532c8f864cab87d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563080"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="cf3fb-103">recurrenceRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf3fb-103">recurrenceRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf3fb-104">描述了定期[事件](event.md)在哪个日期范围内重复发生。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-104">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="cf3fb-105">可以使用下面的 3 种方法之一（具体视方案而定），指定定期事件的日期范围。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-105">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="cf3fb-106">虽然必须始终指定日期范围的 **startDate** 值，但定期事件的结束日期可以有多种指定方法。可以指定定期事件在特定日期前结束、没有结束日期或在重复发生特定次数后结束。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-106">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="cf3fb-107">请注意，在日期范围内，实际发生的定期事件始终遵循为事件指定的定期模式。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-107">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="cf3fb-108">定期事件始终由 [recurrencePattern](recurrencepattern.md)（事件的重复发生频率）和 **recurrenceRange**（事件在哪个日期范围内重复发生）进行定义。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-108">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="cf3fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="cf3fb-109">Properties</span></span>

| <span data-ttu-id="cf3fb-110">属性</span><span class="sxs-lookup"><span data-stu-id="cf3fb-110">Property</span></span>     | <span data-ttu-id="cf3fb-111">类型</span><span class="sxs-lookup"><span data-stu-id="cf3fb-111">Type</span></span>   |<span data-ttu-id="cf3fb-112">说明</span><span class="sxs-lookup"><span data-stu-id="cf3fb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf3fb-113">endDate</span><span class="sxs-lookup"><span data-stu-id="cf3fb-113">endDate</span></span>|<span data-ttu-id="cf3fb-114">Date</span><span class="sxs-lookup"><span data-stu-id="cf3fb-114">Date</span></span>|<span data-ttu-id="cf3fb-115">定期模式的停止应用日期。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-115">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="cf3fb-116">会议的最后一次发生时间可能不是此日期，具体视事件的定期模式而定。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-116">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="cf3fb-117">如果 **type** 为 `endDate`，此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-117">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="cf3fb-118">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="cf3fb-118">numberOfOccurrences</span></span>|<span data-ttu-id="cf3fb-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cf3fb-119">Int32</span></span>|<span data-ttu-id="cf3fb-120">事件重复发生次数。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-120">The number of times to repeat the event.</span></span> <span data-ttu-id="cf3fb-121">如果 **type** 为 `numbered`，此为必需属性，且必须为正数。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-121">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="cf3fb-122">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="cf3fb-122">recurrenceTimeZone</span></span>|<span data-ttu-id="cf3fb-123">String</span><span class="sxs-lookup"><span data-stu-id="cf3fb-123">String</span></span> |<span data-ttu-id="cf3fb-124">**startDate** 和 **endDate** 属性的时区。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-124">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="cf3fb-125">此为可选属性。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-125">Optional.</span></span> <span data-ttu-id="cf3fb-126">如果未指定，使用的是事件时区。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-126">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="cf3fb-127">startDate</span><span class="sxs-lookup"><span data-stu-id="cf3fb-127">startDate</span></span>|<span data-ttu-id="cf3fb-128">日期</span><span class="sxs-lookup"><span data-stu-id="cf3fb-128">Date</span></span>|<span data-ttu-id="cf3fb-129">定期模式的开始应用日期。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-129">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="cf3fb-130">会议的第一次发生时间可能是此日期，也可能晚于此日期，具体视事件的定期模式而定。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-130">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="cf3fb-131">必须与定期[事件](event.md)的 **start** 属性值相同。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-131">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="cf3fb-132">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-132">Required.</span></span>|
|<span data-ttu-id="cf3fb-133">type</span><span class="sxs-lookup"><span data-stu-id="cf3fb-133">type</span></span>|<span data-ttu-id="cf3fb-134">String</span><span class="sxs-lookup"><span data-stu-id="cf3fb-134">String</span></span>|<span data-ttu-id="cf3fb-135">定期范围。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-135">The recurrence range.</span></span> <span data-ttu-id="cf3fb-136">可取值为：`endDate`、`noEnd`、`numbered`。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-136">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="cf3fb-137">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-137">Required.</span></span>|

<span data-ttu-id="cf3fb-138">**type** 属性可用于指定不同类型的 **recurrenceRange**。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-138">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="cf3fb-139">请注意每种类型的必需属性，如下表所述。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-139">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="cf3fb-140">type 属性</span><span class="sxs-lookup"><span data-stu-id="cf3fb-140">type property</span></span>  | <span data-ttu-id="cf3fb-141">定期范围类型</span><span class="sxs-lookup"><span data-stu-id="cf3fb-141">Type of recurrence range</span></span> | <span data-ttu-id="cf3fb-142">说明</span><span class="sxs-lookup"><span data-stu-id="cf3fb-142">Description</span></span> | <span data-ttu-id="cf3fb-143">示例</span><span class="sxs-lookup"><span data-stu-id="cf3fb-143">Example</span></span> | <span data-ttu-id="cf3fb-144">必需属性</span><span class="sxs-lookup"><span data-stu-id="cf3fb-144">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="cf3fb-145">有结束日期的范围</span><span class="sxs-lookup"><span data-stu-id="cf3fb-145">Range with end date</span></span> | <span data-ttu-id="cf3fb-146">事件在 **startDate** 到 **endDate**（含边界值）之间遵循相应的定期模式重复发生。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-146">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="cf3fb-147">事件在日期范围 2017 年 6 月 1 日到 2017 年 6 月 15 日之间重复发生。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-147">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="cf3fb-148">**type**、**startDate**、**endDate**</span><span class="sxs-lookup"><span data-stu-id="cf3fb-148">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="cf3fb-149">无结束日期的范围</span><span class="sxs-lookup"><span data-stu-id="cf3fb-149">Range without an end date</span></span> | <span data-ttu-id="cf3fb-150">事件从 **startDate** 起遵循相应的定期模式重复发生。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-150">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="cf3fb-151">事件在从 2017 年 6 月 1 日起的无限期日期范围内重复发生。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-151">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="cf3fb-152">**type**、**startDate**</span><span class="sxs-lookup"><span data-stu-id="cf3fb-152">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="cf3fb-153">指定了特定发生次数的范围</span><span class="sxs-lookup"><span data-stu-id="cf3fb-153">Range with specific number of occurrences</span></span> | <span data-ttu-id="cf3fb-154">从 **startDate** 起，事件遵循定期模式重复发生 **numberOfOccurrences** 次。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-154">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="cf3fb-155">事件在从 2017 年 6 月 1 日起的日期范围内重复发生 10 次。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-155">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="cf3fb-156">**type**、**startDate**、**numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="cf3fb-156">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf3fb-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf3fb-157">JSON representation</span></span>

<span data-ttu-id="cf3fb-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf3fb-158">Here is a JSON representation of the resource</span></span>

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
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |",
    "Error: /api-reference/beta/resources/recurrencerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
