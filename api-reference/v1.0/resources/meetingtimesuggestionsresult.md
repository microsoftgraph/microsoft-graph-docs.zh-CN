---
title: meetingTimeSuggestionsResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1b30f2ad3d6ebe84ad733b7136cd14f30fef1ea9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472634"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="34d9e-103">meetingTimeSuggestionsResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="34d9e-103">meetingTimeSuggestionsResult resource type</span></span>

<span data-ttu-id="34d9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34d9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34d9e-105">一组会议时间建议（若有）；如果没有建议，则返回原因。</span><span class="sxs-lookup"><span data-stu-id="34d9e-105">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="34d9e-106">下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。</span><span class="sxs-lookup"><span data-stu-id="34d9e-106">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="34d9e-107">**emptySuggestionsReason 值**</span><span class="sxs-lookup"><span data-stu-id="34d9e-107">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="34d9e-108">**原因**</span><span class="sxs-lookup"><span data-stu-id="34d9e-108">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="34d9e-109">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="34d9e-109">attendeesUnavailable</span></span> | <span data-ttu-id="34d9e-110">所有与会者的可用性都是已知的，但没有足够的与会者可用于在任何时段达到会议可信度阈值（默认为[](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)50%。）</span><span class="sxs-lookup"><span data-stu-id="34d9e-110">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="34d9e-111">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="34d9e-111">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="34d9e-p101">部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。</span><span class="sxs-lookup"><span data-stu-id="34d9e-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="34d9e-114">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="34d9e-114">locationsUnavailable</span></span> | <span data-ttu-id="34d9e-115">**locationConstraint** 参数的 [isRequired](locationconstraint.md) 属性被指定为必需，但在计算的时间段内尚无可用地点。</span><span class="sxs-lookup"><span data-stu-id="34d9e-115">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="34d9e-116">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="34d9e-116">organizerUnavailable</span></span> | <span data-ttu-id="34d9e-117">**isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。</span><span class="sxs-lookup"><span data-stu-id="34d9e-117">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="34d9e-118">unknown</span><span class="sxs-lookup"><span data-stu-id="34d9e-118">unknown</span></span> | <span data-ttu-id="34d9e-119">未返回任何会议时间建议的原因未知。</span><span class="sxs-lookup"><span data-stu-id="34d9e-119">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34d9e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34d9e-120">JSON representation</span></span>

<span data-ttu-id="34d9e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34d9e-121">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="34d9e-122">属性</span><span class="sxs-lookup"><span data-stu-id="34d9e-122">Properties</span></span>
| <span data-ttu-id="34d9e-123">属性</span><span class="sxs-lookup"><span data-stu-id="34d9e-123">Property</span></span>     | <span data-ttu-id="34d9e-124">类型</span><span class="sxs-lookup"><span data-stu-id="34d9e-124">Type</span></span>   |<span data-ttu-id="34d9e-125">说明</span><span class="sxs-lookup"><span data-stu-id="34d9e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34d9e-126">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="34d9e-126">emptySuggestionsReason</span></span>|<span data-ttu-id="34d9e-127">String</span><span class="sxs-lookup"><span data-stu-id="34d9e-127">String</span></span>|<span data-ttu-id="34d9e-128">未返回任何会议时间建议的原因。</span><span class="sxs-lookup"><span data-stu-id="34d9e-128">A reason for not returning any meeting suggestions.</span></span> <span data-ttu-id="34d9e-129">可能的值是： `attendeesUnavailable` 、 `attendeesUnavailableOrUnknown` 、 或 `locationsUnavailable` `organizerUnavailable` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="34d9e-129">The possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span> <span data-ttu-id="34d9e-130">如果 **meetingTimeSuggestions** 属性包含任何会议建议，则此属性为空字符串。</span><span class="sxs-lookup"><span data-stu-id="34d9e-130">This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="34d9e-131">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="34d9e-131">meetingTimeSuggestions</span></span>|<span data-ttu-id="34d9e-132">[meetingTimeSuggestion](meetingtimesuggestion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="34d9e-132">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="34d9e-133">一组会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="34d9e-133">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

