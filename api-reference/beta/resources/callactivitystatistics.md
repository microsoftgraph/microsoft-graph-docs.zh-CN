---
title: callActivityStatistics 资源类型
description: 表示有关用户的呼叫活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 014cec3f8adab9f8d41b9f3062b38898b9956bb6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450727"
---
# <a name="callactivitystatistics-resource-type"></a><span data-ttu-id="558b3-103">callActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="558b3-103">callActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="558b3-104">表示有关用户在 Microsoft 团队或 Skype for business 上的呼叫活动中花费的时间的数据。</span><span class="sxs-lookup"><span data-stu-id="558b3-104">Represents data about the user's time spent in call activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="558b3-105">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="558b3-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="558b3-106">属性</span><span class="sxs-lookup"><span data-stu-id="558b3-106">Properties</span></span>

| <span data-ttu-id="558b3-107">属性</span><span class="sxs-lookup"><span data-stu-id="558b3-107">Property</span></span>     | <span data-ttu-id="558b3-108">类型</span><span class="sxs-lookup"><span data-stu-id="558b3-108">Type</span></span>        | <span data-ttu-id="558b3-109">说明</span><span class="sxs-lookup"><span data-stu-id="558b3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="558b3-110">activity</span><span class="sxs-lookup"><span data-stu-id="558b3-110">activity</span></span>|<span data-ttu-id="558b3-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="558b3-111">analyticsActivityType</span></span>| <span data-ttu-id="558b3-112">返回其统计信息的呼叫活动。</span><span class="sxs-lookup"><span data-stu-id="558b3-112">Call activity for which statistics are returned.</span></span>|
|<span data-ttu-id="558b3-113">duration</span><span class="sxs-lookup"><span data-stu-id="558b3-113">duration</span></span>|<span data-ttu-id="558b3-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="558b3-114">Duration</span></span>|<span data-ttu-id="558b3-115">对呼叫花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="558b3-115">Total hours spent on calls.</span></span> <span data-ttu-id="558b3-116">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="558b3-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="558b3-117">endDate</span><span class="sxs-lookup"><span data-stu-id="558b3-117">endDate</span></span>|<span data-ttu-id="558b3-118">Date</span><span class="sxs-lookup"><span data-stu-id="558b3-118">Date</span></span>|<span data-ttu-id="558b3-119">呼叫活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="558b3-119">Date when the call activity ended.</span></span> <span data-ttu-id="558b3-120">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="558b3-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="558b3-121">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="558b3-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="558b3-122">id</span><span class="sxs-lookup"><span data-stu-id="558b3-122">id</span></span>|<span data-ttu-id="558b3-123">String</span><span class="sxs-lookup"><span data-stu-id="558b3-123">String</span></span>| <span data-ttu-id="558b3-124">呼叫活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="558b3-124">Read-only ID for the call activity.</span></span>|
|<span data-ttu-id="558b3-125">startDate</span><span class="sxs-lookup"><span data-stu-id="558b3-125">startDate</span></span>|<span data-ttu-id="558b3-126">日期</span><span class="sxs-lookup"><span data-stu-id="558b3-126">Date</span></span>|<span data-ttu-id="558b3-127">呼叫活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="558b3-127">Date when the call activity started.</span></span> <span data-ttu-id="558b3-128">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="558b3-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="558b3-129">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="558b3-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="558b3-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="558b3-130">timeZoneUsed</span></span>|<span data-ttu-id="558b3-131">String</span><span class="sxs-lookup"><span data-stu-id="558b3-131">String</span></span>|<span data-ttu-id="558b3-132">用户在 Microsoft Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="558b3-132">The time zone that the user sets in Microsoft Outlook calendar is used for the computation.</span></span> <span data-ttu-id="558b3-133">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="558b3-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="558b3-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="558b3-134">afterHours</span></span>|<span data-ttu-id="558b3-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="558b3-135">Duration</span></span>|<span data-ttu-id="558b3-136">在工作时间之外的呼叫上花费的时间, 基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="558b3-136">Time spent on calls outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="558b3-137">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="558b3-137">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="558b3-138">关系</span><span class="sxs-lookup"><span data-stu-id="558b3-138">Relationships</span></span>

<span data-ttu-id="558b3-139">无</span><span class="sxs-lookup"><span data-stu-id="558b3-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="558b3-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="558b3-140">JSON representation</span></span>

<span data-ttu-id="558b3-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="558b3-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->