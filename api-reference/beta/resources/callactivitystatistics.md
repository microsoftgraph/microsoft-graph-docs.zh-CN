---
title: callActivityStatistics 资源类型
description: 表示有关用户的呼叫活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 03625811beec7df8cd679455e9853ea49edf0ed6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507815"
---
# <a name="callactivitystatistics-resource-type"></a><span data-ttu-id="4bb3e-103">callActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bb3e-103">callActivityStatistics resource type</span></span>

<span data-ttu-id="4bb3e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4bb3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb3e-105">表示有关用户在 Microsoft 团队或 Skype for business 上的呼叫活动中花费的时间的数据。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-105">Represents data about the user's time spent in call activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="4bb3e-106">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4bb3e-107">属性</span><span class="sxs-lookup"><span data-stu-id="4bb3e-107">Properties</span></span>

| <span data-ttu-id="4bb3e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bb3e-108">Property</span></span>     | <span data-ttu-id="4bb3e-109">类型</span><span class="sxs-lookup"><span data-stu-id="4bb3e-109">Type</span></span>        | <span data-ttu-id="4bb3e-110">说明</span><span class="sxs-lookup"><span data-stu-id="4bb3e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4bb3e-111">activity</span><span class="sxs-lookup"><span data-stu-id="4bb3e-111">activity</span></span>|<span data-ttu-id="4bb3e-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="4bb3e-112">analyticsActivityType</span></span>| <span data-ttu-id="4bb3e-113">返回其统计信息的呼叫活动。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-113">Call activity for which statistics are returned.</span></span>|
|<span data-ttu-id="4bb3e-114">duration</span><span class="sxs-lookup"><span data-stu-id="4bb3e-114">duration</span></span>|<span data-ttu-id="4bb3e-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="4bb3e-115">Duration</span></span>|<span data-ttu-id="4bb3e-116">对呼叫花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-116">Total hours spent on calls.</span></span> <span data-ttu-id="4bb3e-117">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="4bb3e-118">endDate</span><span class="sxs-lookup"><span data-stu-id="4bb3e-118">endDate</span></span>|<span data-ttu-id="4bb3e-119">Date</span><span class="sxs-lookup"><span data-stu-id="4bb3e-119">Date</span></span>|<span data-ttu-id="4bb3e-120">呼叫活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-120">Date when the call activity ended.</span></span> <span data-ttu-id="4bb3e-121">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="4bb3e-122">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="4bb3e-123">id</span><span class="sxs-lookup"><span data-stu-id="4bb3e-123">id</span></span>|<span data-ttu-id="4bb3e-124">String</span><span class="sxs-lookup"><span data-stu-id="4bb3e-124">String</span></span>| <span data-ttu-id="4bb3e-125">呼叫活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-125">Read-only ID for the call activity.</span></span>|
|<span data-ttu-id="4bb3e-126">startDate</span><span class="sxs-lookup"><span data-stu-id="4bb3e-126">startDate</span></span>|<span data-ttu-id="4bb3e-127">日期</span><span class="sxs-lookup"><span data-stu-id="4bb3e-127">Date</span></span>|<span data-ttu-id="4bb3e-128">呼叫活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-128">Date when the call activity started.</span></span> <span data-ttu-id="4bb3e-129">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="4bb3e-130">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="4bb3e-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="4bb3e-131">timeZoneUsed</span></span>|<span data-ttu-id="4bb3e-132">String</span><span class="sxs-lookup"><span data-stu-id="4bb3e-132">String</span></span>|<span data-ttu-id="4bb3e-133">用户在 Microsoft Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-133">The time zone that the user sets in Microsoft Outlook calendar is used for the computation.</span></span> <span data-ttu-id="4bb3e-134">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="4bb3e-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="4bb3e-135">afterHours</span></span>|<span data-ttu-id="4bb3e-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="4bb3e-136">Duration</span></span>|<span data-ttu-id="4bb3e-137">在工作时间之外的呼叫上花费的时间，基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-137">Time spent on calls outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="4bb3e-138">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-138">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4bb3e-139">关系</span><span class="sxs-lookup"><span data-stu-id="4bb3e-139">Relationships</span></span>

<span data-ttu-id="4bb3e-140">无</span><span class="sxs-lookup"><span data-stu-id="4bb3e-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bb3e-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bb3e-141">JSON representation</span></span>

<span data-ttu-id="4bb3e-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bb3e-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
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