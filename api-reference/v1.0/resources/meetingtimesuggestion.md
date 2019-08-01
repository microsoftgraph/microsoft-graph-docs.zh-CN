---
title: meetingTimeSuggestion 资源类型
description: '会议建议, 其中包含会议时间、出勤可能性、个人等信息 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 723468d14ebd089d8ed5b020f56e0c70c426ed9b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036202"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="af2bb-103">meetingTimeSuggestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="af2bb-103">meetingTimeSuggestion resource type</span></span>

<span data-ttu-id="af2bb-104">会议时间建议包括会议时间、出席可能性、个人忙/闲状态和可用会议地点等信息。</span><span class="sxs-lookup"><span data-stu-id="af2bb-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af2bb-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af2bb-105">JSON representation</span></span>

<span data-ttu-id="af2bb-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af2bb-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="af2bb-107">属性</span><span class="sxs-lookup"><span data-stu-id="af2bb-107">Properties</span></span>
| <span data-ttu-id="af2bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="af2bb-108">Property</span></span>     | <span data-ttu-id="af2bb-109">类型</span><span class="sxs-lookup"><span data-stu-id="af2bb-109">Type</span></span>   |<span data-ttu-id="af2bb-110">说明</span><span class="sxs-lookup"><span data-stu-id="af2bb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af2bb-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="af2bb-111">attendeeAvailability</span></span>|<span data-ttu-id="af2bb-112">[attendeeAvailability](attendeeavailability.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2bb-112">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="af2bb-113">显示此会议时间建议中各个与会者的忙/闲状态的数组。</span><span class="sxs-lookup"><span data-stu-id="af2bb-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="af2bb-114">confidence</span><span class="sxs-lookup"><span data-stu-id="af2bb-114">confidence</span></span>|<span data-ttu-id="af2bb-115">Double</span><span class="sxs-lookup"><span data-stu-id="af2bb-115">Double</span></span>|<span data-ttu-id="af2bb-116">表示所有与会者的出席可能性的百分比值。</span><span class="sxs-lookup"><span data-stu-id="af2bb-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="af2bb-117">locations</span><span class="sxs-lookup"><span data-stu-id="af2bb-117">locations</span></span>|<span data-ttu-id="af2bb-118">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2bb-118">[location](location.md) collection</span></span>|<span data-ttu-id="af2bb-119">指定此会议时间建议中各个会议地点的名称和地理位置的数组。</span><span class="sxs-lookup"><span data-stu-id="af2bb-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="af2bb-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="af2bb-120">meetingTimeSlot</span></span>|[<span data-ttu-id="af2bb-121">timeSlot</span><span class="sxs-lookup"><span data-stu-id="af2bb-121">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="af2bb-122">建议的会议时间段。</span><span class="sxs-lookup"><span data-stu-id="af2bb-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="af2bb-123">顺序</span><span class="sxs-lookup"><span data-stu-id="af2bb-123">order</span></span>|<span data-ttu-id="af2bb-124">Int32</span><span class="sxs-lookup"><span data-stu-id="af2bb-124">Int32</span></span>|<span data-ttu-id="af2bb-125">会议时间建议的顺序按其计算可信度值 (从高到低) 进行排序, 然后按 chronology (如果有相同可信度的建议)。</span><span class="sxs-lookup"><span data-stu-id="af2bb-125">Order of meeting time suggestions sorted by their computed confidence value from high to low, then by chronology if there are suggestions with the same confidence.</span></span> |
|<span data-ttu-id="af2bb-126">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="af2bb-126">organizerAvailability</span></span>|<span data-ttu-id="af2bb-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="af2bb-127">freeBusyStatus</span></span>| <span data-ttu-id="af2bb-128">此会议时间建议中会议组织者的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="af2bb-128">Availability of the meeting organizer for this meeting suggestion.</span></span> <span data-ttu-id="af2bb-129">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="af2bb-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="af2bb-130">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="af2bb-130">suggestionReason</span></span>|<span data-ttu-id="af2bb-131">String</span><span class="sxs-lookup"><span data-stu-id="af2bb-131">String</span></span>|<span data-ttu-id="af2bb-132">会议时间建议的理由。</span><span class="sxs-lookup"><span data-stu-id="af2bb-132">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
