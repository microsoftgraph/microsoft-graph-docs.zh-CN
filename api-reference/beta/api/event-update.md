---
title: 更新事件
description: 更新事件对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ec274fb0e850a3a18b3722e27bbe394986459cbb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329795"
---
# <a name="update-event"></a><span data-ttu-id="466c3-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="466c3-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="466c3-104">更新[事件](../resources/event.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="466c3-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="466c3-105">权限</span><span class="sxs-lookup"><span data-stu-id="466c3-105">Permissions</span></span>
<span data-ttu-id="466c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="466c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="466c3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="466c3-108">Permission type</span></span>      | <span data-ttu-id="466c3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="466c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="466c3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="466c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="466c3-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="466c3-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="466c3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="466c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="466c3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="466c3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="466c3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="466c3-114">Application</span></span> | <span data-ttu-id="466c3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="466c3-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="466c3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="466c3-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="466c3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="466c3-117">Request headers</span></span>
| <span data-ttu-id="466c3-118">名称</span><span class="sxs-lookup"><span data-stu-id="466c3-118">Name</span></span>       | <span data-ttu-id="466c3-119">类型</span><span class="sxs-lookup"><span data-stu-id="466c3-119">Type</span></span> | <span data-ttu-id="466c3-120">说明</span><span class="sxs-lookup"><span data-stu-id="466c3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="466c3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="466c3-121">Authorization</span></span>  | <span data-ttu-id="466c3-122">字符串</span><span class="sxs-lookup"><span data-stu-id="466c3-122">string</span></span>  | <span data-ttu-id="466c3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="466c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="466c3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="466c3-125">Request body</span></span>
<span data-ttu-id="466c3-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="466c3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="466c3-129">属性</span><span class="sxs-lookup"><span data-stu-id="466c3-129">Property</span></span>       | <span data-ttu-id="466c3-130">类型</span><span class="sxs-lookup"><span data-stu-id="466c3-130">Type</span></span>    | <span data-ttu-id="466c3-131">说明</span><span class="sxs-lookup"><span data-stu-id="466c3-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="466c3-132">attendees</span><span class="sxs-lookup"><span data-stu-id="466c3-132">attendees</span></span>|<span data-ttu-id="466c3-133">与会者</span><span class="sxs-lookup"><span data-stu-id="466c3-133">Attendee</span></span>|<span data-ttu-id="466c3-134">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="466c3-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="466c3-135">body</span><span class="sxs-lookup"><span data-stu-id="466c3-135">body</span></span>|<span data-ttu-id="466c3-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="466c3-136">ItemBody</span></span>|<span data-ttu-id="466c3-137">与事件相关联的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="466c3-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="466c3-138">categories</span><span class="sxs-lookup"><span data-stu-id="466c3-138">categories</span></span>|<span data-ttu-id="466c3-139">String</span><span class="sxs-lookup"><span data-stu-id="466c3-139">String</span></span>|<span data-ttu-id="466c3-140">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="466c3-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="466c3-141">end</span><span class="sxs-lookup"><span data-stu-id="466c3-141">end</span></span>|<span data-ttu-id="466c3-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="466c3-142">DateTimeTimeZone</span></span>|<span data-ttu-id="466c3-143">事件的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="466c3-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="466c3-p104">默认情况下，结束时间使用 UTC 格式。可以在 EndTimeZone 中指定可选的时区，用该时区表示结束时间并包括与 UTC 的时间偏移量。请注意，如果使用 EndTimeZone，必须为 StartTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="466c3-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="466c3-147">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 9:34：“2015-02-25T21:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="466c3-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="466c3-148">importance</span><span class="sxs-lookup"><span data-stu-id="466c3-148">importance</span></span>|<span data-ttu-id="466c3-149">String</span><span class="sxs-lookup"><span data-stu-id="466c3-149">String</span></span>|<span data-ttu-id="466c3-150">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="466c3-150">The importance of the event.</span></span> <span data-ttu-id="466c3-151">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="466c3-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="466c3-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="466c3-152">isAllDay</span></span>|<span data-ttu-id="466c3-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="466c3-153">Boolean</span></span>|<span data-ttu-id="466c3-154">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="466c3-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="466c3-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="466c3-155">isReminderOn</span></span>|<span data-ttu-id="466c3-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="466c3-156">Boolean</span></span>|<span data-ttu-id="466c3-157">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="466c3-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="466c3-158">位置</span><span class="sxs-lookup"><span data-stu-id="466c3-158">location</span></span>|<span data-ttu-id="466c3-159">位置</span><span class="sxs-lookup"><span data-stu-id="466c3-159">Location</span></span>|<span data-ttu-id="466c3-160">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="466c3-160">The location of the event.</span></span>|
|<span data-ttu-id="466c3-161">位置</span><span class="sxs-lookup"><span data-stu-id="466c3-161">locations</span></span>|<span data-ttu-id="466c3-162">[location](../resources/location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="466c3-162">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="466c3-163">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="466c3-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="466c3-164">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="466c3-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="466c3-165">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="466c3-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="466c3-166">定期</span><span class="sxs-lookup"><span data-stu-id="466c3-166">recurrence</span></span>|<span data-ttu-id="466c3-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="466c3-167">PatternedRecurrence</span></span>|<span data-ttu-id="466c3-168">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="466c3-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="466c3-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="466c3-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="466c3-170">Int32</span><span class="sxs-lookup"><span data-stu-id="466c3-170">Int32</span></span>|<span data-ttu-id="466c3-171">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="466c3-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="466c3-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="466c3-172">responseRequested</span></span>|<span data-ttu-id="466c3-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="466c3-173">Boolean</span></span>|<span data-ttu-id="466c3-174">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="466c3-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="466c3-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="466c3-175">sensitivity</span></span>|<span data-ttu-id="466c3-176">String</span><span class="sxs-lookup"><span data-stu-id="466c3-176">String</span></span>| <span data-ttu-id="466c3-177">可能的值是：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="466c3-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="466c3-178">showAs</span><span class="sxs-lookup"><span data-stu-id="466c3-178">showAs</span></span>|<span data-ttu-id="466c3-179">String</span><span class="sxs-lookup"><span data-stu-id="466c3-179">String</span></span>|<span data-ttu-id="466c3-180">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="466c3-180">The status to show.</span></span> <span data-ttu-id="466c3-181">可能的值为`free` : `tentative`、 `busy`、 `oof`、 `workingElsewhere`、 `unknown`、。</span><span class="sxs-lookup"><span data-stu-id="466c3-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="466c3-182">start</span><span class="sxs-lookup"><span data-stu-id="466c3-182">start</span></span>|<span data-ttu-id="466c3-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="466c3-183">DateTimeTimeZone</span></span>|<span data-ttu-id="466c3-184">事件的开始时间。</span><span class="sxs-lookup"><span data-stu-id="466c3-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="466c3-p108">默认情况下，开始时间使用 UTC 格式。可以在 StartTimeZone 中指定可选的时区，用该时区表示开始时间并包括与 UTC 的时间偏移量。请注意，如果使用 StartTimeZone，你也必须为 EndTimeZone 指定一个值。</span><span class="sxs-lookup"><span data-stu-id="466c3-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="466c3-188">本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 7:34：“2015-02-25T19:34:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="466c3-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="466c3-189">subject</span><span class="sxs-lookup"><span data-stu-id="466c3-189">subject</span></span>|<span data-ttu-id="466c3-190">String</span><span class="sxs-lookup"><span data-stu-id="466c3-190">String</span></span>|<span data-ttu-id="466c3-191">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="466c3-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="466c3-192">由于**事件**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**事件**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="466c3-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="466c3-193">如果您正在更新的**事件**是定期系列的主事件, 包含多个与会者, 并且具有单独更新的实例, 则会发出多个通知电子邮件: 一个主系列, 一个是, 每个实例包含已更新。</span><span class="sxs-lookup"><span data-stu-id="466c3-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="466c3-194">响应</span><span class="sxs-lookup"><span data-stu-id="466c3-194">Response</span></span>

<span data-ttu-id="466c3-195">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="466c3-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="466c3-196">**注意:** 此方法可以返回一个错误代码为的`ErrorOccurrenceCrossingBoundary` HTTP 400 请求响应, 并返回以下错误消息: 修改的事件发生交叉或重叠的相邻事件。</span><span class="sxs-lookup"><span data-stu-id="466c3-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="466c3-197">这表明更新违反了对定期例外的以下 Outlook 限制: 不能将事件移到上一次出现的日期之前或之前, 也不能将其移至以下事件的日期或时间。</span><span class="sxs-lookup"><span data-stu-id="466c3-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="466c3-198">示例</span><span class="sxs-lookup"><span data-stu-id="466c3-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="466c3-199">请求</span><span class="sxs-lookup"><span data-stu-id="466c3-199">Request</span></span>

<span data-ttu-id="466c3-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="466c3-200">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="466c3-201">响应</span><span class="sxs-lookup"><span data-stu-id="466c3-201">Response</span></span>
<span data-ttu-id="466c3-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="466c3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="466c3-205">另请参阅</span><span class="sxs-lookup"><span data-stu-id="466c3-205">See also</span></span>

- [<span data-ttu-id="466c3-206">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="466c3-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="466c3-207">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="466c3-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="466c3-208">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="466c3-208">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
