---
title: 更新事件
description: 更新 event 对象的属性。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 564cea7760c7e91102ce47ab725b27871a3b6f86
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002802"
---
# <a name="update-event"></a><span data-ttu-id="2e90f-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="2e90f-103">Update event</span></span>

<span data-ttu-id="2e90f-104">更新 [event](../resources/event.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e90f-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="2e90f-105">更新事件开始或结束时间的时区时，首先[找到支持的时区](outlookuser-supportedtimezones.md)，以确保仅设置针对用户的邮箱服务器配置的时区。</span><span class="sxs-lookup"><span data-stu-id="2e90f-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2e90f-106">权限</span><span class="sxs-lookup"><span data-stu-id="2e90f-106">Permissions</span></span>
<span data-ttu-id="2e90f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e90f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e90f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e90f-109">Permission type</span></span>      | <span data-ttu-id="2e90f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e90f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e90f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e90f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e90f-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e90f-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e90f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e90f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e90f-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e90f-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2e90f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e90f-115">Application</span></span> | <span data-ttu-id="2e90f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e90f-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e90f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e90f-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="2e90f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e90f-118">Request headers</span></span>
| <span data-ttu-id="2e90f-119">名称</span><span class="sxs-lookup"><span data-stu-id="2e90f-119">Name</span></span>       | <span data-ttu-id="2e90f-120">类型</span><span class="sxs-lookup"><span data-stu-id="2e90f-120">Type</span></span> | <span data-ttu-id="2e90f-121">说明</span><span class="sxs-lookup"><span data-stu-id="2e90f-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e90f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e90f-122">Authorization</span></span>  | <span data-ttu-id="2e90f-123">string</span><span class="sxs-lookup"><span data-stu-id="2e90f-123">string</span></span>  | <span data-ttu-id="2e90f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e90f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e90f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e90f-126">Request body</span></span>
<span data-ttu-id="2e90f-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2e90f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e90f-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e90f-130">Property</span></span>     | <span data-ttu-id="2e90f-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e90f-131">Type</span></span>   |<span data-ttu-id="2e90f-132">说明</span><span class="sxs-lookup"><span data-stu-id="2e90f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e90f-133">attendees</span><span class="sxs-lookup"><span data-stu-id="2e90f-133">attendees</span></span>|[<span data-ttu-id="2e90f-134">与会者</span><span class="sxs-lookup"><span data-stu-id="2e90f-134">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="2e90f-135">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="2e90f-135">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="2e90f-136">body</span><span class="sxs-lookup"><span data-stu-id="2e90f-136">body</span></span>|[<span data-ttu-id="2e90f-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="2e90f-137">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="2e90f-138">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="2e90f-138">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="2e90f-139">categories</span><span class="sxs-lookup"><span data-stu-id="2e90f-139">categories</span></span>|<span data-ttu-id="2e90f-140">String</span><span class="sxs-lookup"><span data-stu-id="2e90f-140">String</span></span>|<span data-ttu-id="2e90f-141">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="2e90f-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="2e90f-142">end</span><span class="sxs-lookup"><span data-stu-id="2e90f-142">end</span></span>|<span data-ttu-id="2e90f-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e90f-143">DateTimeTimeZone</span></span>|<span data-ttu-id="2e90f-144">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="2e90f-144">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="2e90f-145">importance</span><span class="sxs-lookup"><span data-stu-id="2e90f-145">importance</span></span>|<span data-ttu-id="2e90f-146">String</span><span class="sxs-lookup"><span data-stu-id="2e90f-146">String</span></span>|<span data-ttu-id="2e90f-147">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="2e90f-147">The importance of the event.</span></span> <span data-ttu-id="2e90f-148">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="2e90f-148">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="2e90f-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="2e90f-149">isAllDay</span></span>|<span data-ttu-id="2e90f-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e90f-150">Boolean</span></span>|<span data-ttu-id="2e90f-151">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2e90f-151">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="2e90f-152">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="2e90f-152">isReminderOn</span></span>|<span data-ttu-id="2e90f-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e90f-153">Boolean</span></span>|<span data-ttu-id="2e90f-154">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2e90f-154">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="2e90f-155">位置</span><span class="sxs-lookup"><span data-stu-id="2e90f-155">location</span></span>|[<span data-ttu-id="2e90f-156">位置</span><span class="sxs-lookup"><span data-stu-id="2e90f-156">Location</span></span>](../resources/location.md)|<span data-ttu-id="2e90f-157">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="2e90f-157">The location of the event.</span></span>|
|<span data-ttu-id="2e90f-158">locations</span><span class="sxs-lookup"><span data-stu-id="2e90f-158">locations</span></span>|<span data-ttu-id="2e90f-159">[location](../resources/location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e90f-159">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="2e90f-160">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="2e90f-160">The locations where the event is held or attended from.</span></span> <span data-ttu-id="2e90f-161">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="2e90f-161">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="2e90f-162">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="2e90f-162">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="2e90f-163">recurrence</span><span class="sxs-lookup"><span data-stu-id="2e90f-163">recurrence</span></span>|[<span data-ttu-id="2e90f-164">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="2e90f-164">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="2e90f-165">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="2e90f-165">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="2e90f-166">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="2e90f-166">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="2e90f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="2e90f-167">Int32</span></span>|<span data-ttu-id="2e90f-168">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2e90f-168">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="2e90f-169">responseRequested</span><span class="sxs-lookup"><span data-stu-id="2e90f-169">responseRequested</span></span>|<span data-ttu-id="2e90f-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e90f-170">Boolean</span></span>|<span data-ttu-id="2e90f-171">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2e90f-171">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="2e90f-172">sensitivity</span><span class="sxs-lookup"><span data-stu-id="2e90f-172">sensitivity</span></span>|<span data-ttu-id="2e90f-173">String</span><span class="sxs-lookup"><span data-stu-id="2e90f-173">String</span></span>| <span data-ttu-id="2e90f-174">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="2e90f-174">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="2e90f-175">showAs</span><span class="sxs-lookup"><span data-stu-id="2e90f-175">showAs</span></span>|<span data-ttu-id="2e90f-176">String</span><span class="sxs-lookup"><span data-stu-id="2e90f-176">String</span></span>|<span data-ttu-id="2e90f-177">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="2e90f-177">The status to show.</span></span> <span data-ttu-id="2e90f-178">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="2e90f-178">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="2e90f-179">start</span><span class="sxs-lookup"><span data-stu-id="2e90f-179">start</span></span>|<span data-ttu-id="2e90f-180">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e90f-180">DateTimeTimeZone</span></span>|<span data-ttu-id="2e90f-181">事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="2e90f-181">The date, time, and time zone that the event starts.</span></span> |
|<span data-ttu-id="2e90f-182">subject</span><span class="sxs-lookup"><span data-stu-id="2e90f-182">subject</span></span>|<span data-ttu-id="2e90f-183">String</span><span class="sxs-lookup"><span data-stu-id="2e90f-183">String</span></span>|<span data-ttu-id="2e90f-184">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="2e90f-184">The text of the event's subject line.</span></span>|

<span data-ttu-id="2e90f-185">由于**事件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**事件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="2e90f-185">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="2e90f-186">如果你正更新的**事件**是定期系列的主事件，包含多个与会者，并且具有已单独更新的实例，则将发送多个通知电子邮件：一个用于主系列，另一个用于已更新的实例。</span><span class="sxs-lookup"><span data-stu-id="2e90f-186">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="2e90f-187">响应</span><span class="sxs-lookup"><span data-stu-id="2e90f-187">Response</span></span>

<span data-ttu-id="2e90f-188">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e90f-188">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="2e90f-189">**注意：** 此方法可以返回 HTTP 400 错误请求响应，错误代码为 `ErrorOccurrenceCrossingBoundary`，并显示以下错误消息：已修改的事件正在交叉或重叠相邻的事件。</span><span class="sxs-lookup"><span data-stu-id="2e90f-189">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="2e90f-190">这表示更新违反了重复例外的以下 Outlook 限制：事件无法移动到上一次发生的日期或之前，并且无法移动到下一次发生的日期或之后。 </span><span class="sxs-lookup"><span data-stu-id="2e90f-190">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="2e90f-191">示例</span><span class="sxs-lookup"><span data-stu-id="2e90f-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e90f-192">请求</span><span class="sxs-lookup"><span data-stu-id="2e90f-192">Request</span></span>

<span data-ttu-id="2e90f-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e90f-193">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2e90f-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e90f-194">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e90f-195">C#</span><span class="sxs-lookup"><span data-stu-id="2e90f-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e90f-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="2e90f-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2e90f-197">Java</span><span class="sxs-lookup"><span data-stu-id="2e90f-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e90f-198">响应</span><span class="sxs-lookup"><span data-stu-id="2e90f-198">Response</span></span>

<span data-ttu-id="2e90f-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e90f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2e90f-202">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e90f-202">See also</span></span>

- [<span data-ttu-id="2e90f-203">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e90f-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2e90f-204">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e90f-204">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2e90f-205">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e90f-205">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



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
