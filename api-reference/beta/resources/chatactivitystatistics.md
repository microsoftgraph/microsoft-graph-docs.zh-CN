---
title: chatActivityStatistics 资源类型
description: 表示有关用户的聊天活动的信息。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a380ef18435ca971da4f3163fc1268ec7f28e565
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064344"
---
# <a name="chatactivitystatistics-resource-type"></a><span data-ttu-id="ca225-103">chatActivityStatistics 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca225-103">chatActivityStatistics resource type</span></span>

<span data-ttu-id="ca225-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca225-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca225-105">表示有关用户在 Microsoft 团队或 Skype for business 上的聊天活动中花费的时间的数据。</span><span class="sxs-lookup"><span data-stu-id="ca225-105">Represents data about the user's time spent in chat activities on Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="ca225-106">这基于 [activityStatistics](../resources/activitystatistics.md)。</span><span class="sxs-lookup"><span data-stu-id="ca225-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ca225-107">属性</span><span class="sxs-lookup"><span data-stu-id="ca225-107">Properties</span></span>

| <span data-ttu-id="ca225-108">属性</span><span class="sxs-lookup"><span data-stu-id="ca225-108">Property</span></span>     | <span data-ttu-id="ca225-109">类型</span><span class="sxs-lookup"><span data-stu-id="ca225-109">Type</span></span>        | <span data-ttu-id="ca225-110">说明</span><span class="sxs-lookup"><span data-stu-id="ca225-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca225-111">activity</span><span class="sxs-lookup"><span data-stu-id="ca225-111">activity</span></span>|<span data-ttu-id="ca225-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="ca225-112">analyticsActivityType</span></span>| <span data-ttu-id="ca225-113">将返回其统计信息的聊天活动。</span><span class="sxs-lookup"><span data-stu-id="ca225-113">Chat activity for which statistics are returned.</span></span>|
|<span data-ttu-id="ca225-114">duration</span><span class="sxs-lookup"><span data-stu-id="ca225-114">duration</span></span>|<span data-ttu-id="ca225-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="ca225-115">Duration</span></span>|<span data-ttu-id="ca225-116">在聊天上花费的总小时数。</span><span class="sxs-lookup"><span data-stu-id="ca225-116">Total hours spent on chats.</span></span> <span data-ttu-id="ca225-117">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="ca225-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="ca225-118">endDate</span><span class="sxs-lookup"><span data-stu-id="ca225-118">endDate</span></span>|<span data-ttu-id="ca225-119">日期</span><span class="sxs-lookup"><span data-stu-id="ca225-119">Date</span></span>|<span data-ttu-id="ca225-120">聊天活动结束的日期。</span><span class="sxs-lookup"><span data-stu-id="ca225-120">Date when the chat activity ended.</span></span> <span data-ttu-id="ca225-121">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="ca225-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="ca225-122">例如，属性值可以是 "2019-07-04"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="ca225-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="ca225-123">id</span><span class="sxs-lookup"><span data-stu-id="ca225-123">id</span></span>|<span data-ttu-id="ca225-124">String</span><span class="sxs-lookup"><span data-stu-id="ca225-124">String</span></span>| <span data-ttu-id="ca225-125">聊天活动的只读 ID。</span><span class="sxs-lookup"><span data-stu-id="ca225-125">Read-only ID for the chat activity.</span></span>|
|<span data-ttu-id="ca225-126">startDate</span><span class="sxs-lookup"><span data-stu-id="ca225-126">startDate</span></span>|<span data-ttu-id="ca225-127">日期</span><span class="sxs-lookup"><span data-stu-id="ca225-127">Date</span></span>|<span data-ttu-id="ca225-128">聊天活动的开始日期。</span><span class="sxs-lookup"><span data-stu-id="ca225-128">Date when the chat activity started.</span></span> <span data-ttu-id="ca225-129">对于日历日期，该值以 ISO 8601 格式表示。</span><span class="sxs-lookup"><span data-stu-id="ca225-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="ca225-130">例如，属性值可以是 "2019-07-03"，它遵循 YYYY-MM-DD 格式。</span><span class="sxs-lookup"><span data-stu-id="ca225-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="ca225-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="ca225-131">timeZoneUsed</span></span>|<span data-ttu-id="ca225-132">String</span><span class="sxs-lookup"><span data-stu-id="ca225-132">String</span></span>|<span data-ttu-id="ca225-133">用户在 Outlook 日历中设置的时区用于计算。</span><span class="sxs-lookup"><span data-stu-id="ca225-133">The time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="ca225-134">例如，属性值可以是 "太平洋标准时间"。</span><span class="sxs-lookup"><span data-stu-id="ca225-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="ca225-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="ca225-135">afterHours</span></span>|<span data-ttu-id="ca225-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="ca225-136">Duration</span></span>|<span data-ttu-id="ca225-137">在工作时间之外的聊天上花费的时间，基于用户的 Microsoft Outlook 日历设置的工作时间。</span><span class="sxs-lookup"><span data-stu-id="ca225-137">Time spent on chats outside of working hours, which is based on the user's Microsoft Outlook calendar setting for work hours.</span></span> <span data-ttu-id="ca225-138">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="ca225-138">The value is represented in ISO 8601 format for durations.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ca225-139">关系</span><span class="sxs-lookup"><span data-stu-id="ca225-139">Relationships</span></span>

<span data-ttu-id="ca225-140">无</span><span class="sxs-lookup"><span data-stu-id="ca225-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca225-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca225-141">JSON representation</span></span>

<span data-ttu-id="ca225-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca225-142">The following is a JSON representation of the resource.</span></span>

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



