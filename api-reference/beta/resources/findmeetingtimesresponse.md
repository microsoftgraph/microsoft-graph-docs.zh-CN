---
title: findMeetingTimesResponse 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0d52da8e5798932d4f78463d6e4bea08ecb7c793
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057345"
---
# <a name="findmeetingtimesresponse-resource-type"></a><span data-ttu-id="22356-103">findMeetingTimesResponse 资源类型</span><span class="sxs-lookup"><span data-stu-id="22356-103">findMeetingTimesResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22356-104">会议建议的集合 (如果有), 如果没有, 则为 "原因"。</span><span class="sxs-lookup"><span data-stu-id="22356-104">A collection of meeting suggestions if there is any, and the reason if there isn't.</span></span>

<span data-ttu-id="22356-105">下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。</span><span class="sxs-lookup"><span data-stu-id="22356-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="22356-106">**emptySuggestionsReason 值**</span><span class="sxs-lookup"><span data-stu-id="22356-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="22356-107">**原因**</span><span class="sxs-lookup"><span data-stu-id="22356-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="22356-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="22356-108">attendeesUnavailable</span></span> | <span data-ttu-id="22356-109">所有与会者的忙/闲状态均已知，但任意时间段的与会者出席可能性达不到[会议置信度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)阈值（默认为 50%）。</span><span class="sxs-lookup"><span data-stu-id="22356-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="22356-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="22356-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="22356-p101">部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。</span><span class="sxs-lookup"><span data-stu-id="22356-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="22356-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="22356-113">locationsUnavailable</span></span> | <span data-ttu-id="22356-114">将**locationConstraint**参数的**isRequired**属性指定为 true, 但在计算的时间段中没有可用的位置。</span><span class="sxs-lookup"><span data-stu-id="22356-114">The **isRequired** property of the **locationConstraint** parameter is specified as true, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="22356-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="22356-115">organizerUnavailable</span></span> | <span data-ttu-id="22356-116">**isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。</span><span class="sxs-lookup"><span data-stu-id="22356-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="22356-117">unknown</span><span class="sxs-lookup"><span data-stu-id="22356-117">unknown</span></span> | <span data-ttu-id="22356-118">未返回任何会议时间建议的原因未知。</span><span class="sxs-lookup"><span data-stu-id="22356-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22356-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22356-119">JSON representation</span></span>

<span data-ttu-id="22356-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22356-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesResponse"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="22356-121">属性</span><span class="sxs-lookup"><span data-stu-id="22356-121">Properties</span></span>
| <span data-ttu-id="22356-122">属性</span><span class="sxs-lookup"><span data-stu-id="22356-122">Property</span></span>     | <span data-ttu-id="22356-123">类型</span><span class="sxs-lookup"><span data-stu-id="22356-123">Type</span></span>   |<span data-ttu-id="22356-124">说明</span><span class="sxs-lookup"><span data-stu-id="22356-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22356-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="22356-125">emptySuggestionsReason</span></span>|<span data-ttu-id="22356-126">String</span><span class="sxs-lookup"><span data-stu-id="22356-126">String</span></span>|<span data-ttu-id="22356-p102">未返回任何会议时间建议的原因。可取值为：`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable` 或 `unknown`。如果 **meetingTimeSuggestions** 属性未包含任何会议建议，则此属性为空字符串。</span><span class="sxs-lookup"><span data-stu-id="22356-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="22356-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="22356-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="22356-131">[meetingTimeSuggestion](meetingtimesuggestion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22356-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="22356-132">一组会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="22356-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimesresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->