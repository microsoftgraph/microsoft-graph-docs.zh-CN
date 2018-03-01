# <a name="update-event"></a><span data-ttu-id="160d0-101">更新事件</span><span class="sxs-lookup"><span data-stu-id="160d0-101">Update event</span></span>

<span data-ttu-id="160d0-102">更新 event 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="160d0-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="160d0-103">权限</span><span class="sxs-lookup"><span data-stu-id="160d0-103">Permissions</span></span>
<span data-ttu-id="160d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="160d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="160d0-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="160d0-106">Permission type</span></span>      | <span data-ttu-id="160d0-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="160d0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="160d0-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="160d0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="160d0-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="160d0-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="160d0-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="160d0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="160d0-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="160d0-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="160d0-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="160d0-112">Application</span></span> | <span data-ttu-id="160d0-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="160d0-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="160d0-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="160d0-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="160d0-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="160d0-115">Request headers</span></span>
| <span data-ttu-id="160d0-116">名称</span><span class="sxs-lookup"><span data-stu-id="160d0-116">Name</span></span>       | <span data-ttu-id="160d0-117">类型</span><span class="sxs-lookup"><span data-stu-id="160d0-117">Type</span></span> | <span data-ttu-id="160d0-118">说明</span><span class="sxs-lookup"><span data-stu-id="160d0-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="160d0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="160d0-119">Authorization</span></span>  | <span data-ttu-id="160d0-120">string</span><span class="sxs-lookup"><span data-stu-id="160d0-120">string</span></span>  | <span data-ttu-id="160d0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="160d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="160d0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="160d0-123">Request body</span></span>
<span data-ttu-id="160d0-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="160d0-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="160d0-127">属性</span><span class="sxs-lookup"><span data-stu-id="160d0-127">Property</span></span>     | <span data-ttu-id="160d0-128">类型</span><span class="sxs-lookup"><span data-stu-id="160d0-128">Type</span></span>   |<span data-ttu-id="160d0-129">说明</span><span class="sxs-lookup"><span data-stu-id="160d0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="160d0-130">attendees</span><span class="sxs-lookup"><span data-stu-id="160d0-130">attendees</span></span>|[<span data-ttu-id="160d0-131">与会者</span><span class="sxs-lookup"><span data-stu-id="160d0-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="160d0-132">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="160d0-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="160d0-133">body</span><span class="sxs-lookup"><span data-stu-id="160d0-133">body</span></span>|[<span data-ttu-id="160d0-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="160d0-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="160d0-135">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="160d0-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="160d0-136">categories</span><span class="sxs-lookup"><span data-stu-id="160d0-136">categories</span></span>|<span data-ttu-id="160d0-137">String</span><span class="sxs-lookup"><span data-stu-id="160d0-137">String</span></span>|<span data-ttu-id="160d0-138">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="160d0-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="160d0-139">end</span><span class="sxs-lookup"><span data-stu-id="160d0-139">end</span></span>|[<span data-ttu-id="160d0-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="160d0-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="160d0-141">事件的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="160d0-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="160d0-p104">默认情况下，结束时间使用 UTC 格式。可以在 EndTimeZone 中指定可选的时区，用该时区表示结束时间并包括与 UTC 的时间偏移量。请注意，如果使用 EndTimeZone，必须为 StartTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="160d0-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="160d0-145">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 9:34：“2015-02-25T21:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="160d0-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="160d0-146">重要性</span><span class="sxs-lookup"><span data-stu-id="160d0-146">importance</span></span>|<span data-ttu-id="160d0-147">String</span><span class="sxs-lookup"><span data-stu-id="160d0-147">String</span></span>|<span data-ttu-id="160d0-148">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="160d0-148">The importance of the event.</span></span> <span data-ttu-id="160d0-149">可取值为：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="160d0-149">Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="160d0-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="160d0-150">isAllDay</span></span>|<span data-ttu-id="160d0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="160d0-151">Boolean</span></span>|<span data-ttu-id="160d0-152">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="160d0-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="160d0-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="160d0-153">isReminderOn</span></span>|<span data-ttu-id="160d0-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="160d0-154">Boolean</span></span>|<span data-ttu-id="160d0-155">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="160d0-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="160d0-156">位置</span><span class="sxs-lookup"><span data-stu-id="160d0-156">location</span></span>|[<span data-ttu-id="160d0-157">位置</span><span class="sxs-lookup"><span data-stu-id="160d0-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="160d0-158">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="160d0-158">The location of the event.</span></span>|
|<span data-ttu-id="160d0-159">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="160d0-159">onlineMeetingUrl</span></span>|<span data-ttu-id="160d0-160">String</span><span class="sxs-lookup"><span data-stu-id="160d0-160">String</span></span>|<span data-ttu-id="160d0-161">在线会议的链接。</span><span class="sxs-lookup"><span data-stu-id="160d0-161">A URL for an online meeting.</span></span>|
|<span data-ttu-id="160d0-162">recurrence</span><span class="sxs-lookup"><span data-stu-id="160d0-162">recurrence</span></span>|[<span data-ttu-id="160d0-163">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="160d0-163">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="160d0-164">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="160d0-164">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="160d0-165">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="160d0-165">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="160d0-166">Int32</span><span class="sxs-lookup"><span data-stu-id="160d0-166">Int32</span></span>|<span data-ttu-id="160d0-167">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="160d0-167">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="160d0-168">responseRequested</span><span class="sxs-lookup"><span data-stu-id="160d0-168">responseRequested</span></span>|<span data-ttu-id="160d0-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="160d0-169">Boolean</span></span>|<span data-ttu-id="160d0-170">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="160d0-170">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="160d0-171">sensitivity</span><span class="sxs-lookup"><span data-stu-id="160d0-171">sensitivity</span></span>|<span data-ttu-id="160d0-172">String</span><span class="sxs-lookup"><span data-stu-id="160d0-172">String</span></span>| <span data-ttu-id="160d0-173">可能的值是：`Normal`、`Personal`、`Private`、`Confidential`。</span><span class="sxs-lookup"><span data-stu-id="160d0-173">Possible values are: `Normal`, `Personal`, `Private`, `Confidential`.</span></span>|
|<span data-ttu-id="160d0-174">showAs</span><span class="sxs-lookup"><span data-stu-id="160d0-174">showAs</span></span>|<span data-ttu-id="160d0-175">String</span><span class="sxs-lookup"><span data-stu-id="160d0-175">String</span></span>|<span data-ttu-id="160d0-176">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="160d0-176">The status to show.</span></span> <span data-ttu-id="160d0-177">可取值为 `Free`、`Tentative`、`Busy`、`Oof`、`WorkingElsewhere`、`Unknown`。</span><span class="sxs-lookup"><span data-stu-id="160d0-177">Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.</span></span>|
|<span data-ttu-id="160d0-178">start</span><span class="sxs-lookup"><span data-stu-id="160d0-178">start</span></span>|[<span data-ttu-id="160d0-179">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="160d0-179">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="160d0-180">事件的开始时间。</span><span class="sxs-lookup"><span data-stu-id="160d0-180">The start time of the event.</span></span> <br/><br/><span data-ttu-id="160d0-p107">默认情况下，开始时间使用 UTC 格式。可以在 StartTimeZone 中指定可选的时区，用该时区表示开始时间并包括与 UTC 的时间偏移量。请注意，如果使用 StartTimeZone，你也必须为 EndTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="160d0-p107">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="160d0-184">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 7:34：“2015-02-25T19:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="160d0-184">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="160d0-185">subject</span><span class="sxs-lookup"><span data-stu-id="160d0-185">subject</span></span>|<span data-ttu-id="160d0-186">String</span><span class="sxs-lookup"><span data-stu-id="160d0-186">String</span></span>|<span data-ttu-id="160d0-187">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="160d0-187">The text of the event's subject line.</span></span>|

<span data-ttu-id="160d0-188">由于**事件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此可以使用 `PATCH` 操作在现有**事件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="160d0-188">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="160d0-189">响应</span><span class="sxs-lookup"><span data-stu-id="160d0-189">Response</span></span>

<span data-ttu-id="160d0-190">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="160d0-190">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="160d0-191">示例</span><span class="sxs-lookup"><span data-stu-id="160d0-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="160d0-192">请求</span><span class="sxs-lookup"><span data-stu-id="160d0-192">Request</span></span>

<span data-ttu-id="160d0-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="160d0-193">Here is an example of the request.</span></span>
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
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="160d0-194">响应</span><span class="sxs-lookup"><span data-stu-id="160d0-194">Response</span></span>

<span data-ttu-id="160d0-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="160d0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isReminderOn": true
}
```

## <a name="see-also"></a><span data-ttu-id="160d0-198">另请参阅</span><span class="sxs-lookup"><span data-stu-id="160d0-198">See also</span></span>

- [<span data-ttu-id="160d0-199">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="160d0-199">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="160d0-200">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="160d0-200">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
