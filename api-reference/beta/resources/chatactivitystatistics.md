---
title: chatActivityStatistics 资源类型
description: 表示有关用户的聊天活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 05003110c397932f27e700c119f3926b44fe7c31
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622640"
---
# <a name="chatactivitystatistics-resource-type"></a><span data-ttu-id="ade34-103">chatActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="ade34-103">chatActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade34-104">表示有关用户在 Microsoft 团队或 Skype for business 上的聊天活动中花费的时间的数据。</span><span class="sxs-lookup"><span data-stu-id="ade34-104">Represents data about the user's time spent in chat activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="ade34-105">这基于[activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="ade34-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ade34-106">属性</span><span class="sxs-lookup"><span data-stu-id="ade34-106">Properties</span></span>

| <span data-ttu-id="ade34-107">属性</span><span class="sxs-lookup"><span data-stu-id="ade34-107">Property</span></span>     | <span data-ttu-id="ade34-108">类型</span><span class="sxs-lookup"><span data-stu-id="ade34-108">Type</span></span>        | <span data-ttu-id="ade34-109">说明</span><span class="sxs-lookup"><span data-stu-id="ade34-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ade34-110">activity</span><span class="sxs-lookup"><span data-stu-id="ade34-110">activity</span></span>|<span data-ttu-id="ade34-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="ade34-111">analyticsActivityType</span></span>| <span data-ttu-id="ade34-112">将返回其统计信息的聊天活动。</span><span class="sxs-lookup"><span data-stu-id="ade34-112">Chat activity for which statistics are returned.</span></span>|
|<span data-ttu-id="ade34-113">duration</span><span class="sxs-lookup"><span data-stu-id="ade34-113">duration</span></span>|<span data-ttu-id="ade34-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="ade34-114">Duration</span></span>|<span data-ttu-id="ade34-115">在聊天上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="ade34-115">Total hours spent on chats.</span></span> <span data-ttu-id="ade34-116">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="ade34-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="ade34-117">endDate</span><span class="sxs-lookup"><span data-stu-id="ade34-117">endDate</span></span>|<span data-ttu-id="ade34-118">Date</span><span class="sxs-lookup"><span data-stu-id="ade34-118">Date</span></span>|<span data-ttu-id="ade34-119">聊天活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="ade34-119">Date when the chat activity ended.</span></span> <span data-ttu-id="ade34-120">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="ade34-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="ade34-121">例如, 属性值可以是 "2019-07-04", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="ade34-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="ade34-122">id</span><span class="sxs-lookup"><span data-stu-id="ade34-122">id</span></span>|<span data-ttu-id="ade34-123">String</span><span class="sxs-lookup"><span data-stu-id="ade34-123">String</span></span>| <span data-ttu-id="ade34-124">聊天活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="ade34-124">Read-only ID for the chat activity.</span></span>|
|<span data-ttu-id="ade34-125">startDate</span><span class="sxs-lookup"><span data-stu-id="ade34-125">startDate</span></span>|<span data-ttu-id="ade34-126">日期</span><span class="sxs-lookup"><span data-stu-id="ade34-126">Date</span></span>|<span data-ttu-id="ade34-127">聊天活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="ade34-127">Date when the chat activity started.</span></span> <span data-ttu-id="ade34-128">对于日历日期, 该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="ade34-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="ade34-129">例如, 属性值可以是 "2019-07-03", 它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="ade34-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="ade34-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="ade34-130">timeZoneUsed</span></span>|<span data-ttu-id="ade34-131">String</span><span class="sxs-lookup"><span data-stu-id="ade34-131">String</span></span>|<span data-ttu-id="ade34-132">用户在 Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="ade34-132">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="ade34-133">例如, 属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="ade34-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="ade34-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="ade34-134">afterHours</span></span>|<span data-ttu-id="ade34-135">持续时间</span><span class="sxs-lookup"><span data-stu-id="ade34-135">Duration</span></span>|<span data-ttu-id="ade34-136">在工作时间之外的聊天上花费的时间, 基于用户的 Microsoft Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="ade34-136">Time spent on chats outside of working hours, which is based on the user's Microsoft Outlook calendar setting for work hours.</span></span> <span data-ttu-id="ade34-137">值以 ISO 8601 格式表示, 持续时间。</span><span class="sxs-lookup"><span data-stu-id="ade34-137">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ade34-138">关系</span><span class="sxs-lookup"><span data-stu-id="ade34-138">Relationships</span></span>

<span data-ttu-id="ade34-139">无</span><span class="sxs-lookup"><span data-stu-id="ade34-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ade34-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ade34-140">JSON representation</span></span>

<span data-ttu-id="ade34-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ade34-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatActivityStatistics"
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
  "description": "chatActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

