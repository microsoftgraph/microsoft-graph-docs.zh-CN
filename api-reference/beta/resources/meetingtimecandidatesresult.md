---
title: meetingTimeCandidatesResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: ffa8ec3c423da5d94daff4b95cdac52cd511da9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985086"
---
# <a name="meetingtimecandidatesresult-resource-type"></a><span data-ttu-id="cb769-103">meetingTimeCandidatesResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb769-103">meetingTimeCandidatesResult resource type</span></span>

> <span data-ttu-id="cb769-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cb769-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb769-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb769-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb769-106">一组会议时间建议（若有）；如果没有建议，则返回原因。</span><span class="sxs-lookup"><span data-stu-id="cb769-106">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="cb769-107">下面介绍了 [findMeetingTimes](../api/user-findmeetingtimes.md) 未返回任何会议时间建议的可能原因。</span><span class="sxs-lookup"><span data-stu-id="cb769-107">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="cb769-108">**emptySuggestionsHint 值**</span><span class="sxs-lookup"><span data-stu-id="cb769-108">**emptySuggestionsHint value**</span></span>|<span data-ttu-id="cb769-109">**原因**</span><span class="sxs-lookup"><span data-stu-id="cb769-109">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="cb769-110">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="cb769-110">attendeesUnavailable</span></span> | <span data-ttu-id="cb769-111">所有与会者的忙/闲状态均已知，但任意时间段的与会者出席可能性达不到会议置信度阈值（默认为 50%）。</span><span class="sxs-lookup"><span data-stu-id="cb769-111">All of the attendees' availability is known, but not enough attendees are available to reach the meeting confidence threshold, which is 50% by default, for any time period.</span></span> <span data-ttu-id="cb769-112">此阈值基于与会者的忙/闲状态的建议会议的时间段，对应于 100%有机会在出勤、 未知的状态 50%，以及忙状态 0%的与会者的免费状态。</span><span class="sxs-lookup"><span data-stu-id="cb769-112">This threshold is based on the attendees' free/busy status for a suggested meeting time period, with an attendee's free status corresponding to 100% chance of attendance, unknown status 50%, and busy status 0%.</span></span>|
| <span data-ttu-id="cb769-113">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="cb769-113">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="cb769-p103">部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。</span><span class="sxs-lookup"><span data-stu-id="cb769-p103">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="cb769-116">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="cb769-116">locationsUnavailable</span></span> | <span data-ttu-id="cb769-117">[locationConstraint](locationconstraint.md) 参数的 **isRequired** 属性被指定为必需，但在计算的时间段内尚无可用地点。</span><span class="sxs-lookup"><span data-stu-id="cb769-117">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="cb769-118">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="cb769-118">organizerUnavailable</span></span> | <span data-ttu-id="cb769-119">**isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。</span><span class="sxs-lookup"><span data-stu-id="cb769-119">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="cb769-120">unknown</span><span class="sxs-lookup"><span data-stu-id="cb769-120">unknown</span></span> | <span data-ttu-id="cb769-121">未返回任何会议时间建议的原因未知。</span><span class="sxs-lookup"><span data-stu-id="cb769-121">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb769-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb769-122">JSON representation</span></span>

<span data-ttu-id="cb769-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb769-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeCandidatesResult"
}-->

```json
{
  "emptySuggestionsHint": "String",
  "meetingTimeSlots": [{"@odata.type": "microsoft.graph.meetingTimeCandidate"}]
}

```
## <a name="properties"></a><span data-ttu-id="cb769-124">属性</span><span class="sxs-lookup"><span data-stu-id="cb769-124">Properties</span></span>
| <span data-ttu-id="cb769-125">属性</span><span class="sxs-lookup"><span data-stu-id="cb769-125">Property</span></span>     | <span data-ttu-id="cb769-126">类型</span><span class="sxs-lookup"><span data-stu-id="cb769-126">Type</span></span>   |<span data-ttu-id="cb769-127">Description</span><span class="sxs-lookup"><span data-stu-id="cb769-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb769-128">emptySuggestionsHint</span><span class="sxs-lookup"><span data-stu-id="cb769-128">emptySuggestionsHint</span></span>|<span data-ttu-id="cb769-129">字符串</span><span class="sxs-lookup"><span data-stu-id="cb769-129">String</span></span>|<span data-ttu-id="cb769-p104">未返回任何会议时间建议的原因。可取值为：`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable` 或 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="cb769-p104">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`.</span></span>|
|<span data-ttu-id="cb769-132">meetingTimeSlots</span><span class="sxs-lookup"><span data-stu-id="cb769-132">meetingTimeSlots</span></span>|<span data-ttu-id="cb769-133">[meetingTimeCandidate](meetingtimecandidate.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb769-133">[meetingTimeCandidate](meetingtimecandidate.md) collection</span></span>|<span data-ttu-id="cb769-134">一组会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="cb769-134">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
