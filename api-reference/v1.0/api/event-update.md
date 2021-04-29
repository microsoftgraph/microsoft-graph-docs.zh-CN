---
title: 更新事件
description: 更新 event 对象的属性。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8ff929216fa15859744a686090c522d810d3a8c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054026"
---
# <a name="update-event"></a><span data-ttu-id="5e69d-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="5e69d-103">Update event</span></span>

<span data-ttu-id="5e69d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e69d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e69d-105">更新 [event](../resources/event.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e69d-105">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="5e69d-106">更新事件开始或结束时间的时区时，首先[找到支持的时区](outlookuser-supportedtimezones.md)，以确保仅设置针对用户的邮箱服务器配置的时区。</span><span class="sxs-lookup"><span data-stu-id="5e69d-106">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5e69d-107">权限</span><span class="sxs-lookup"><span data-stu-id="5e69d-107">Permissions</span></span>
<span data-ttu-id="5e69d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e69d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e69d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e69d-110">Permission type</span></span>      | <span data-ttu-id="5e69d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e69d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e69d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e69d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e69d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e69d-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5e69d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e69d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e69d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e69d-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5e69d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e69d-116">Application</span></span> | <span data-ttu-id="5e69d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e69d-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e69d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e69d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5e69d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e69d-119">Request headers</span></span>
| <span data-ttu-id="5e69d-120">名称</span><span class="sxs-lookup"><span data-stu-id="5e69d-120">Name</span></span>       | <span data-ttu-id="5e69d-121">类型</span><span class="sxs-lookup"><span data-stu-id="5e69d-121">Type</span></span> | <span data-ttu-id="5e69d-122">说明</span><span class="sxs-lookup"><span data-stu-id="5e69d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e69d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e69d-123">Authorization</span></span>  | <span data-ttu-id="5e69d-124">string</span><span class="sxs-lookup"><span data-stu-id="5e69d-124">string</span></span>  | <span data-ttu-id="5e69d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e69d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e69d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e69d-127">Request body</span></span>
<span data-ttu-id="5e69d-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5e69d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e69d-131">属性</span><span class="sxs-lookup"><span data-stu-id="5e69d-131">Property</span></span>     | <span data-ttu-id="5e69d-132">类型</span><span class="sxs-lookup"><span data-stu-id="5e69d-132">Type</span></span>   |<span data-ttu-id="5e69d-133">说明</span><span class="sxs-lookup"><span data-stu-id="5e69d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e69d-134">attendees</span><span class="sxs-lookup"><span data-stu-id="5e69d-134">attendees</span></span>|[<span data-ttu-id="5e69d-135">与会者</span><span class="sxs-lookup"><span data-stu-id="5e69d-135">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="5e69d-136">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="5e69d-136">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="5e69d-137">body</span><span class="sxs-lookup"><span data-stu-id="5e69d-137">body</span></span>|[<span data-ttu-id="5e69d-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="5e69d-138">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="5e69d-139">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="5e69d-139">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="5e69d-140">categories</span><span class="sxs-lookup"><span data-stu-id="5e69d-140">categories</span></span>|<span data-ttu-id="5e69d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5e69d-141">String collection</span></span>|<span data-ttu-id="5e69d-142">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="5e69d-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="5e69d-143">end</span><span class="sxs-lookup"><span data-stu-id="5e69d-143">end</span></span>|<span data-ttu-id="5e69d-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5e69d-144">DateTimeTimeZone</span></span>|<span data-ttu-id="5e69d-145">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="5e69d-145">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="5e69d-146">hideAttendees</span><span class="sxs-lookup"><span data-stu-id="5e69d-146">hideAttendees</span></span>|<span data-ttu-id="5e69d-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="5e69d-147">Boolean</span></span>|<span data-ttu-id="5e69d-148">如果设置为 `true`，则每个与会者仅会在会议请求和会议 **跟踪** 列表中看到自己。</span><span class="sxs-lookup"><span data-stu-id="5e69d-148">When set to `true`, each attendee only sees themselves in the meeting request and meeting **Tracking** list.</span></span> <span data-ttu-id="5e69d-149">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="5e69d-149">Default is false.</span></span>|
|<span data-ttu-id="5e69d-150">importance</span><span class="sxs-lookup"><span data-stu-id="5e69d-150">importance</span></span>|<span data-ttu-id="5e69d-151">String</span><span class="sxs-lookup"><span data-stu-id="5e69d-151">String</span></span>|<span data-ttu-id="5e69d-152">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="5e69d-152">The importance of the event.</span></span> <span data-ttu-id="5e69d-153">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="5e69d-153">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="5e69d-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="5e69d-154">isAllDay</span></span>|<span data-ttu-id="5e69d-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e69d-155">Boolean</span></span>|<span data-ttu-id="5e69d-156">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5e69d-156">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="5e69d-157">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5e69d-157">isOnlineMeeting</span></span>|<span data-ttu-id="5e69d-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e69d-158">Boolean</span></span>| <span data-ttu-id="5e69d-159">若此事件包含联机会议信息则为 `True`，反之则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="5e69d-159">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="5e69d-160">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="5e69d-160">Default is false.</span></span> <span data-ttu-id="5e69d-161">可选。</span><span class="sxs-lookup"><span data-stu-id="5e69d-161">Optional.</span></span>|
|<span data-ttu-id="5e69d-162">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="5e69d-162">isReminderOn</span></span>|<span data-ttu-id="5e69d-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e69d-163">Boolean</span></span>|<span data-ttu-id="5e69d-164">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5e69d-164">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="5e69d-165">位置</span><span class="sxs-lookup"><span data-stu-id="5e69d-165">location</span></span>|[<span data-ttu-id="5e69d-166">位置</span><span class="sxs-lookup"><span data-stu-id="5e69d-166">Location</span></span>](../resources/location.md)|<span data-ttu-id="5e69d-167">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="5e69d-167">The location of the event.</span></span>|
|<span data-ttu-id="5e69d-168">locations</span><span class="sxs-lookup"><span data-stu-id="5e69d-168">locations</span></span>|<span data-ttu-id="5e69d-169">[location](../resources/location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e69d-169">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="5e69d-170">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="5e69d-170">The locations where the event is held or attended from.</span></span> <span data-ttu-id="5e69d-171">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="5e69d-171">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="5e69d-172">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="5e69d-172">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="5e69d-173">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="5e69d-173">onlineMeetingProvider</span></span>|<span data-ttu-id="5e69d-174">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="5e69d-174">onlineMeetingProviderType</span></span>| <span data-ttu-id="5e69d-175">表示联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="5e69d-175">Represents the online meeting service provider.</span></span> <span data-ttu-id="5e69d-176">可取值为：`teamsForBusiness`、`skypeForBusiness` 和 `skypeForConsumer`。</span><span class="sxs-lookup"><span data-stu-id="5e69d-176">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="5e69d-177">可选。</span><span class="sxs-lookup"><span data-stu-id="5e69d-177">Optional.</span></span> |
|<span data-ttu-id="5e69d-178">recurrence</span><span class="sxs-lookup"><span data-stu-id="5e69d-178">recurrence</span></span>|[<span data-ttu-id="5e69d-179">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="5e69d-179">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="5e69d-180">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="5e69d-180">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="5e69d-181">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5e69d-181">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="5e69d-182">Int32</span><span class="sxs-lookup"><span data-stu-id="5e69d-182">Int32</span></span>|<span data-ttu-id="5e69d-183">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="5e69d-183">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="5e69d-184">responseRequested</span><span class="sxs-lookup"><span data-stu-id="5e69d-184">responseRequested</span></span>|<span data-ttu-id="5e69d-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e69d-185">Boolean</span></span>|<span data-ttu-id="5e69d-186">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5e69d-186">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="5e69d-187">sensitivity</span><span class="sxs-lookup"><span data-stu-id="5e69d-187">sensitivity</span></span>|<span data-ttu-id="5e69d-188">String</span><span class="sxs-lookup"><span data-stu-id="5e69d-188">String</span></span>| <span data-ttu-id="5e69d-189">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="5e69d-189">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="5e69d-190">showAs</span><span class="sxs-lookup"><span data-stu-id="5e69d-190">showAs</span></span>|<span data-ttu-id="5e69d-191">String</span><span class="sxs-lookup"><span data-stu-id="5e69d-191">String</span></span>|<span data-ttu-id="5e69d-192">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="5e69d-192">The status to show.</span></span> <span data-ttu-id="5e69d-193">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="5e69d-193">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="5e69d-194">start</span><span class="sxs-lookup"><span data-stu-id="5e69d-194">start</span></span>|<span data-ttu-id="5e69d-195">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5e69d-195">DateTimeTimeZone</span></span>|<span data-ttu-id="5e69d-196">事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="5e69d-196">The start date, time, and time zone of the event.</span></span> |
|<span data-ttu-id="5e69d-197">subject</span><span class="sxs-lookup"><span data-stu-id="5e69d-197">subject</span></span>|<span data-ttu-id="5e69d-198">String</span><span class="sxs-lookup"><span data-stu-id="5e69d-198">String</span></span>|<span data-ttu-id="5e69d-199">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="5e69d-199">The text of the event's subject line.</span></span>|

<span data-ttu-id="5e69d-200">由于 **事件** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有 **事件** 实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="5e69d-200">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="5e69d-201">如果你正更新的 **事件** 是定期系列的主事件，包含多个与会者，并且具有已单独更新的实例，则将发送多个通知电子邮件：一个用于主系列，另一个用于已更新的实例。</span><span class="sxs-lookup"><span data-stu-id="5e69d-201">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="5e69d-202">响应</span><span class="sxs-lookup"><span data-stu-id="5e69d-202">Response</span></span>

<span data-ttu-id="5e69d-203">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e69d-203">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="5e69d-204">**注意：** 此方法可以返回 HTTP 400 错误请求响应，错误代码为 `ErrorOccurrenceCrossingBoundary`，并显示以下错误消息：已修改的事件正在交叉或重叠相邻的事件。</span><span class="sxs-lookup"><span data-stu-id="5e69d-204">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="5e69d-205">这表示更新违反了重复例外的以下 Outlook 限制：事件无法移动到上一次发生的日期或之前，并且无法移动到下一次发生的日期或之后。 </span><span class="sxs-lookup"><span data-stu-id="5e69d-205">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="5e69d-206">示例</span><span class="sxs-lookup"><span data-stu-id="5e69d-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e69d-207">请求</span><span class="sxs-lookup"><span data-stu-id="5e69d-207">Request</span></span>

<span data-ttu-id="5e69d-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e69d-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e69d-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e69d-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "categories": ["Red category"]
}
```
# <a name="c"></a>[<span data-ttu-id="5e69d-210">C#</span><span class="sxs-lookup"><span data-stu-id="5e69d-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e69d-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e69d-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e69d-212">Java</span><span class="sxs-lookup"><span data-stu-id="5e69d-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e69d-213">响应</span><span class="sxs-lookup"><span data-stu-id="5e69d-213">Response</span></span>

<span data-ttu-id="5e69d-214">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e69d-214">Here is an example of the response.</span></span> <span data-ttu-id="5e69d-215">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5e69d-215">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="5e69d-216">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5e69d-216">See also</span></span>

- [<span data-ttu-id="5e69d-217">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5e69d-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5e69d-218">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5e69d-218">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5e69d-219">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5e69d-219">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

