---
title: 'user: findMeetingTimes'
description: 建议的会议时间内和基于组织者和与会者可用性和作为参数指定的时间或位置约束位置。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1e2ced373cffec19ab0d945dbc27e24833e8059
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923164"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="f2708-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="f2708-103">user: findMeetingTimes</span></span>
<span data-ttu-id="f2708-104">建议的会议时间内和基于组织者和与会者可用性和作为参数指定的时间或位置约束位置。</span><span class="sxs-lookup"><span data-stu-id="f2708-104">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="f2708-p101">如果 **findMeetingTimes** 无法返回任何会议时间建议，响应会在 **emptySuggestionsReason** 属性中指明原因。根据此值，可以更好地调整参数，并重新调用 **findMeetingTimes**。</span><span class="sxs-lookup"><span data-stu-id="f2708-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>


## <a name="permissions"></a><span data-ttu-id="f2708-107">权限</span><span class="sxs-lookup"><span data-stu-id="f2708-107">Permissions</span></span>
<span data-ttu-id="f2708-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2708-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2708-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2708-110">Permission type</span></span>      | <span data-ttu-id="f2708-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2708-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2708-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2708-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2708-113">Calendars.Read.Shared、Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="f2708-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="f2708-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2708-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2708-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2708-115">Not supported.</span></span>    |
|<span data-ttu-id="f2708-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2708-116">Application</span></span> | <span data-ttu-id="f2708-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2708-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2708-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2708-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="f2708-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2708-119">Request headers</span></span>
| <span data-ttu-id="f2708-120">名称</span><span class="sxs-lookup"><span data-stu-id="f2708-120">Name</span></span>       | <span data-ttu-id="f2708-121">值</span><span class="sxs-lookup"><span data-stu-id="f2708-121">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f2708-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2708-122">Authorization</span></span>  | <span data-ttu-id="f2708-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2708-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2708-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f2708-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f2708-p104">表示响应的具体时区的字符串，例如，“Pacific Standard Time”。可选。如果未指定此标头则使用 UTC。</span><span class="sxs-lookup"><span data-stu-id="f2708-p104">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2708-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2708-129">Request body</span></span>
<span data-ttu-id="f2708-p105">下面列出了支持的所有参数。根据你自己的方案，在请求正文中为各个必需参数指定 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f2708-p105">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="f2708-132">参数</span><span class="sxs-lookup"><span data-stu-id="f2708-132">Parameter</span></span>    | <span data-ttu-id="f2708-133">类型</span><span class="sxs-lookup"><span data-stu-id="f2708-133">Type</span></span>   |<span data-ttu-id="f2708-134">说明</span><span class="sxs-lookup"><span data-stu-id="f2708-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2708-135">attendees</span><span class="sxs-lookup"><span data-stu-id="f2708-135">attendees</span></span>|<span data-ttu-id="f2708-136">[attendeeBase](../resources/attendeebase.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2708-136">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="f2708-p106">一组会议与会者或资源。由于 findMeetingTimes 假设始终需要具备与会人员，因此在对应的 **type** 属性中将人员指定为 `required` 而将资源指定为 `resource`。如果集合为空，则 **findMeetingTimes** 只会查找组织者的空闲时间段。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p106">A collection of attendees or resources for the meeting. Since findMeetingTimes assumes that any attendee who is a person is always required, specify `required` for a person and `resource` for a resource in the corresponding **type** property. An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer. Optional.</span></span>|
|<span data-ttu-id="f2708-141">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="f2708-141">isOrganizerOptional</span></span>|<span data-ttu-id="f2708-142">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f2708-142">Edm.Boolean</span></span>|<span data-ttu-id="f2708-p107">如果组织者不必必须参加，则指定 `True`。默认值为 `false`。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p107">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="f2708-146">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f2708-146">locationConstraint</span></span>|[<span data-ttu-id="f2708-147">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f2708-147">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="f2708-p108">组织者对会议地点的要求，如是否必须返回会议地点建议，或是否只能在特定地点举行会议。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p108">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="f2708-150">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="f2708-150">maxCandidates</span></span>|<span data-ttu-id="f2708-151">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f2708-151">Edm.Int32</span></span>|<span data-ttu-id="f2708-p109">要返回的会议时间建议数量上限。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p109">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="f2708-154">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="f2708-154">meetingDuration</span></span>|<span data-ttu-id="f2708-155">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="f2708-155">Edm.Duration</span></span>|<span data-ttu-id="f2708-p110">会议时长，以 [ISO8601](https://www.iso.org/iso/iso8601) 格式表示。例如，1 小时表示为“PT1H”，其中“P”是持续时间指示符，“T”是时间指示符，“H”是小时指示符。使用 M 指示时长的分钟数；例如，2 小时 30 分钟是“PT2H30M”。如果未指定会议持续时间，则 **findMeetingTimes** 使用默认值 30 分钟。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p110">The length of the meeting, denoted in [ISO8601](https://www.iso.org/iso/iso8601) format. For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator. Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'. If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes. Optional.</span></span>|
|<span data-ttu-id="f2708-161">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="f2708-161">minimumAttendeePercentage</span></span>|<span data-ttu-id="f2708-162">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="f2708-162">Edm.Double</span></span>| <span data-ttu-id="f2708-p111">在响应中返回时间段所需的最低 [confidence](#the-confidence-of-a-meeting-suggestion)。这是一个介于 0 到 100 之间的百分比值。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p111">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="f2708-166">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="f2708-166">returnSuggestionReasons</span></span>|<span data-ttu-id="f2708-167">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f2708-167">Edm.Boolean</span></span>|<span data-ttu-id="f2708-p112">指定 `True` 可以在 **suggestionReason** 属性中返回每个会议建议的理由。默认为 `false`，即不返回此属性。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p112">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="f2708-171">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f2708-171">timeConstraint</span></span>|[<span data-ttu-id="f2708-172">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f2708-172">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="f2708-p113">会议的所有时间限制，可以包括会议性质（**activityDomain** 属性）和可能的会议时间段（**timeSlots** 属性）。如果未指定此参数，则 **findMeetingTimes** 将 **activityDomain** 假定为 `work`。可选。</span><span class="sxs-lookup"><span data-stu-id="f2708-p113">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="f2708-176">下表描述了**activityDomain**限制可以进一步**timeConstraint**参数中指定。</span><span class="sxs-lookup"><span data-stu-id="f2708-176">The following table describes the **activityDomain** restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="f2708-177">activityDomain 值</span><span class="sxs-lookup"><span data-stu-id="f2708-177">activityDomain value</span></span>|<span data-ttu-id="f2708-178">会议时间建议</span><span class="sxs-lookup"><span data-stu-id="f2708-178">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="f2708-179">工时</span><span class="sxs-lookup"><span data-stu-id="f2708-179">work</span></span>| <span data-ttu-id="f2708-p114">建议处于用户的工作时间（在用户的日历配置中定义该时间，并且可由用户或管理员自定义）内。默认工作时间是星期一到星期五的上午八点到下午五点（使用为邮箱设置的时区）。如果未指定 **activityDomain** 则此为默认值。</span><span class="sxs-lookup"><span data-stu-id="f2708-p114">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="f2708-183">personal</span><span class="sxs-lookup"><span data-stu-id="f2708-183">personal</span></span>| <span data-ttu-id="f2708-p115">建议处于用户的工作时间内及星期六和星期日。默认是星期一到星期日的上午八点到下午五点（使用邮箱的时区设置）。</span><span class="sxs-lookup"><span data-stu-id="f2708-p115">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="f2708-186">unrestricted</span><span class="sxs-lookup"><span data-stu-id="f2708-186">unrestricted</span></span> | <span data-ttu-id="f2708-187">建议可以是全年任意一天的任意时间段。</span><span class="sxs-lookup"><span data-stu-id="f2708-187">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="f2708-188">unknown</span><span class="sxs-lookup"><span data-stu-id="f2708-188">unknown</span></span> | <span data-ttu-id="f2708-p116">请勿使用此值，因为以后会弃用此值。当前其行为与 `work` 相同。根据需要将任何现有代码更改为使用 `work`、`personal`、或 `unrestricted`。</span><span class="sxs-lookup"><span data-stu-id="f2708-p116">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>


<span data-ttu-id="f2708-p117">根据指定的参数，**findMeetingTimes** 会检查组织者和与会者的主日历中的忙/闲状态。此操作会计算出最可行的会议时间，并返回所有会议时间建议。</span><span class="sxs-lookup"><span data-stu-id="f2708-p117">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="f2708-194">响应</span><span class="sxs-lookup"><span data-stu-id="f2708-194">Response</span></span>

<span data-ttu-id="f2708-195">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md)。</span><span class="sxs-lookup"><span data-stu-id="f2708-195">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="f2708-p118">**meetingTimeSuggestionsResult** 包含一组会议时间建议和 **emptySuggestionsReason** 属性。每条建议都被定义为 [meetingTimeSuggestion](../resources/meetingtimesuggestion.md)，同时与会者出席置信度平均值为 50%，或为你在 **minimumAttendeePercentage** 参数中指定的特定百分比值。</span><span class="sxs-lookup"><span data-stu-id="f2708-p118">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="f2708-198">默认情况下，返回的每条会议时间建议的时区均为 UTC。</span><span class="sxs-lookup"><span data-stu-id="f2708-198">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="f2708-p119">如果 **findMeetingTimes** 无法返回任何会议时间建议，响应会在 **emptySuggestionsReason** 属性中指明原因。根据此值，可以更好地调整参数，并重新调用 **findMeetingTimes**。</span><span class="sxs-lookup"><span data-stu-id="f2708-p119">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="f2708-201">会议时间建议的置信度</span><span class="sxs-lookup"><span data-stu-id="f2708-201">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="f2708-202">**meetingTimeSuggestion** 的 **confidence** 属性值介于 0% 到 100% 之间，表示所有与会者出席会议的可能性（以每个人的忙/闲状态为依据）：</span><span class="sxs-lookup"><span data-stu-id="f2708-202">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="f2708-203">对于每个与会者，在指定的会议时间段内，空闲、未知和忙碌状态对应的与会者出席可能性分别为 100%、49% 和 0%。</span><span class="sxs-lookup"><span data-stu-id="f2708-203">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="f2708-204">会议时间建议的置信度是通过计算相应会议的所有指定与会者的出席可能性平均值而得出。</span><span class="sxs-lookup"><span data-stu-id="f2708-204">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="f2708-p120">可以使用 **findMeetingTimes** 的可选参数 **minimumAttendeePercentage**，指定仅返回置信度不低于特定值的会议时间建议。例如，如果只想返回所有与会者的出席可能性不低于 80% 的会议时间建议，可以将 **minimumAttendeePercentage** 指定为 80%。如果未指定 **minimumAttendeePercentage**，**findMeetingTimes** 假定值为 50%。</span><span class="sxs-lookup"><span data-stu-id="f2708-p120">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>
- <span data-ttu-id="f2708-p121">如果有多条会议时间建议，**findMeetingTimes** 操作首先会按计算得出的置信度值由高到低对建议进行排序。如果会议时间建议的置信度相同，此操作会按时间顺序对建议进行排序。</span><span class="sxs-lookup"><span data-stu-id="f2708-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>

<span data-ttu-id="f2708-210">例如，如果会议时间建议涉及 3 位与会者，他们的忙/闲状态如下：</span><span class="sxs-lookup"><span data-stu-id="f2708-210">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="f2708-211">**与会者**</span><span class="sxs-lookup"><span data-stu-id="f2708-211">**Attendee**</span></span>|<span data-ttu-id="f2708-212">**忙/闲状态**</span><span class="sxs-lookup"><span data-stu-id="f2708-212">**Free/busy status**</span></span>|<span data-ttu-id="f2708-213">**出席可能性 (%)**</span><span class="sxs-lookup"><span data-stu-id="f2708-213">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f2708-214">Dana</span><span class="sxs-lookup"><span data-stu-id="f2708-214">Dana</span></span> | <span data-ttu-id="f2708-215">空闲</span><span class="sxs-lookup"><span data-stu-id="f2708-215">Free</span></span> | <span data-ttu-id="f2708-216">100%</span><span class="sxs-lookup"><span data-stu-id="f2708-216">100%</span></span> |
|<span data-ttu-id="f2708-217">John</span><span class="sxs-lookup"><span data-stu-id="f2708-217">John</span></span> | <span data-ttu-id="f2708-218">未知</span><span class="sxs-lookup"><span data-stu-id="f2708-218">Unknown</span></span> | <span data-ttu-id="f2708-219">49%</span><span class="sxs-lookup"><span data-stu-id="f2708-219">49%</span></span> |
|<span data-ttu-id="f2708-220">Samantha</span><span class="sxs-lookup"><span data-stu-id="f2708-220">Samantha</span></span> | <span data-ttu-id="f2708-221">忙碌</span><span class="sxs-lookup"><span data-stu-id="f2708-221">Busy</span></span> | <span data-ttu-id="f2708-222">0%</span><span class="sxs-lookup"><span data-stu-id="f2708-222">0%</span></span> |

<span data-ttu-id="f2708-223">会议时间建议的置信度为与会者出席可能性的平均值，即 (100% + 49% + 0%)/3 = 49.66%。</span><span class="sxs-lookup"><span data-stu-id="f2708-223">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="f2708-224">如果你在 **findMeetingTimes** 操作中将 **minimumAttendeePercentage** 指定为 80%，此操作将不会在响应中建议此时间，这是因为 49.66% < 80%。</span><span class="sxs-lookup"><span data-stu-id="f2708-224">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="f2708-225">示例</span><span class="sxs-lookup"><span data-stu-id="f2708-225">Example</span></span>

<span data-ttu-id="f2708-226">以下示例展示了如何查找预定地点会议的时间，并请求获得各条建议的理由，具体是通过在请求正文中指定以下参数：</span><span class="sxs-lookup"><span data-stu-id="f2708-226">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="f2708-227">**attendees**</span><span class="sxs-lookup"><span data-stu-id="f2708-227">**attendees**</span></span>
- <span data-ttu-id="f2708-228">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="f2708-228">**locationConstraint**</span></span>
- <span data-ttu-id="f2708-229">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="f2708-229">**timeConstraint**</span></span>
- <span data-ttu-id="f2708-230">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="f2708-230">**meetingDuration**</span></span>
- <span data-ttu-id="f2708-231">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="f2708-231">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="f2708-232">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="f2708-232">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="f2708-233">设置 **returnSuggestionReasons** 参数后，**suggestionReason** 属性中还会返回各条建议的理由（如果 **findMeetingTimes** 返回建议的话）。</span><span class="sxs-lookup"><span data-stu-id="f2708-233">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="f2708-p122">请注意，请求指定的是 PST 时区时间，而响应返回的会议时间建议默认采用 UTC。可以使用 `Prefer: outlook.timezone` 请求头也为响应中的时间值指定 PST 时区。</span><span class="sxs-lookup"><span data-stu-id="f2708-p122">Notice that the request specifies time in the PST time zone, and the response returns meeting time suggestions in UTC, by default. You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="f2708-236">请求</span><span class="sxs-lookup"><span data-stu-id="f2708-236">Request</span></span>
<span data-ttu-id="f2708-237">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2708-237">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"unrestricted", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-17T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-19T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100.0
}
```

##### <a name="response"></a><span data-ttu-id="f2708-238">响应</span><span class="sxs-lookup"><span data-stu-id="f2708-238">Response</span></span>
<span data-ttu-id="f2708-p123">下面展示了示例响应。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2708-p123">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 976

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T18:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        },
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T22:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/user-findmeetingtimes.md:
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|"
  ],
  "tocPath": ""
}-->
