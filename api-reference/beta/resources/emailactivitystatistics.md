---
title: emailActivityStatistics 资源类型
description: 表示有关用户的电子邮件活动的其他信息
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: af0fbc4247e7ffc9c8285409789d0437d8e09cb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055510"
---
# <a name="emailactivitystatistics-resource-type"></a><span data-ttu-id="54f31-103">emailActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="54f31-103">emailActivityStatistics resource type</span></span>

<span data-ttu-id="54f31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54f31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54f31-105">表示有关用户在 Microsoft Outlook 的电子邮件活动中所用时间的数据。</span><span class="sxs-lookup"><span data-stu-id="54f31-105">Represents data about the user's time spent in email activities in Microsoft Outlook.</span></span> <span data-ttu-id="54f31-106">这基于 [activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="54f31-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="54f31-107">属性</span><span class="sxs-lookup"><span data-stu-id="54f31-107">Properties</span></span>

| <span data-ttu-id="54f31-108">属性</span><span class="sxs-lookup"><span data-stu-id="54f31-108">Property</span></span>     | <span data-ttu-id="54f31-109">类型</span><span class="sxs-lookup"><span data-stu-id="54f31-109">Type</span></span>        | <span data-ttu-id="54f31-110">说明</span><span class="sxs-lookup"><span data-stu-id="54f31-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54f31-111">activity</span><span class="sxs-lookup"><span data-stu-id="54f31-111">activity</span></span>|<span data-ttu-id="54f31-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="54f31-112">analyticsActivityType</span></span>| <span data-ttu-id="54f31-113">返回其统计信息的电子邮件活动。</span><span class="sxs-lookup"><span data-stu-id="54f31-113">Email activity for which statistics are returned.</span></span>|
|<span data-ttu-id="54f31-114">duration</span><span class="sxs-lookup"><span data-stu-id="54f31-114">duration</span></span>|<span data-ttu-id="54f31-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="54f31-115">Duration</span></span>|<span data-ttu-id="54f31-116">在电子邮件上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="54f31-116">Total hours spent on emails.</span></span> <span data-ttu-id="54f31-117">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="54f31-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="54f31-118">endDate</span><span class="sxs-lookup"><span data-stu-id="54f31-118">endDate</span></span>|<span data-ttu-id="54f31-119">日期</span><span class="sxs-lookup"><span data-stu-id="54f31-119">Date</span></span>|<span data-ttu-id="54f31-120">电子邮件活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="54f31-120">Date when the email activity ended.</span></span> <span data-ttu-id="54f31-121">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="54f31-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="54f31-122">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="54f31-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="54f31-123">id</span><span class="sxs-lookup"><span data-stu-id="54f31-123">id</span></span>|<span data-ttu-id="54f31-124">String</span><span class="sxs-lookup"><span data-stu-id="54f31-124">String</span></span>| <span data-ttu-id="54f31-125">电子邮件活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="54f31-125">Read-only ID for the email activity.</span></span>|
|<span data-ttu-id="54f31-126">startDate</span><span class="sxs-lookup"><span data-stu-id="54f31-126">startDate</span></span>|<span data-ttu-id="54f31-127">日期</span><span class="sxs-lookup"><span data-stu-id="54f31-127">Date</span></span>|<span data-ttu-id="54f31-128">电子邮件活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="54f31-128">Date when the email activity started.</span></span> <span data-ttu-id="54f31-129">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="54f31-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="54f31-130">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="54f31-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="54f31-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="54f31-131">timeZoneUsed</span></span>|<span data-ttu-id="54f31-132">String</span><span class="sxs-lookup"><span data-stu-id="54f31-132">String</span></span>|<span data-ttu-id="54f31-133">用户在 Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="54f31-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="54f31-134">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="54f31-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="54f31-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="54f31-135">afterHours</span></span>|<span data-ttu-id="54f31-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="54f31-136">Duration</span></span>|<span data-ttu-id="54f31-137">在工作时间之外的电子邮件上花费的总小时数，基于用户的 Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="54f31-137">Total hours spent on email outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="54f31-138">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="54f31-138">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="54f31-139">readEmail</span><span class="sxs-lookup"><span data-stu-id="54f31-139">readEmail</span></span>|<span data-ttu-id="54f31-140">持续时间</span><span class="sxs-lookup"><span data-stu-id="54f31-140">Duration</span></span>|<span data-ttu-id="54f31-141">阅读电子邮件所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="54f31-141">Total hours spent reading email.</span></span> <span data-ttu-id="54f31-142">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="54f31-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="54f31-143">sentEmail</span><span class="sxs-lookup"><span data-stu-id="54f31-143">sentEmail</span></span>|<span data-ttu-id="54f31-144">持续时间</span><span class="sxs-lookup"><span data-stu-id="54f31-144">Duration</span></span>|<span data-ttu-id="54f31-145">撰写和发送电子邮件所用的总小时数。</span><span class="sxs-lookup"><span data-stu-id="54f31-145">Total hours spent writing and sending email.</span></span> <span data-ttu-id="54f31-146">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="54f31-146">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54f31-147">关系</span><span class="sxs-lookup"><span data-stu-id="54f31-147">Relationships</span></span>

<span data-ttu-id="54f31-148">无</span><span class="sxs-lookup"><span data-stu-id="54f31-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54f31-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54f31-149">JSON representation</span></span>

<span data-ttu-id="54f31-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54f31-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

