---
title: meetingTimeSuggestionsResult 资源类型
description: 一组会议时间建议（若有）；如果没有建议，则返回原因。
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 9d64fe43ac65e3366975b3981053b6d163d41522
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510818"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a><span data-ttu-id="682cf-103">meetingTimeSuggestionsResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="682cf-103">meetingTimeSuggestionsResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682cf-104">一组会议时间建议（若有）；如果没有建议，则返回原因。</span><span class="sxs-lookup"><span data-stu-id="682cf-104">A collection of meeting suggestions if there is any, or the reason if there isn't.</span></span>

<span data-ttu-id="682cf-105">下面介绍了 findMeetingTimes 未返回任何会议时间建议的可能原因。</span><span class="sxs-lookup"><span data-stu-id="682cf-105">The following are the possible reasons that [findMeetingTimes](../api/user-findmeetingtimes.md) does not return any meeting suggestions.</span></span>

|<span data-ttu-id="682cf-106">emptySuggestionsReason 值</span><span class="sxs-lookup"><span data-stu-id="682cf-106">**emptySuggestionsReason value**</span></span>|<span data-ttu-id="682cf-107">原因</span><span class="sxs-lookup"><span data-stu-id="682cf-107">**Reasons**</span></span>|
|:-----|:-----|
| <span data-ttu-id="682cf-108">attendeesUnavailable</span><span class="sxs-lookup"><span data-stu-id="682cf-108">attendeesUnavailable</span></span> | <span data-ttu-id="682cf-109">所有与会者的忙/闲状态均已知，但任意时间段的与会者出席可能性达不到[会议置信度](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion)阈值（默认为 50%）。</span><span class="sxs-lookup"><span data-stu-id="682cf-109">All of the attendees' availability is known, but not enough attendees are available to reach the [meeting confidence](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) threshold, which is 50% by default, for any time period.</span></span>|
| <span data-ttu-id="682cf-110">attendeesUnavailableOrUnknown</span><span class="sxs-lookup"><span data-stu-id="682cf-110">attendeesUnavailableOrUnknown</span></span> | <span data-ttu-id="682cf-p101">部分或全部与会者的忙/闲状态未知，导致会议置信度下降至设定的阈值（默认为 50%）以下。如果与会者不是组织内部的，或获取忙/闲信息时出错了，与会者的忙/闲状态就会变成未知。</span><span class="sxs-lookup"><span data-stu-id="682cf-p101">Some or all of the attendees have unknown availability, causing the meeting confidence to fall below the set threshold, which is 50% by default. Attendee availability can become unknown if the attendee is outside of the organization, or there is an error obtaining free/busy information.</span></span>|
| <span data-ttu-id="682cf-113">locationsUnavailable</span><span class="sxs-lookup"><span data-stu-id="682cf-113">locationsUnavailable</span></span> | <span data-ttu-id="682cf-114">[locationConstraint](locationconstraint.md) 参数的 **isRequired** 属性被指定为必需，但在计算的时间段内尚无可用地点。</span><span class="sxs-lookup"><span data-stu-id="682cf-114">The **isRequired** property of the [locationConstraint](locationconstraint.md) parameter is specified as mandatory, and yet there are no locations available at the calculated time slots.</span></span> |
| <span data-ttu-id="682cf-115">organizerUnavailable</span><span class="sxs-lookup"><span data-stu-id="682cf-115">organizerUnavailable</span></span> | <span data-ttu-id="682cf-116">**isOrganizerOptional** 参数为 false，但组织者在请求的时间范围内不空闲。</span><span class="sxs-lookup"><span data-stu-id="682cf-116">The **isOrganizerOptional** parameter is false and yet the organizer is not available during the requested time window.</span></span> |
| <span data-ttu-id="682cf-117">unknown</span><span class="sxs-lookup"><span data-stu-id="682cf-117">unknown</span></span> | <span data-ttu-id="682cf-118">未返回任何会议时间建议的原因未知。</span><span class="sxs-lookup"><span data-stu-id="682cf-118">The reason for not returning any meeting suggestions is not known.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="682cf-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="682cf-119">JSON representation</span></span>

<span data-ttu-id="682cf-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="682cf-120">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="682cf-121">属性</span><span class="sxs-lookup"><span data-stu-id="682cf-121">Properties</span></span>
| <span data-ttu-id="682cf-122">属性</span><span class="sxs-lookup"><span data-stu-id="682cf-122">Property</span></span>     | <span data-ttu-id="682cf-123">类型</span><span class="sxs-lookup"><span data-stu-id="682cf-123">Type</span></span>   |<span data-ttu-id="682cf-124">说明</span><span class="sxs-lookup"><span data-stu-id="682cf-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="682cf-125">emptySuggestionsReason</span><span class="sxs-lookup"><span data-stu-id="682cf-125">emptySuggestionsReason</span></span>|<span data-ttu-id="682cf-126">String</span><span class="sxs-lookup"><span data-stu-id="682cf-126">String</span></span>|<span data-ttu-id="682cf-p102">未返回任何会议时间建议的原因。可取值为：`attendeesUnavailable`、`attendeesUnavailableOrUnknown`、`locationsUnavailable`、`organizerUnavailable` 或 `unknown`。如果 **meetingTimeSuggestions** 属性未包含任何会议建议，则此属性为空字符串。</span><span class="sxs-lookup"><span data-stu-id="682cf-p102">A reason for not returning any meeting suggestions. Possible values are: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable`, or `unknown`. This property is an empty string if the **meetingTimeSuggestions** property does include any meeting suggestions.</span></span>|
|<span data-ttu-id="682cf-130">meetingTimeSuggestions</span><span class="sxs-lookup"><span data-stu-id="682cf-130">meetingTimeSuggestions</span></span>|<span data-ttu-id="682cf-131">[meetingTimeSuggestion](meetingtimesuggestion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="682cf-131">[meetingTimeSuggestion](meetingtimesuggestion.md) collection</span></span>|<span data-ttu-id="682cf-132">一组会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="682cf-132">An array of meeting suggestions.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimesuggestionsresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
