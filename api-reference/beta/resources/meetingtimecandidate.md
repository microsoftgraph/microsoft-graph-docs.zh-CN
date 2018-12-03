---
title: meetingTimeCandidate 资源类型
description: '会议建议包含类似的会议时间，出勤可能性，个人信息 '
ms.openlocfilehash: 56aae66cf4c532108d2db2f8f4cfc71487f09150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043184"
---
# <a name="meetingtimecandidate-resource-type"></a><span data-ttu-id="42c6f-103">meetingTimeCandidate 资源类型</span><span class="sxs-lookup"><span data-stu-id="42c6f-103">meetingTimeCandidate resource type</span></span>

> <span data-ttu-id="42c6f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42c6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42c6f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42c6f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42c6f-106">会议时间建议包括会议时间、出席可能性、个人忙/闲状态和可用会议地点等信息。</span><span class="sxs-lookup"><span data-stu-id="42c6f-106">A meeting suggestion that includes information like meeting time, attendance likelihood, individual availability, and available meeting locations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42c6f-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42c6f-107">JSON representation</span></span>

<span data-ttu-id="42c6f-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42c6f-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidate"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 1024.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "organizerAvailability": "String",
  "suggestionHint": "String"
}

```
## <a name="properties"></a><span data-ttu-id="42c6f-109">属性</span><span class="sxs-lookup"><span data-stu-id="42c6f-109">Properties</span></span>
| <span data-ttu-id="42c6f-110">属性</span><span class="sxs-lookup"><span data-stu-id="42c6f-110">Property</span></span>     | <span data-ttu-id="42c6f-111">类型</span><span class="sxs-lookup"><span data-stu-id="42c6f-111">Type</span></span>   |<span data-ttu-id="42c6f-112">说明</span><span class="sxs-lookup"><span data-stu-id="42c6f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42c6f-113">attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="42c6f-113">attendeeAvailability</span></span>|<span data-ttu-id="42c6f-114">[attendeeAvailability](attendeeavailability.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42c6f-114">[attendeeAvailability](attendeeavailability.md) collection</span></span>|<span data-ttu-id="42c6f-115">显示此会议时间建议中各个与会者的忙/闲状态的数组。</span><span class="sxs-lookup"><span data-stu-id="42c6f-115">An array that shows the availability status of each attendee for this meeting suggestion.</span></span>|
|<span data-ttu-id="42c6f-116">confidence</span><span class="sxs-lookup"><span data-stu-id="42c6f-116">confidence</span></span>|<span data-ttu-id="42c6f-117">Double</span><span class="sxs-lookup"><span data-stu-id="42c6f-117">Double</span></span>|<span data-ttu-id="42c6f-118">表示所有与会者的出席可能性的百分比值。</span><span class="sxs-lookup"><span data-stu-id="42c6f-118">A percentage that represents the likelhood of all the attendees attending.</span></span>|
|<span data-ttu-id="42c6f-119">locations</span><span class="sxs-lookup"><span data-stu-id="42c6f-119">locations</span></span>|<span data-ttu-id="42c6f-120">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42c6f-120">[location](location.md) collection</span></span>|<span data-ttu-id="42c6f-121">指定此会议时间建议中各个会议地点的名称和地理位置的数组。</span><span class="sxs-lookup"><span data-stu-id="42c6f-121">An array that specifies the name and geographic location of each meeting location for this meeting suggestion.</span></span>|
|<span data-ttu-id="42c6f-122">meetingTimeSlot</span><span class="sxs-lookup"><span data-stu-id="42c6f-122">meetingTimeSlot</span></span>|[<span data-ttu-id="42c6f-123">timeSlot</span><span class="sxs-lookup"><span data-stu-id="42c6f-123">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="42c6f-124">建议的会议时间段。</span><span class="sxs-lookup"><span data-stu-id="42c6f-124">A time period suggested for the meeting.</span></span>|
|<span data-ttu-id="42c6f-125">organizerAvailability</span><span class="sxs-lookup"><span data-stu-id="42c6f-125">organizerAvailability</span></span>|<span data-ttu-id="42c6f-126">字符串</span><span class="sxs-lookup"><span data-stu-id="42c6f-126">String</span></span>| <span data-ttu-id="42c6f-p102">此会议时间建议中会议组织者的忙/闲状态。可取值为：`free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="42c6f-p102">Availability of the meeting organizer for this meeting suggestion. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="42c6f-129">suggestionHint</span><span class="sxs-lookup"><span data-stu-id="42c6f-129">suggestionHint</span></span>|<span data-ttu-id="42c6f-130">String</span><span class="sxs-lookup"><span data-stu-id="42c6f-130">String</span></span>|<span data-ttu-id="42c6f-131">会议时间建议的理由。</span><span class="sxs-lookup"><span data-stu-id="42c6f-131">Reason for suggesting the meeting time.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->