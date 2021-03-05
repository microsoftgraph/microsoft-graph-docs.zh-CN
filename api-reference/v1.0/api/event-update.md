---
title: 更新事件
description: 更新 event 对象的属性。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4c9db9213b6245cc3a0c07c0bb590f0543055cb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448261"
---
# <a name="update-event"></a><span data-ttu-id="97062-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="97062-103">Update event</span></span>

<span data-ttu-id="97062-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97062-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97062-105">更新 [event](../resources/event.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97062-105">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="97062-106">更新事件开始或结束时间的时区时，首先[找到支持的时区](outlookuser-supportedtimezones.md)，以确保仅设置针对用户的邮箱服务器配置的时区。</span><span class="sxs-lookup"><span data-stu-id="97062-106">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="97062-107">权限</span><span class="sxs-lookup"><span data-stu-id="97062-107">Permissions</span></span>
<span data-ttu-id="97062-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97062-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97062-110">Permission type</span></span>      | <span data-ttu-id="97062-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97062-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97062-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97062-112">Delegated (work or school account)</span></span> | <span data-ttu-id="97062-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97062-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="97062-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97062-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97062-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97062-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="97062-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="97062-116">Application</span></span> | <span data-ttu-id="97062-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97062-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97062-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97062-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="97062-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="97062-119">Request headers</span></span>
| <span data-ttu-id="97062-120">名称</span><span class="sxs-lookup"><span data-stu-id="97062-120">Name</span></span>       | <span data-ttu-id="97062-121">类型</span><span class="sxs-lookup"><span data-stu-id="97062-121">Type</span></span> | <span data-ttu-id="97062-122">说明</span><span class="sxs-lookup"><span data-stu-id="97062-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97062-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97062-123">Authorization</span></span>  | <span data-ttu-id="97062-124">string</span><span class="sxs-lookup"><span data-stu-id="97062-124">string</span></span>  | <span data-ttu-id="97062-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97062-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97062-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="97062-127">Request body</span></span>
<span data-ttu-id="97062-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="97062-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97062-131">属性</span><span class="sxs-lookup"><span data-stu-id="97062-131">Property</span></span>     | <span data-ttu-id="97062-132">类型</span><span class="sxs-lookup"><span data-stu-id="97062-132">Type</span></span>   |<span data-ttu-id="97062-133">说明</span><span class="sxs-lookup"><span data-stu-id="97062-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97062-134">attendees</span><span class="sxs-lookup"><span data-stu-id="97062-134">attendees</span></span>|[<span data-ttu-id="97062-135">与会者</span><span class="sxs-lookup"><span data-stu-id="97062-135">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="97062-136">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="97062-136">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="97062-137">body</span><span class="sxs-lookup"><span data-stu-id="97062-137">body</span></span>|[<span data-ttu-id="97062-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="97062-138">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="97062-139">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="97062-139">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="97062-140">categories</span><span class="sxs-lookup"><span data-stu-id="97062-140">categories</span></span>|<span data-ttu-id="97062-141">String collection</span><span class="sxs-lookup"><span data-stu-id="97062-141">String collection</span></span>|<span data-ttu-id="97062-142">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="97062-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="97062-143">end</span><span class="sxs-lookup"><span data-stu-id="97062-143">end</span></span>|<span data-ttu-id="97062-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="97062-144">DateTimeTimeZone</span></span>|<span data-ttu-id="97062-145">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="97062-145">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="97062-146">hideAttendees</span><span class="sxs-lookup"><span data-stu-id="97062-146">hideAttendees</span></span>|<span data-ttu-id="97062-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="97062-147">Boolean</span></span>|<span data-ttu-id="97062-148">如果设置为 `true`，则每个与会者仅会在会议请求和会议 **跟踪** 列表中看到自己。</span><span class="sxs-lookup"><span data-stu-id="97062-148">When set to `true`, each attendee only sees themselves in the meeting request and meeting **Tracking** list.</span></span> <span data-ttu-id="97062-149">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="97062-149">Default is false.</span></span>|
|<span data-ttu-id="97062-150">importance</span><span class="sxs-lookup"><span data-stu-id="97062-150">importance</span></span>|<span data-ttu-id="97062-151">String</span><span class="sxs-lookup"><span data-stu-id="97062-151">String</span></span>|<span data-ttu-id="97062-152">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="97062-152">The importance of the event.</span></span> <span data-ttu-id="97062-153">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="97062-153">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="97062-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="97062-154">isAllDay</span></span>|<span data-ttu-id="97062-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="97062-155">Boolean</span></span>|<span data-ttu-id="97062-156">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="97062-156">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="97062-157">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="97062-157">isOnlineMeeting</span></span>|<span data-ttu-id="97062-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="97062-158">Boolean</span></span>| <span data-ttu-id="97062-159">若此事件包含联机会议信息则为 `True`，反之则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="97062-159">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="97062-160">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="97062-160">Default is false.</span></span> <span data-ttu-id="97062-161">可选。</span><span class="sxs-lookup"><span data-stu-id="97062-161">Optional.</span></span>|
|<span data-ttu-id="97062-162">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="97062-162">isReminderOn</span></span>|<span data-ttu-id="97062-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="97062-163">Boolean</span></span>|<span data-ttu-id="97062-164">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="97062-164">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="97062-165">位置</span><span class="sxs-lookup"><span data-stu-id="97062-165">location</span></span>|[<span data-ttu-id="97062-166">位置</span><span class="sxs-lookup"><span data-stu-id="97062-166">Location</span></span>](../resources/location.md)|<span data-ttu-id="97062-167">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="97062-167">The location of the event.</span></span>|
|<span data-ttu-id="97062-168">locations</span><span class="sxs-lookup"><span data-stu-id="97062-168">locations</span></span>|<span data-ttu-id="97062-169">[location](../resources/location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97062-169">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="97062-170">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="97062-170">The locations where the event is held or attended from.</span></span> <span data-ttu-id="97062-171">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="97062-171">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="97062-172">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="97062-172">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="97062-173">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="97062-173">onlineMeetingProvider</span></span>|<span data-ttu-id="97062-174">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="97062-174">onlineMeetingProviderType</span></span>| <span data-ttu-id="97062-175">表示联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="97062-175">Represents the online meeting service provider.</span></span> <span data-ttu-id="97062-176">可取值为：`teamsForBusiness`、`skypeForBusiness` 和 `skypeForConsumer`。</span><span class="sxs-lookup"><span data-stu-id="97062-176">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="97062-177">可选。</span><span class="sxs-lookup"><span data-stu-id="97062-177">Optional.</span></span> |
|<span data-ttu-id="97062-178">recurrence</span><span class="sxs-lookup"><span data-stu-id="97062-178">recurrence</span></span>|[<span data-ttu-id="97062-179">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="97062-179">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="97062-180">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="97062-180">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="97062-181">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="97062-181">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="97062-182">Int32</span><span class="sxs-lookup"><span data-stu-id="97062-182">Int32</span></span>|<span data-ttu-id="97062-183">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="97062-183">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="97062-184">responseRequested</span><span class="sxs-lookup"><span data-stu-id="97062-184">responseRequested</span></span>|<span data-ttu-id="97062-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="97062-185">Boolean</span></span>|<span data-ttu-id="97062-186">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="97062-186">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="97062-187">sensitivity</span><span class="sxs-lookup"><span data-stu-id="97062-187">sensitivity</span></span>|<span data-ttu-id="97062-188">String</span><span class="sxs-lookup"><span data-stu-id="97062-188">String</span></span>| <span data-ttu-id="97062-189">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="97062-189">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="97062-190">showAs</span><span class="sxs-lookup"><span data-stu-id="97062-190">showAs</span></span>|<span data-ttu-id="97062-191">String</span><span class="sxs-lookup"><span data-stu-id="97062-191">String</span></span>|<span data-ttu-id="97062-192">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="97062-192">The status to show.</span></span> <span data-ttu-id="97062-193">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="97062-193">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="97062-194">start</span><span class="sxs-lookup"><span data-stu-id="97062-194">start</span></span>|<span data-ttu-id="97062-195">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="97062-195">DateTimeTimeZone</span></span>|<span data-ttu-id="97062-196">事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="97062-196">The start date, time, and time zone of the event.</span></span> |
|<span data-ttu-id="97062-197">subject</span><span class="sxs-lookup"><span data-stu-id="97062-197">subject</span></span>|<span data-ttu-id="97062-198">String</span><span class="sxs-lookup"><span data-stu-id="97062-198">String</span></span>|<span data-ttu-id="97062-199">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="97062-199">The text of the event's subject line.</span></span>|

<span data-ttu-id="97062-200">由于 **事件** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有 **事件** 实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="97062-200">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="97062-201">如果你正更新的 **事件** 是定期系列的主事件，包含多个与会者，并且具有已单独更新的实例，则将发送多个通知电子邮件：一个用于主系列，另一个用于已更新的实例。</span><span class="sxs-lookup"><span data-stu-id="97062-201">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="97062-202">响应</span><span class="sxs-lookup"><span data-stu-id="97062-202">Response</span></span>

<span data-ttu-id="97062-203">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97062-203">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="97062-204">**注意：** 此方法可以返回 HTTP 400 错误请求响应，错误代码为 `ErrorOccurrenceCrossingBoundary`，并显示以下错误消息：已修改的事件正在交叉或重叠相邻的事件。</span><span class="sxs-lookup"><span data-stu-id="97062-204">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="97062-205">这表示更新违反了重复例外的以下 Outlook 限制：事件无法移动到上一次发生的日期或之前，并且无法移动到下一次发生的日期或之后。 </span><span class="sxs-lookup"><span data-stu-id="97062-205">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="97062-206">示例</span><span class="sxs-lookup"><span data-stu-id="97062-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="97062-207">请求</span><span class="sxs-lookup"><span data-stu-id="97062-207">Request</span></span>

<span data-ttu-id="97062-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97062-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97062-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="97062-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="97062-210">C#</span><span class="sxs-lookup"><span data-stu-id="97062-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97062-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97062-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97062-212">Java</span><span class="sxs-lookup"><span data-stu-id="97062-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="97062-213">响应</span><span class="sxs-lookup"><span data-stu-id="97062-213">Response</span></span>

<span data-ttu-id="97062-214">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97062-214">Here is an example of the response.</span></span> <span data-ttu-id="97062-215">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="97062-215">Note: The response object shown here may be truncated for brevity.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="97062-216">另请参阅</span><span class="sxs-lookup"><span data-stu-id="97062-216">See also</span></span>

- [<span data-ttu-id="97062-217">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97062-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="97062-218">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97062-218">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="97062-219">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97062-219">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



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

