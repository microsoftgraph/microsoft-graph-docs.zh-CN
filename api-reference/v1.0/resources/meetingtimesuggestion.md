---
title: meetingTimeSuggestion 资源类型
description: '包含会议时间、出席可能性、个人信息的会议建议 '
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5340fa9912ecb183dda8603d4b3ce4bbf6d70e8d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474699"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="97e35-103">meetingTimeSuggestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="97e35-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="97e35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97e35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97e35-105">会议时间建议包括会议时间、出席可能性、个人忙/闲状态和可用会议地点等信息。</span><span class="sxs-lookup"><span data-stu-id="97e35-105">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97e35-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97e35-106">JSON representation</span></span>

<span data-ttu-id="97e35-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97e35-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="97e35-108">属性</span><span class="sxs-lookup"><span data-stu-id="97e35-108">Properties</span></span>
| <span data-ttu-id="97e35-109">属性</span><span class="sxs-lookup"><span data-stu-id="97e35-109">Property</span></span>     | <span data-ttu-id="97e35-110">类型</span><span class="sxs-lookup"><span data-stu-id="97e35-110">Type</span></span>   |<span data-ttu-id="97e35-111">说明</span><span class="sxs-lookup"><span data-stu-id="97e35-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97e35-112">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="97e35-112">attendeeAvailability</span></span>|<span data-ttu-id="97e35-113">[attendeeAvailability](attendeeavailability.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97e35-113">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="97e35-114">显示此会议时间建议中各个与会者的忙/闲状态的数组。</span><span class="sxs-lookup"><span data-stu-id="97e35-114">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="97e35-115">confidence</span><span class="sxs-lookup"><span data-stu-id="97e35-115">confidence</span></span>|<span data-ttu-id="97e35-116">Double</span><span class="sxs-lookup"><span data-stu-id="97e35-116">Double</span></span>|<span data-ttu-id="97e35-117">表示所有与会者的出席可能性的百分比值。</span><span class="sxs-lookup"><span data-stu-id="97e35-117">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="97e35-118">locations</span><span class="sxs-lookup"><span data-stu-id="97e35-118">locations</span></span>|<span data-ttu-id="97e35-119">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97e35-119">[location](location.md) collection</span></span>|<span data-ttu-id="97e35-120">指定此会议时间建议中各个会议地点的名称和地理位置的数组。</span><span class="sxs-lookup"><span data-stu-id="97e35-120">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="97e35-121">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="97e35-121">meetingTimeSlot</span></span>|[<span data-ttu-id="97e35-122">timeSlot</span><span class="sxs-lookup"><span data-stu-id="97e35-122">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="97e35-123">建议的会议时间段。</span><span class="sxs-lookup"><span data-stu-id="97e35-123">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="97e35-124">order</span><span class="sxs-lookup"><span data-stu-id="97e35-124">order</span></span>|<span data-ttu-id="97e35-125">Int32</span><span class="sxs-lookup"><span data-stu-id="97e35-125">Int32</span></span>|<span data-ttu-id="97e35-126">会议时间建议的顺序，按计算可信度值从高到低排序，如果建议具有相同的置信度，则按时间顺序排序。</span><span class="sxs-lookup"><span data-stu-id="97e35-126">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="97e35-127">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="97e35-127">organizerAvailability</span></span>|<span data-ttu-id="97e35-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="97e35-128">freeBusyStatus</span></span>| <span data-ttu-id="97e35-129">此会议时间建议中会议组织者的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="97e35-129">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="97e35-130">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="97e35-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="97e35-131">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="97e35-131">suggestionReason</span></span>|<span data-ttu-id="97e35-132">String</span><span class="sxs-lookup"><span data-stu-id="97e35-132">String</span></span>|<span data-ttu-id="97e35-133">会议时间建议的理由。</span><span class="sxs-lookup"><span data-stu-id="97e35-133">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

