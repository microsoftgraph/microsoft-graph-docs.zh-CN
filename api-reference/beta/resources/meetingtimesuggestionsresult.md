---
title: meetingTimeSuggestionsResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
localization_priority: Normal
ms.openlocfilehash: aff5abd69297cd466027c1a614b2609697c00ce6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806837"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="fd7a2-103">meetingTimeSuggestionsResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd7a2-103">meetingTimeSuggestionsResult resource type</span></span>

> <span data-ttu-id="fd7a2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd7a2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd7a2-106">一组会议时间建议（若有）；如果没有建议，则返回原因。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="fd7a2-107">下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="fd7a2-108">**emptySuggestionsReason 值**</span><span class="sxs-lookup"><span data-stu-id="fd7a2-108">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="fd7a2-109">**原因**</span><span class="sxs-lookup"><span data-stu-id="fd7a2-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="fd7a2-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="fd7a2-110">attendeesUnavailable</span></span> | <span data-ttu-id="fd7a2-111">所有与会者的忙/闲状态均已知，但任意时间段的与会者出席可能性达不到[会议置信度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)阈值（默认为 50%）。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-111">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="fd7a2-112">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="fd7a2-112">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="fd7a2-p102">部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-p102">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="fd7a2-115">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="fd7a2-115">locationsUnavailable</span></span> | <span data-ttu-id="fd7a2-116">[locationConstraint](locationconstraint.md) 参数的 **isRequired** 属性被指定为必需，但在计算的时间段内尚无可用地点。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-116">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="fd7a2-117">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="fd7a2-117">organizerUnavailable</span></span> | <span data-ttu-id="fd7a2-118">**isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-118">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="fd7a2-119">unknown</span><span class="sxs-lookup"><span data-stu-id="fd7a2-119">unknown</span></span> | <span data-ttu-id="fd7a2-120">未返回任何会议时间建议的原因未知。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-120">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd7a2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd7a2-121">JSON representation</span></span>

<span data-ttu-id="fd7a2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-122">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="fd7a2-123">属性</span><span class="sxs-lookup"><span data-stu-id="fd7a2-123">Properties</span></span>
| <span data-ttu-id="fd7a2-124">属性</span><span class="sxs-lookup"><span data-stu-id="fd7a2-124">Property</span></span>     | <span data-ttu-id="fd7a2-125">类型</span><span class="sxs-lookup"><span data-stu-id="fd7a2-125">Type</span></span>   |<span data-ttu-id="fd7a2-126">说明</span><span class="sxs-lookup"><span data-stu-id="fd7a2-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd7a2-127">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="fd7a2-127">emptySuggestionsReason</span></span>|<span data-ttu-id="fd7a2-128">String</span><span class="sxs-lookup"><span data-stu-id="fd7a2-128">String</span></span>|<span data-ttu-id="fd7a2-p103">未返回任何会议时间建议的原因。可取值为：`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable` 或 `unknown`。如果 **meetingTimeSuggestions** 属性未包含任何会议建议，则此属性为空字符串。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-p103">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="fd7a2-132">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="fd7a2-132">meetingTimeSuggestions</span></span>|<span data-ttu-id="fd7a2-133">[meetingTimeSuggestion](meetingtimesuggestion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd7a2-133">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="fd7a2-134">一组会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="fd7a2-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
