---
title: 更新事件
description: 更新 event 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0c9b182d4a586b43aead0023651844dc98581da0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586371"
---
# <a name="update-event"></a><span data-ttu-id="73518-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="73518-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73518-104">更新 [event](../resources/event.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73518-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="73518-105">权限</span><span class="sxs-lookup"><span data-stu-id="73518-105">Permissions</span></span>
<span data-ttu-id="73518-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73518-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73518-108">Permission type</span></span>      | <span data-ttu-id="73518-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73518-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73518-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73518-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73518-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73518-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="73518-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73518-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73518-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73518-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="73518-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73518-114">Application</span></span> | <span data-ttu-id="73518-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73518-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73518-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73518-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="73518-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="73518-117">Request headers</span></span>
| <span data-ttu-id="73518-118">名称</span><span class="sxs-lookup"><span data-stu-id="73518-118">Name</span></span>       | <span data-ttu-id="73518-119">类型</span><span class="sxs-lookup"><span data-stu-id="73518-119">Type</span></span> | <span data-ttu-id="73518-120">说明</span><span class="sxs-lookup"><span data-stu-id="73518-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73518-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73518-121">Authorization</span></span>  | <span data-ttu-id="73518-122">string</span><span class="sxs-lookup"><span data-stu-id="73518-122">string</span></span>  | <span data-ttu-id="73518-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73518-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73518-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="73518-125">Request body</span></span>
<span data-ttu-id="73518-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="73518-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73518-129">属性</span><span class="sxs-lookup"><span data-stu-id="73518-129">Property</span></span>       | <span data-ttu-id="73518-130">类型</span><span class="sxs-lookup"><span data-stu-id="73518-130">Type</span></span>    | <span data-ttu-id="73518-131">说明</span><span class="sxs-lookup"><span data-stu-id="73518-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="73518-132">attendees</span><span class="sxs-lookup"><span data-stu-id="73518-132">attendees</span></span>|<span data-ttu-id="73518-133">与会者</span><span class="sxs-lookup"><span data-stu-id="73518-133">Attendee</span></span>|<span data-ttu-id="73518-134">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="73518-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="73518-135">body</span><span class="sxs-lookup"><span data-stu-id="73518-135">body</span></span>|<span data-ttu-id="73518-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="73518-136">ItemBody</span></span>|<span data-ttu-id="73518-137">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="73518-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="73518-138">categories</span><span class="sxs-lookup"><span data-stu-id="73518-138">categories</span></span>|<span data-ttu-id="73518-139">String</span><span class="sxs-lookup"><span data-stu-id="73518-139">String</span></span>|<span data-ttu-id="73518-140">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="73518-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="73518-141">end</span><span class="sxs-lookup"><span data-stu-id="73518-141">end</span></span>|<span data-ttu-id="73518-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="73518-142">DateTimeTimeZone</span></span>|<span data-ttu-id="73518-143">事件的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73518-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="73518-p104">默认情况下，结束时间使用 UTC 格式。可以在 EndTimeZone 中指定可选的时区，用该时区表示结束时间并包括与 UTC 的时间偏移量。请注意，如果使用 EndTimeZone，必须为 StartTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="73518-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="73518-147">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 9:34：“2015-02-25T21:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="73518-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="73518-148">重要性</span><span class="sxs-lookup"><span data-stu-id="73518-148">importance</span></span>|<span data-ttu-id="73518-149">String</span><span class="sxs-lookup"><span data-stu-id="73518-149">String</span></span>|<span data-ttu-id="73518-150">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="73518-150">The importance of the event.</span></span> <span data-ttu-id="73518-151">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="73518-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="73518-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="73518-152">isAllDay</span></span>|<span data-ttu-id="73518-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="73518-153">Boolean</span></span>|<span data-ttu-id="73518-154">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="73518-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="73518-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="73518-155">isReminderOn</span></span>|<span data-ttu-id="73518-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="73518-156">Boolean</span></span>|<span data-ttu-id="73518-157">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="73518-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="73518-158">位置</span><span class="sxs-lookup"><span data-stu-id="73518-158">location</span></span>|<span data-ttu-id="73518-159">位置</span><span class="sxs-lookup"><span data-stu-id="73518-159">Location</span></span>|<span data-ttu-id="73518-160">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="73518-160">The location of the event.</span></span>|
|<span data-ttu-id="73518-161">locations</span><span class="sxs-lookup"><span data-stu-id="73518-161">locations</span></span>|<span data-ttu-id="73518-162">[location](../resources/location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73518-162">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="73518-163">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="73518-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="73518-164">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="73518-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="73518-165">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="73518-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="73518-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="73518-166">recurrence</span></span>|<span data-ttu-id="73518-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="73518-167">PatternedRecurrence</span></span>|<span data-ttu-id="73518-168">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="73518-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="73518-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="73518-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="73518-170">Int32</span><span class="sxs-lookup"><span data-stu-id="73518-170">Int32</span></span>|<span data-ttu-id="73518-171">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="73518-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="73518-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="73518-172">responseRequested</span></span>|<span data-ttu-id="73518-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="73518-173">Boolean</span></span>|<span data-ttu-id="73518-174">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="73518-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="73518-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="73518-175">sensitivity</span></span>|<span data-ttu-id="73518-176">String</span><span class="sxs-lookup"><span data-stu-id="73518-176">String</span></span>| <span data-ttu-id="73518-177">可能的值是：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="73518-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="73518-178">showAs</span><span class="sxs-lookup"><span data-stu-id="73518-178">showAs</span></span>|<span data-ttu-id="73518-179">String</span><span class="sxs-lookup"><span data-stu-id="73518-179">String</span></span>|<span data-ttu-id="73518-180">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="73518-180">The status to show.</span></span> <span data-ttu-id="73518-181">可能的值为`free` : `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`、。</span><span class="sxs-lookup"><span data-stu-id="73518-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="73518-182">start</span><span class="sxs-lookup"><span data-stu-id="73518-182">start</span></span>|<span data-ttu-id="73518-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="73518-183">DateTimeTimeZone</span></span>|<span data-ttu-id="73518-184">事件的开始时间。</span><span class="sxs-lookup"><span data-stu-id="73518-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="73518-p108">默认情况下，开始时间使用 UTC 格式。可以在 StartTimeZone 中指定可选的时区，用该时区表示开始时间并包括与 UTC 的时间偏移量。请注意，如果使用 StartTimeZone，你也必须为 EndTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="73518-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="73518-188">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 7:34：“2015-02-25T19:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="73518-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="73518-189">subject</span><span class="sxs-lookup"><span data-stu-id="73518-189">subject</span></span>|<span data-ttu-id="73518-190">String</span><span class="sxs-lookup"><span data-stu-id="73518-190">String</span></span>|<span data-ttu-id="73518-191">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="73518-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="73518-192">由于**事件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**事件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="73518-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="73518-193">如果你正更新的**事件**是定期系列的主事件，包含多个与会者，并且具有已单独更新的实例，则将发送多个通知电子邮件：一个用于主系列，另一个用于已更新的实例。</span><span class="sxs-lookup"><span data-stu-id="73518-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="73518-194">响应</span><span class="sxs-lookup"><span data-stu-id="73518-194">Response</span></span>

<span data-ttu-id="73518-195">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73518-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="73518-196">注意：此方法可以返回 HTTP 400 错误请求响应，错误代码为 `ErrorOccurrenceCrossingBoundary`，并显示以下错误消息：已修改的事件正在交叉或重叠相邻的事件。</span><span class="sxs-lookup"><span data-stu-id="73518-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="73518-197">这表示更新违反了重复例外的以下 Outlook 限制：事件无法移动到上一次发生的日期或之前，并且无法移动到下一次发生的日期或之后。 </span><span class="sxs-lookup"><span data-stu-id="73518-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="73518-198">示例</span><span class="sxs-lookup"><span data-stu-id="73518-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73518-199">请求</span><span class="sxs-lookup"><span data-stu-id="73518-199">Request</span></span>

<span data-ttu-id="73518-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73518-200">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="73518-201">响应</span><span class="sxs-lookup"><span data-stu-id="73518-201">Response</span></span>
<span data-ttu-id="73518-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73518-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="73518-205">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="73518-205">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="73518-206">语言</span><span class="sxs-lookup"><span data-stu-id="73518-206">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73518-207">Javascript</span><span class="sxs-lookup"><span data-stu-id="73518-207">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="see-also"></a><span data-ttu-id="73518-208">另请参阅</span><span class="sxs-lookup"><span data-stu-id="73518-208">See also</span></span>

- [<span data-ttu-id="73518-209">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="73518-209">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="73518-210">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="73518-210">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="73518-211">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="73518-211">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/event-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
