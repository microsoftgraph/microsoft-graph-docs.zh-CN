---
title: 更新事件
description: 更新 event 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 09ebb87d33a7fe3d32281e6b83fde3bd7b3efefc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883060"
---
# <a name="update-event"></a><span data-ttu-id="094b3-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="094b3-103">Update event</span></span>

> <span data-ttu-id="094b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="094b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="094b3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="094b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="094b3-106">更新[event](../resources/event.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="094b3-106">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="094b3-107">权限</span><span class="sxs-lookup"><span data-stu-id="094b3-107">Permissions</span></span>
<span data-ttu-id="094b3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="094b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="094b3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="094b3-110">Permission type</span></span>      | <span data-ttu-id="094b3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="094b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="094b3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="094b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="094b3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="094b3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="094b3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="094b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="094b3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="094b3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="094b3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="094b3-116">Application</span></span> | <span data-ttu-id="094b3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="094b3-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="094b3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="094b3-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="094b3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="094b3-119">Request headers</span></span>
| <span data-ttu-id="094b3-120">名称</span><span class="sxs-lookup"><span data-stu-id="094b3-120">Name</span></span>       | <span data-ttu-id="094b3-121">类型</span><span class="sxs-lookup"><span data-stu-id="094b3-121">Type</span></span> | <span data-ttu-id="094b3-122">说明</span><span class="sxs-lookup"><span data-stu-id="094b3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="094b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="094b3-123">Authorization</span></span>  | <span data-ttu-id="094b3-124">string</span><span class="sxs-lookup"><span data-stu-id="094b3-124">string</span></span>  | <span data-ttu-id="094b3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="094b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="094b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="094b3-127">Request body</span></span>
<span data-ttu-id="094b3-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="094b3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="094b3-131">属性</span><span class="sxs-lookup"><span data-stu-id="094b3-131">Property</span></span>       | <span data-ttu-id="094b3-132">类型</span><span class="sxs-lookup"><span data-stu-id="094b3-132">Type</span></span>    | <span data-ttu-id="094b3-133">说明</span><span class="sxs-lookup"><span data-stu-id="094b3-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="094b3-134">attendees</span><span class="sxs-lookup"><span data-stu-id="094b3-134">attendees</span></span>|<span data-ttu-id="094b3-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="094b3-135">Attendee</span></span>|<span data-ttu-id="094b3-136">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="094b3-136">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="094b3-137">body</span><span class="sxs-lookup"><span data-stu-id="094b3-137">body</span></span>|<span data-ttu-id="094b3-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="094b3-138">ItemBody</span></span>|<span data-ttu-id="094b3-139">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="094b3-139">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="094b3-140">categories</span><span class="sxs-lookup"><span data-stu-id="094b3-140">categories</span></span>|<span data-ttu-id="094b3-141">String</span><span class="sxs-lookup"><span data-stu-id="094b3-141">String</span></span>|<span data-ttu-id="094b3-142">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="094b3-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="094b3-143">end</span><span class="sxs-lookup"><span data-stu-id="094b3-143">end</span></span>|<span data-ttu-id="094b3-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="094b3-144">DateTimeTimeZone</span></span>|<span data-ttu-id="094b3-145">事件的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="094b3-145">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="094b3-p105">默认情况下，结束时间使用 UTC 格式。可以在 EndTimeZone 中指定可选的时区，用该时区表示结束时间并包括与 UTC 的时间偏移量。请注意，如果使用 EndTimeZone，必须为 StartTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="094b3-p105">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="094b3-149">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 9:34：“2015-02-25T21:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="094b3-149">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="094b3-150">importance</span><span class="sxs-lookup"><span data-stu-id="094b3-150">importance</span></span>|<span data-ttu-id="094b3-151">String</span><span class="sxs-lookup"><span data-stu-id="094b3-151">String</span></span>|<span data-ttu-id="094b3-152">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="094b3-152">The importance of the event.</span></span> <span data-ttu-id="094b3-153">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="094b3-153">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="094b3-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="094b3-154">isAllDay</span></span>|<span data-ttu-id="094b3-155">布尔</span><span class="sxs-lookup"><span data-stu-id="094b3-155">Boolean</span></span>|<span data-ttu-id="094b3-156">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="094b3-156">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="094b3-157">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="094b3-157">isReminderOn</span></span>|<span data-ttu-id="094b3-158">布尔</span><span class="sxs-lookup"><span data-stu-id="094b3-158">Boolean</span></span>|<span data-ttu-id="094b3-159">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="094b3-159">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="094b3-160">location</span><span class="sxs-lookup"><span data-stu-id="094b3-160">location</span></span>|<span data-ttu-id="094b3-161">Location</span><span class="sxs-lookup"><span data-stu-id="094b3-161">Location</span></span>|<span data-ttu-id="094b3-162">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="094b3-162">The location of the event.</span></span>|
|<span data-ttu-id="094b3-163">locations</span><span class="sxs-lookup"><span data-stu-id="094b3-163">locations</span></span>|<span data-ttu-id="094b3-164">[位置](../resources/location.md)集合</span><span class="sxs-lookup"><span data-stu-id="094b3-164">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="094b3-165">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="094b3-165">The locations where the event is held or attended from.</span></span> <span data-ttu-id="094b3-166">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="094b3-166">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="094b3-167">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="094b3-167">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="094b3-168">recurrence</span><span class="sxs-lookup"><span data-stu-id="094b3-168">recurrence</span></span>|<span data-ttu-id="094b3-169">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="094b3-169">PatternedRecurrence</span></span>|<span data-ttu-id="094b3-170">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="094b3-170">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="094b3-171">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="094b3-171">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="094b3-172">Int32</span><span class="sxs-lookup"><span data-stu-id="094b3-172">Int32</span></span>|<span data-ttu-id="094b3-173">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="094b3-173">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="094b3-174">responseRequested</span><span class="sxs-lookup"><span data-stu-id="094b3-174">responseRequested</span></span>|<span data-ttu-id="094b3-175">布尔</span><span class="sxs-lookup"><span data-stu-id="094b3-175">Boolean</span></span>|<span data-ttu-id="094b3-176">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="094b3-176">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="094b3-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="094b3-177">sensitivity</span></span>|<span data-ttu-id="094b3-178">String</span><span class="sxs-lookup"><span data-stu-id="094b3-178">String</span></span>| <span data-ttu-id="094b3-179">可能的值是：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="094b3-179">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="094b3-180">showAs</span><span class="sxs-lookup"><span data-stu-id="094b3-180">showAs</span></span>|<span data-ttu-id="094b3-181">String</span><span class="sxs-lookup"><span data-stu-id="094b3-181">String</span></span>|<span data-ttu-id="094b3-182">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="094b3-182">The status to show.</span></span> <span data-ttu-id="094b3-183">可能的值为： `free` ， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。</span><span class="sxs-lookup"><span data-stu-id="094b3-183">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="094b3-184">start</span><span class="sxs-lookup"><span data-stu-id="094b3-184">start</span></span>|<span data-ttu-id="094b3-185">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="094b3-185">DateTimeTimeZone</span></span>|<span data-ttu-id="094b3-186">事件的开始时间。</span><span class="sxs-lookup"><span data-stu-id="094b3-186">The start time of the event.</span></span> <br/><br/><span data-ttu-id="094b3-p109">默认情况下，开始时间使用 UTC 格式。可以在 StartTimeZone 中指定可选的时区，用该时区表示开始时间并包括与 UTC 的时间偏移量。请注意，如果使用 StartTimeZone，你也必须为 EndTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="094b3-p109">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="094b3-190">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 7:34：“2015-02-25T19:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="094b3-190">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="094b3-191">subject</span><span class="sxs-lookup"><span data-stu-id="094b3-191">subject</span></span>|<span data-ttu-id="094b3-192">String</span><span class="sxs-lookup"><span data-stu-id="094b3-192">String</span></span>|<span data-ttu-id="094b3-193">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="094b3-193">The text of the event's subject line.</span></span>|

<span data-ttu-id="094b3-194">由于**事件**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**事件**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="094b3-194">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="094b3-195">如果您要更新的**事件**是定期系列的主事件，包含多个与会者，并且包含单独已更新的实例，多个电子邮件发送的通知： 一个用于主系列，每个实例具有一个已进行了更新。</span><span class="sxs-lookup"><span data-stu-id="094b3-195">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="094b3-196">响应</span><span class="sxs-lookup"><span data-stu-id="094b3-196">Response</span></span>

<span data-ttu-id="094b3-197">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="094b3-197">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="094b3-198">**注意：** 此方法可返回的错误代码 HTTP 400 错误请求响应`ErrorOccurrenceCrossingBoundary`并显示以下错误消息： 已修改的事件是通过或重叠相邻事件。</span><span class="sxs-lookup"><span data-stu-id="094b3-198">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="094b3-199">这指示更新违反了以下 Outlook 限制重复例外： 出现或上一个匹配项，天之前不能移动，不能将移动到或之后的以下匹配项的天。</span><span class="sxs-lookup"><span data-stu-id="094b3-199">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="094b3-200">示例</span><span class="sxs-lookup"><span data-stu-id="094b3-200">Example</span></span>

##### <a name="request"></a><span data-ttu-id="094b3-201">请求</span><span class="sxs-lookup"><span data-stu-id="094b3-201">Request</span></span>

<span data-ttu-id="094b3-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="094b3-202">Here is an example of the request.</span></span>
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
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="094b3-203">响应</span><span class="sxs-lookup"><span data-stu-id="094b3-203">Response</span></span>
<span data-ttu-id="094b3-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="094b3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isReminderOn": true
}
```


## <a name="see-also"></a><span data-ttu-id="094b3-207">另请参阅</span><span class="sxs-lookup"><span data-stu-id="094b3-207">See also</span></span>

- [<span data-ttu-id="094b3-208">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="094b3-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="094b3-209">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="094b3-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="094b3-210">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="094b3-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
