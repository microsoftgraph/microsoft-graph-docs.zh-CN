---
title: focusActivityStatistics 资源类型
description: 表示有关用户的单个焦点工作的信息
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 11ca850dc7aa24c17f485eb628c7e574bbd4ff4c
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622605"
---
# <a name="focusactivitystatistics-resource-type"></a><span data-ttu-id="7065e-103">focusActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="7065e-103">focusActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7065e-104">表示有关用户可用于焦点工作的时间的数据。</span><span class="sxs-lookup"><span data-stu-id="7065e-104">Represents data about the user's time available for focus work.</span></span> <span data-ttu-id="7065e-105">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="7065e-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7065e-106">属性</span><span class="sxs-lookup"><span data-stu-id="7065e-106">Properties</span></span>

| <span data-ttu-id="7065e-107">属性</span><span class="sxs-lookup"><span data-stu-id="7065e-107">Property</span></span>     | <span data-ttu-id="7065e-108">类型</span><span class="sxs-lookup"><span data-stu-id="7065e-108">Type</span></span>        | <span data-ttu-id="7065e-109">说明</span><span class="sxs-lookup"><span data-stu-id="7065e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7065e-110">activity</span><span class="sxs-lookup"><span data-stu-id="7065e-110">activity</span></span>|<span data-ttu-id="7065e-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="7065e-111">analyticsActivityType</span></span>| <span data-ttu-id="7065e-112">为其返回统计信息的焦点活动。</span><span class="sxs-lookup"><span data-stu-id="7065e-112">Focus activity for which statistics are returned.</span></span>|
|<span data-ttu-id="7065e-113">duration</span><span class="sxs-lookup"><span data-stu-id="7065e-113">duration</span></span>|<span data-ttu-id="7065e-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="7065e-114">Duration</span></span>|<span data-ttu-id="7065e-115">总的工作时间总和 (相当于至少两个连续的小时) 在用户的 Microsoft Outlook 日历中, 在用户设置的工作时间内没有与其他人召开会议。</span><span class="sxs-lookup"><span data-stu-id="7065e-115">Total sum of focus hours, which is equal to all time blocks of at least two consecutive hours, in a user's Microsoft Outlook calendar without a meeting with other people within the user's set work hours.</span></span> <span data-ttu-id="7065e-116">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="7065e-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="7065e-117">endDate</span><span class="sxs-lookup"><span data-stu-id="7065e-117">endDate</span></span>|<span data-ttu-id="7065e-118">Date</span><span class="sxs-lookup"><span data-stu-id="7065e-118">Date</span></span>|<span data-ttu-id="7065e-119">焦点活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="7065e-119">Date when the focus activity ended.</span></span> <span data-ttu-id="7065e-120">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="7065e-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="7065e-121">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="7065e-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="7065e-122">id</span><span class="sxs-lookup"><span data-stu-id="7065e-122">id</span></span>|<span data-ttu-id="7065e-123">String</span><span class="sxs-lookup"><span data-stu-id="7065e-123">String</span></span>| <span data-ttu-id="7065e-124">焦点活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="7065e-124">Read-only ID for the focus activity.</span></span>|
|<span data-ttu-id="7065e-125">startDate</span><span class="sxs-lookup"><span data-stu-id="7065e-125">startDate</span></span>|<span data-ttu-id="7065e-126">日期</span><span class="sxs-lookup"><span data-stu-id="7065e-126">Date</span></span>|<span data-ttu-id="7065e-127">焦点活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="7065e-127">Date when the focus activity started.</span></span> <span data-ttu-id="7065e-128">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="7065e-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="7065e-129">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="7065e-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="7065e-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="7065e-130">timeZoneUsed</span></span>|<span data-ttu-id="7065e-131">String</span><span class="sxs-lookup"><span data-stu-id="7065e-131">String</span></span>|<span data-ttu-id="7065e-132">用户在 Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="7065e-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="7065e-133">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="7065e-133">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="7065e-134">关系</span><span class="sxs-lookup"><span data-stu-id="7065e-134">Relationships</span></span>

<span data-ttu-id="7065e-135">无</span><span class="sxs-lookup"><span data-stu-id="7065e-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7065e-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7065e-136">JSON representation</span></span>

<span data-ttu-id="7065e-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7065e-137">The following is a JSON representation of the resource.</span></span>

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