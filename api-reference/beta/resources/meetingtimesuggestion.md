---
title: meetingTimeSuggestion 资源类型
description: '会议建议, 其中包含会议时间、出勤可能性、个人等信息 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 379bb4ac4be8e2d8d1bec494cf4d573550d46b55
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057027"
---
# <a name="meetingtimesuggestion-resource-type"></a><span data-ttu-id="67c05-103">meetingTimeSuggestion 资源类型</span><span class="sxs-lookup"><span data-stu-id="67c05-103">meetingTimeSuggestion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67c05-104">会议时间建议包括会议时间、出席可能性、个人忙/闲状态和可用会议地点等信息。</span><span class="sxs-lookup"><span data-stu-id="67c05-104">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67c05-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67c05-105">JSON representation</span></span>

<span data-ttu-id="67c05-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67c05-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.locationDataModel"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.meetingTimeSlotDataModel"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a><span data-ttu-id="67c05-107">属性</span><span class="sxs-lookup"><span data-stu-id="67c05-107">Properties</span></span>
| <span data-ttu-id="67c05-108">属性</span><span class="sxs-lookup"><span data-stu-id="67c05-108">Property</span></span>     | <span data-ttu-id="67c05-109">类型</span><span class="sxs-lookup"><span data-stu-id="67c05-109">Type</span></span>   |<span data-ttu-id="67c05-110">说明</span><span class="sxs-lookup"><span data-stu-id="67c05-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67c05-111">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="67c05-111">attendeeAvailability</span></span>|<span data-ttu-id="67c05-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md)集合</span><span class="sxs-lookup"><span data-stu-id="67c05-112">[attendeeAvailabilityDataModel](attendeeavailabilitydatamodel.md) collection</span></span>|<span data-ttu-id="67c05-113">显示此会议时间建议中各个与会者的忙/闲状态的数组。</span><span class="sxs-lookup"><span data-stu-id="67c05-113">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="67c05-114">confidence</span><span class="sxs-lookup"><span data-stu-id="67c05-114">confidence</span></span>|<span data-ttu-id="67c05-115">Double</span><span class="sxs-lookup"><span data-stu-id="67c05-115">Double</span></span>|<span data-ttu-id="67c05-116">表示所有与会者的出席可能性的百分比值。</span><span class="sxs-lookup"><span data-stu-id="67c05-116">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="67c05-117">locations</span><span class="sxs-lookup"><span data-stu-id="67c05-117">locations</span></span>|<span data-ttu-id="67c05-118">[locationDataModel](locationdatamodel.md)集合</span><span class="sxs-lookup"><span data-stu-id="67c05-118">[locationDataModel](locationdatamodel.md) collection</span></span>|<span data-ttu-id="67c05-119">指定此会议时间建议中各个会议地点的名称和地理位置的数组。</span><span class="sxs-lookup"><span data-stu-id="67c05-119">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="67c05-120">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="67c05-120">meetingTimeSlot</span></span>|[<span data-ttu-id="67c05-121">meetingTimeSlotDataModel</span><span class="sxs-lookup"><span data-stu-id="67c05-121">meetingTimeSlotDataModel</span></span>](meetingtimeslotdatamodel.md)|<span data-ttu-id="67c05-122">建议的会议时间段。</span><span class="sxs-lookup"><span data-stu-id="67c05-122">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="67c05-123">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="67c05-123">organizerAvailability</span></span>|<span data-ttu-id="67c05-124">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="67c05-124">availabilityStatus</span></span>| <span data-ttu-id="67c05-p101">此会议时间建议中会议组织者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="67c05-p101">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="67c05-127">suggestionReason</span><span class="sxs-lookup"><span data-stu-id="67c05-127">suggestionReason</span></span>|<span data-ttu-id="67c05-128">String</span><span class="sxs-lookup"><span data-stu-id="67c05-128">String</span></span>|<span data-ttu-id="67c05-129">会议时间建议的理由。</span><span class="sxs-lookup"><span data-stu-id="67c05-129">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
