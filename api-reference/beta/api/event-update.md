---
title: 更新事件
description: 更新 event 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 847bb4f25cfdadecc3983ac7365eff8146200094
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268388"
---
# <a name="update-event"></a><span data-ttu-id="23050-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="23050-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23050-104">更新 [event](../resources/event.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23050-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="23050-105">更新事件开始或结束时间的时区时，首先[找到支持的时区](outlookuser-supportedtimezones.md)，以确保仅设置针对用户的邮箱服务器配置的时区。</span><span class="sxs-lookup"><span data-stu-id="23050-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="23050-106">权限</span><span class="sxs-lookup"><span data-stu-id="23050-106">Permissions</span></span>
<span data-ttu-id="23050-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23050-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="23050-109">Permission type</span></span>      | <span data-ttu-id="23050-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23050-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23050-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23050-111">Delegated (work or school account)</span></span> | <span data-ttu-id="23050-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23050-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="23050-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23050-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23050-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23050-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="23050-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="23050-115">Application</span></span> | <span data-ttu-id="23050-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23050-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23050-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23050-117">HTTP request</span></span>
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

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="23050-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="23050-118">Request headers</span></span>
| <span data-ttu-id="23050-119">名称</span><span class="sxs-lookup"><span data-stu-id="23050-119">Name</span></span>       | <span data-ttu-id="23050-120">类型</span><span class="sxs-lookup"><span data-stu-id="23050-120">Type</span></span> | <span data-ttu-id="23050-121">说明</span><span class="sxs-lookup"><span data-stu-id="23050-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23050-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23050-122">Authorization</span></span>  | <span data-ttu-id="23050-123">string</span><span class="sxs-lookup"><span data-stu-id="23050-123">string</span></span>  | <span data-ttu-id="23050-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23050-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23050-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="23050-126">Request body</span></span>
<span data-ttu-id="23050-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="23050-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="23050-130">属性</span><span class="sxs-lookup"><span data-stu-id="23050-130">Property</span></span>       | <span data-ttu-id="23050-131">类型</span><span class="sxs-lookup"><span data-stu-id="23050-131">Type</span></span>    | <span data-ttu-id="23050-132">说明</span><span class="sxs-lookup"><span data-stu-id="23050-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="23050-133">attendees</span><span class="sxs-lookup"><span data-stu-id="23050-133">attendees</span></span>|<span data-ttu-id="23050-134">与会者</span><span class="sxs-lookup"><span data-stu-id="23050-134">Attendee</span></span>|<span data-ttu-id="23050-135">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="23050-135">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="23050-136">body</span><span class="sxs-lookup"><span data-stu-id="23050-136">body</span></span>|<span data-ttu-id="23050-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="23050-137">ItemBody</span></span>|<span data-ttu-id="23050-138">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="23050-138">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="23050-139">categories</span><span class="sxs-lookup"><span data-stu-id="23050-139">categories</span></span>|<span data-ttu-id="23050-140">String</span><span class="sxs-lookup"><span data-stu-id="23050-140">String</span></span>|<span data-ttu-id="23050-141">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="23050-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="23050-142">end</span><span class="sxs-lookup"><span data-stu-id="23050-142">end</span></span>|<span data-ttu-id="23050-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23050-143">DateTimeTimeZone</span></span>|<span data-ttu-id="23050-144">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="23050-144">The date, time, and time zone that the event ends.</span></span> |
| <span data-ttu-id="23050-145">importance</span><span class="sxs-lookup"><span data-stu-id="23050-145">importance</span></span>|<span data-ttu-id="23050-146">String</span><span class="sxs-lookup"><span data-stu-id="23050-146">String</span></span>|<span data-ttu-id="23050-147">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="23050-147">The importance of the event.</span></span> <span data-ttu-id="23050-148">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="23050-148">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="23050-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="23050-149">isAllDay</span></span>|<span data-ttu-id="23050-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="23050-150">Boolean</span></span>|<span data-ttu-id="23050-151">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="23050-151">Set to true if the event lasts all day.</span></span> <span data-ttu-id="23050-152">如果为 true，无论它是一天还是多天事件，开始和结束时间都必须设置为午夜，并且必须在相同的时区内。</span><span class="sxs-lookup"><span data-stu-id="23050-152">If true, regardless of whether it's a single-day or multi-day event, start and end time must be set to midnight and be in the same time zone.</span></span>|
|<span data-ttu-id="23050-153">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="23050-153">isOnlineMeeting</span></span>|<span data-ttu-id="23050-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="23050-154">Boolean</span></span>| <span data-ttu-id="23050-155">若此事件包含联机会议信息则为 `True`，反之则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="23050-155">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="23050-156">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="23050-156">Default is false.</span></span> <span data-ttu-id="23050-157">可选。</span><span class="sxs-lookup"><span data-stu-id="23050-157">Optional.</span></span>|
| <span data-ttu-id="23050-158">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="23050-158">isReminderOn</span></span>|<span data-ttu-id="23050-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="23050-159">Boolean</span></span>|<span data-ttu-id="23050-160">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="23050-160">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="23050-161">位置</span><span class="sxs-lookup"><span data-stu-id="23050-161">location</span></span>|<span data-ttu-id="23050-162">位置</span><span class="sxs-lookup"><span data-stu-id="23050-162">Location</span></span>|<span data-ttu-id="23050-163">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="23050-163">The location of the event.</span></span>|
|<span data-ttu-id="23050-164">位置</span><span class="sxs-lookup"><span data-stu-id="23050-164">locations</span></span>|<span data-ttu-id="23050-165">[location](../resources/location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23050-165">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="23050-166">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="23050-166">The locations where the event is held or attended from.</span></span> <span data-ttu-id="23050-167">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="23050-167">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="23050-168">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="23050-168">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="23050-169">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="23050-169">onlineMeetingProvider</span></span>|<span data-ttu-id="23050-170">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="23050-170">onlineMeetingProviderType</span></span>| <span data-ttu-id="23050-171">表示联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="23050-171">Represents the online meeting service provider.</span></span> <span data-ttu-id="23050-172">可取值为：`teamsForBusiness`、`skypeForBusiness` 和 `skypeForConsumer`。</span><span class="sxs-lookup"><span data-stu-id="23050-172">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="23050-173">可选。</span><span class="sxs-lookup"><span data-stu-id="23050-173">Optional.</span></span> |
| <span data-ttu-id="23050-174">recurrence</span><span class="sxs-lookup"><span data-stu-id="23050-174">recurrence</span></span>|<span data-ttu-id="23050-175">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="23050-175">PatternedRecurrence</span></span>|<span data-ttu-id="23050-176">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="23050-176">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="23050-177">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="23050-177">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="23050-178">Int32</span><span class="sxs-lookup"><span data-stu-id="23050-178">Int32</span></span>|<span data-ttu-id="23050-179">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="23050-179">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="23050-180">responseRequested</span><span class="sxs-lookup"><span data-stu-id="23050-180">responseRequested</span></span>|<span data-ttu-id="23050-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="23050-181">Boolean</span></span>|<span data-ttu-id="23050-182">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="23050-182">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="23050-183">sensitivity</span><span class="sxs-lookup"><span data-stu-id="23050-183">sensitivity</span></span>|<span data-ttu-id="23050-184">String</span><span class="sxs-lookup"><span data-stu-id="23050-184">String</span></span>| <span data-ttu-id="23050-185">可能的值是：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="23050-185">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="23050-186">showAs</span><span class="sxs-lookup"><span data-stu-id="23050-186">showAs</span></span>|<span data-ttu-id="23050-187">String</span><span class="sxs-lookup"><span data-stu-id="23050-187">String</span></span>|<span data-ttu-id="23050-188">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="23050-188">The status to show.</span></span> <span data-ttu-id="23050-189">可能的值为`free` ： `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`、。</span><span class="sxs-lookup"><span data-stu-id="23050-189">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="23050-190">start</span><span class="sxs-lookup"><span data-stu-id="23050-190">start</span></span>|<span data-ttu-id="23050-191">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="23050-191">DateTimeTimeZone</span></span>|<span data-ttu-id="23050-192">事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="23050-192">The start date, time, and time zone of the event.</span></span> |
| <span data-ttu-id="23050-193">subject</span><span class="sxs-lookup"><span data-stu-id="23050-193">subject</span></span>|<span data-ttu-id="23050-194">String</span><span class="sxs-lookup"><span data-stu-id="23050-194">String</span></span>|<span data-ttu-id="23050-195">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="23050-195">The text of the event's subject line.</span></span>|

<span data-ttu-id="23050-196">由于**事件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**事件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="23050-196">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="23050-197">如果你正更新的**事件**是定期系列的主事件，包含多个与会者，并且具有已单独更新的实例，则将发送多个通知电子邮件：一个用于主系列，另一个用于已更新的实例。</span><span class="sxs-lookup"><span data-stu-id="23050-197">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="23050-198">响应</span><span class="sxs-lookup"><span data-stu-id="23050-198">Response</span></span>

<span data-ttu-id="23050-199">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23050-199">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="23050-200">**注意：** 此方法可以返回 HTTP 400 错误请求响应，错误代码为 `ErrorOccurrenceCrossingBoundary`，并显示以下错误消息：已修改的事件正在交叉或重叠相邻的事件。</span><span class="sxs-lookup"><span data-stu-id="23050-200">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="23050-201">这表示更新违反了重复例外的以下 Outlook 限制：事件无法移动到上一次发生的日期或之前，并且无法移动到下一次发生的日期或之后。 </span><span class="sxs-lookup"><span data-stu-id="23050-201">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="23050-202">示例</span><span class="sxs-lookup"><span data-stu-id="23050-202">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23050-203">请求</span><span class="sxs-lookup"><span data-stu-id="23050-203">Request</span></span>

<span data-ttu-id="23050-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23050-204">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23050-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="23050-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true
}
```
# <a name="c"></a>[<span data-ttu-id="23050-206">C#</span><span class="sxs-lookup"><span data-stu-id="23050-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23050-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23050-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23050-208">响应</span><span class="sxs-lookup"><span data-stu-id="23050-208">Response</span></span>
<span data-ttu-id="23050-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23050-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
    }
}
```


## <a name="see-also"></a><span data-ttu-id="23050-212">另请参阅</span><span class="sxs-lookup"><span data-stu-id="23050-212">See also</span></span>

- [<span data-ttu-id="23050-213">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="23050-213">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="23050-214">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="23050-214">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="23050-215">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="23050-215">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
