---
title: focusActivityStatistics 资源类型
description: 表示有关用户的单个焦点工作的信息
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3da2dc2719f24bfd986d5a3df550b4635b734131
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052878"
---
# <a name="focusactivitystatistics-resource-type"></a><span data-ttu-id="5f705-103">focusActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f705-103">focusActivityStatistics resource type</span></span>

<span data-ttu-id="5f705-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f705-105">表示有关用户可用于焦点工作的时间的数据。</span><span class="sxs-lookup"><span data-stu-id="5f705-105">Represents data about the user's time available for focus work.</span></span> <span data-ttu-id="5f705-106">这基于 [activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="5f705-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5f705-107">属性</span><span class="sxs-lookup"><span data-stu-id="5f705-107">Properties</span></span>

| <span data-ttu-id="5f705-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f705-108">Property</span></span>     | <span data-ttu-id="5f705-109">类型</span><span class="sxs-lookup"><span data-stu-id="5f705-109">Type</span></span>        | <span data-ttu-id="5f705-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f705-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5f705-111">activity</span><span class="sxs-lookup"><span data-stu-id="5f705-111">activity</span></span>|<span data-ttu-id="5f705-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="5f705-112">analyticsActivityType</span></span>| <span data-ttu-id="5f705-113">为其返回统计信息的焦点活动。</span><span class="sxs-lookup"><span data-stu-id="5f705-113">Focus activity for which statistics are returned.</span></span>|
|<span data-ttu-id="5f705-114">duration</span><span class="sxs-lookup"><span data-stu-id="5f705-114">duration</span></span>|<span data-ttu-id="5f705-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="5f705-115">Duration</span></span>|<span data-ttu-id="5f705-116">总的工作时间总和（相当于至少两个连续的小时）在用户的 Microsoft Outlook 日历中，在用户设置的工作时间内没有与其他人召开会议。</span><span class="sxs-lookup"><span data-stu-id="5f705-116">Total sum of focus hours, which is equal to all time blocks of at least two consecutive hours, in a user's Microsoft Outlook calendar without a meeting with other people within the user's set work hours.</span></span> <span data-ttu-id="5f705-117">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="5f705-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="5f705-118">endDate</span><span class="sxs-lookup"><span data-stu-id="5f705-118">endDate</span></span>|<span data-ttu-id="5f705-119">日期</span><span class="sxs-lookup"><span data-stu-id="5f705-119">Date</span></span>|<span data-ttu-id="5f705-120">焦点活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="5f705-120">Date when the focus activity ended.</span></span> <span data-ttu-id="5f705-121">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="5f705-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="5f705-122">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="5f705-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="5f705-123">id</span><span class="sxs-lookup"><span data-stu-id="5f705-123">id</span></span>|<span data-ttu-id="5f705-124">String</span><span class="sxs-lookup"><span data-stu-id="5f705-124">String</span></span>| <span data-ttu-id="5f705-125">焦点活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="5f705-125">Read-only ID for the focus activity.</span></span>|
|<span data-ttu-id="5f705-126">startDate</span><span class="sxs-lookup"><span data-stu-id="5f705-126">startDate</span></span>|<span data-ttu-id="5f705-127">日期</span><span class="sxs-lookup"><span data-stu-id="5f705-127">Date</span></span>|<span data-ttu-id="5f705-128">焦点活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="5f705-128">Date when the focus activity started.</span></span> <span data-ttu-id="5f705-129">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="5f705-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="5f705-130">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="5f705-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="5f705-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="5f705-131">timeZoneUsed</span></span>|<span data-ttu-id="5f705-132">String</span><span class="sxs-lookup"><span data-stu-id="5f705-132">String</span></span>|<span data-ttu-id="5f705-133">用户在 Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="5f705-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="5f705-134">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="5f705-134">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f705-135">关系</span><span class="sxs-lookup"><span data-stu-id="5f705-135">Relationships</span></span>

<span data-ttu-id="5f705-136">无</span><span class="sxs-lookup"><span data-stu-id="5f705-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f705-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f705-137">JSON representation</span></span>

<span data-ttu-id="5f705-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f705-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

