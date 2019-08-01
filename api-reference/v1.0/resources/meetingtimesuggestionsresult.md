---
title: meetingTimeSuggestionsResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2c5e7461b27168150c21f8fedd5d697e2b8ec5e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036195"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="c20f7-103">meetingTimeSuggestionsResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="c20f7-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="c20f7-104">一组会议时间建议（若有）；如果没有建议，则返回原因。</span><span class="sxs-lookup"><span data-stu-id="c20f7-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="c20f7-105">下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。</span><span class="sxs-lookup"><span data-stu-id="c20f7-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="c20f7-106">**emptySuggestionsReason 值**</span><span class="sxs-lookup"><span data-stu-id="c20f7-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="c20f7-107">**原因**</span><span class="sxs-lookup"><span data-stu-id="c20f7-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="c20f7-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="c20f7-108">attendeesUnavailable</span></span> | <span data-ttu-id="c20f7-109">所有与会者的可用性都是已知的, 但没有足够的与会者可以达到[会议可信度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)阈值, 默认情况下, 在任何时间段中, 默认为 50%。</span><span class="sxs-lookup"><span data-stu-id="c20f7-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="c20f7-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="c20f7-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="c20f7-p101">部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。</span><span class="sxs-lookup"><span data-stu-id="c20f7-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="c20f7-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="c20f7-113">locationsUnavailable</span></span> | <span data-ttu-id="c20f7-114">**locationConstraint** 参数的 [isRequired](locationconstraint.md) 属性被指定为必需，但在计算的时间段内尚无可用地点。</span><span class="sxs-lookup"><span data-stu-id="c20f7-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="c20f7-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="c20f7-115">organizerUnavailable</span></span> | <span data-ttu-id="c20f7-116">**isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。</span><span class="sxs-lookup"><span data-stu-id="c20f7-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="c20f7-117">unknown</span><span class="sxs-lookup"><span data-stu-id="c20f7-117">unknown</span></span> | <span data-ttu-id="c20f7-118">未返回任何会议时间建议的原因未知。</span><span class="sxs-lookup"><span data-stu-id="c20f7-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c20f7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c20f7-119">JSON representation</span></span>

<span data-ttu-id="c20f7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c20f7-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a><span data-ttu-id="c20f7-121">属性</span><span class="sxs-lookup"><span data-stu-id="c20f7-121">Properties</span></span>
| <span data-ttu-id="c20f7-122">属性</span><span class="sxs-lookup"><span data-stu-id="c20f7-122">Property</span></span>     | <span data-ttu-id="c20f7-123">类型</span><span class="sxs-lookup"><span data-stu-id="c20f7-123">Type</span></span>   |<span data-ttu-id="c20f7-124">说明</span><span class="sxs-lookup"><span data-stu-id="c20f7-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c20f7-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="c20f7-125">emptySuggestionsReason</span></span>|<span data-ttu-id="c20f7-126">String</span><span class="sxs-lookup"><span data-stu-id="c20f7-126">String</span></span>|<span data-ttu-id="c20f7-127">未返回任何会议时间建议的原因。</span><span class="sxs-lookup"><span data-stu-id="c20f7-127">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="c20f7-128">可能的值为: `attendeesUnavailable`、 `attendeesUnavailableOrUnknown`、 `locationsUnavailable` `organizerUnavailable`、或`unknown`。</span><span class="sxs-lookup"><span data-stu-id="c20f7-128">The possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="c20f7-129">如果**meetingTimeSuggestions**属性包含任何会议建议, 则此属性为空字符串。</span><span class="sxs-lookup"><span data-stu-id="c20f7-129">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="c20f7-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="c20f7-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="c20f7-131">[meetingTimeSuggestion](meetingtimesuggestion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c20f7-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="c20f7-132">一组会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="c20f7-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
