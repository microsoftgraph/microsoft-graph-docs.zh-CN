---
title: 创建事件
description: 在用户的默认日历或指定日历中创建事件。
localization_priority: Normal
doc_type: apiPageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: cad97bd555d6d0388f6f402f1365a152942af34b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049623"
---
# <a name="create-event"></a><span data-ttu-id="a3911-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="a3911-103">Create Event</span></span>

<span data-ttu-id="a3911-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3911-105">在用户的默认日历或指定日历中创建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="a3911-105">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="a3911-106">默认情况下，创建事件时，**allowNewTimeProposals** 的属性设置为 true，这意味着被邀请者可以为事件建议不同的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a3911-106">By default, the **allowNewTimeProposals** property is set to true when an event is created, which means invitees can propose a different date/time for the event.</span></span> <span data-ttu-id="a3911-107">有关如何建议时间的详细信息，以及如何接收和接受新的时间建议，请参阅 [建议新的会议时间](/graph/outlook-calendar-meeting-proposals)。</span><span class="sxs-lookup"><span data-stu-id="a3911-107">See [Propose new meeting times](/graph/outlook-calendar-meeting-proposals) for more information on how to propose a time, and how to receive and accept a new time proposal.</span></span>

<span data-ttu-id="a3911-108">可以将事件的各开始和结束时间的时区指定为其值的一部分，因为 **开始** 和 **结束** 属性为 [dateTimeTimeZone](../resources/datetimetimezone.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="a3911-108">You can specify the time zone for each of the start and end times of the event as part of their values, because the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> <span data-ttu-id="a3911-109">首先[找到支持的时区](outlookuser-supportedtimezones.md)，以确保仅设置针对用户的邮箱服务器配置的时区。</span><span class="sxs-lookup"><span data-stu-id="a3911-109">First [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

<span data-ttu-id="a3911-110">发送事件时，服务器会向所有与会者发送邀请。</span><span class="sxs-lookup"><span data-stu-id="a3911-110">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="a3911-111">**在事件中设置地点**</span><span class="sxs-lookup"><span data-stu-id="a3911-111">**Setting the location in an event**</span></span>

<span data-ttu-id="a3911-112">Exchange 管理员可以为资源（如会议室）或设备（如投影仪）设置邮箱和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a3911-112">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="a3911-113">然后，用户可以邀请资源作为会议与会者。</span><span class="sxs-lookup"><span data-stu-id="a3911-113">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="a3911-114">服务器代表资源根据资源的忙/闲计划接受或拒绝会议请求。</span><span class="sxs-lookup"><span data-stu-id="a3911-114">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span>
<span data-ttu-id="a3911-115">如果服务器接受资源的会议，则会在资源的日历中为会议创建一个事件。</span><span class="sxs-lookup"><span data-stu-id="a3911-115">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="a3911-116">如果重新安排会议，则服务器会自动更新资源日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="a3911-116">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="a3911-117">为资源设置邮箱的另一个优点是可以控制资源调度，例如，仅主管或其代理人可以预订私人会议室。</span><span class="sxs-lookup"><span data-stu-id="a3911-117">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="a3911-118">如果要组织涉及会议地点的事件：</span><span class="sxs-lookup"><span data-stu-id="a3911-118">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="a3911-119">相应地设置 **事件** 的 **location** 属性。</span><span class="sxs-lookup"><span data-stu-id="a3911-119">Set the **location** property of the **event** accordingly.</span></span>
2. <span data-ttu-id="a3911-120">如果会议地点具有电子邮件地址，请设置可选 **locationEmailAddress** 属性。</span><span class="sxs-lookup"><span data-stu-id="a3911-120">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="a3911-121">此外，如果会议地点已设置为资源，或者如果事件涉及某些已设置为资源的设备：</span><span class="sxs-lookup"><span data-stu-id="a3911-121">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="a3911-122">邀请该资源作为[与会者](../resources/attendee.md)。</span><span class="sxs-lookup"><span data-stu-id="a3911-122">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="a3911-123">将与会者 **type** 属性设置为 `resource`。</span><span class="sxs-lookup"><span data-stu-id="a3911-123">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="a3911-124">将与会者 **emailAddress** 设置为资源电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a3911-124">Set the attendee **emailAddress** as the resource email address.</span></span>


## <a name="permissions"></a><span data-ttu-id="a3911-125">权限</span><span class="sxs-lookup"><span data-stu-id="a3911-125">Permissions</span></span>
<span data-ttu-id="a3911-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3911-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3911-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3911-128">Permission type</span></span>      | <span data-ttu-id="a3911-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3911-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3911-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3911-130">Delegated (work or school account)</span></span> | <span data-ttu-id="a3911-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3911-131">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a3911-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3911-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3911-133">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3911-133">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a3911-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3911-134">Application</span></span> | <span data-ttu-id="a3911-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3911-135">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3911-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3911-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="a3911-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3911-137">Request headers</span></span>
| <span data-ttu-id="a3911-138">标头</span><span class="sxs-lookup"><span data-stu-id="a3911-138">Header</span></span>       | <span data-ttu-id="a3911-139">值</span><span class="sxs-lookup"><span data-stu-id="a3911-139">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="a3911-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3911-140">Authorization</span></span>  | <span data-ttu-id="a3911-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3911-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3911-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3911-143">Content-Type</span></span>  | <span data-ttu-id="a3911-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a3911-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3911-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3911-146">Request body</span></span>
<span data-ttu-id="a3911-147">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3911-147">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="a3911-148">由于 **事件** 资源支持 [扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建事件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="a3911-148">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="a3911-149">响应</span><span class="sxs-lookup"><span data-stu-id="a3911-149">Response</span></span>

<span data-ttu-id="a3911-150">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3911-150">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3911-151">示例</span><span class="sxs-lookup"><span data-stu-id="a3911-151">Examples</span></span>

### <a name="example-1-create-an-event-in-the-specified-time-zone-and-assign-the-event-an-optional-transactionid-value"></a><span data-ttu-id="a3911-152">示例 1：在指定的时区创建事件，然后为事件分配可选的 transactionId 值</span><span class="sxs-lookup"><span data-stu-id="a3911-152">Example 1: Create an event in the specified time zone, and assign the event an optional transactionId value</span></span>

#### <a name="request"></a><span data-ttu-id="a3911-153">请求</span><span class="sxs-lookup"><span data-stu-id="a3911-153">Request</span></span>
<span data-ttu-id="a3911-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3911-154">Here is an example of the request.</span></span> <span data-ttu-id="a3911-155">它使用 `Prefer: outlook.timezone` 请求头指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="a3911-155">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the start and end times in the response.</span></span> <span data-ttu-id="a3911-156">它还设置 transactionId 属性，以减少服务器上不必要的重试。</span><span class="sxs-lookup"><span data-stu-id="a3911-156">It also sets the transactionId property to reduce unnecessary retries on the server.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3911-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3911-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="a3911-158">C#</span><span class="sxs-lookup"><span data-stu-id="a3911-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3911-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3911-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3911-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3911-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3911-161">Java</span><span class="sxs-lookup"><span data-stu-id="a3911-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a3911-162">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3911-162">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="a3911-163">响应</span><span class="sxs-lookup"><span data-stu-id="a3911-163">Response</span></span>
<span data-ttu-id="a3911-164">下面是一个响应示例，显示 **start** 和 **end** 属性使用 `Prefer: outlook.timezone` 标头中指定的时区。</span><span class="sxs-lookup"><span data-stu-id="a3911-164">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="a3911-165">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3911-165">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does noon work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isDraft": false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider":"unknown",
    "onlineMeeting":null,
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```


### <a name="example-2-create-an-event-that-occurs-in-multiple-locations"></a><span data-ttu-id="a3911-166">示例 2：创建发生在多个位置的事件</span><span class="sxs-lookup"><span data-stu-id="a3911-166">Example 2: Create an event that occurs in multiple locations</span></span>

#### <a name="request"></a><span data-ttu-id="a3911-167">请求</span><span class="sxs-lookup"><span data-stu-id="a3911-167">Request</span></span>
<span data-ttu-id="a3911-168">下一个示例请求指定组织者和与会者可参加会议的 3 个地点。</span><span class="sxs-lookup"><span data-stu-id="a3911-168">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="a3911-169">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3911-169">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3911-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3911-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 1390

{
  "subject": "Plan summer company picnic",
  "body": {
    "contentType": "HTML",
    "content": "Let's kick-start this event planning!"
  },
  "start": {
      "dateTime": "2017-08-30T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-08-30T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "DanaS@contoso.onmicrosoft.com",
        "name": "Dana Swope"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "AlexW@contoso.onmicrosoft.com",
        "name": "Alex Wilber"
      },
      "type": "Required"
    }
  ],
  "location": {
    "displayName": "Conf Room 3; Fourth Coffee; Home Office",
    "locationType": "Default"
  },
  "locations": [
    {
      "displayName": "Conf Room 3"
    },
    {
      "displayName": "Fourth Coffee",
      "address": {
        "street": "4567 Main St",
        "city": "Redmond",
        "state": "WA",
        "countryOrRegion": "US",
        "postalCode": "32008"
      },
      "coordinates": {
        "latitude": 47.672,
        "longitude": -102.103
      }
    },
    {
      "displayName": "Home Office"
    }
  ],
  "allowNewTimeProposals": true
}
```
# <a name="c"></a>[<span data-ttu-id="a3911-171">C#</span><span class="sxs-lookup"><span data-stu-id="a3911-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3911-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3911-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3911-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3911-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3911-174">Java</span><span class="sxs-lookup"><span data-stu-id="a3911-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3911-175">响应</span><span class="sxs-lookup"><span data-stu-id="a3911-175">Response</span></span>
<span data-ttu-id="a3911-176">以下示例响应显示指定 3 个会议地点信息的已创建事件。</span><span class="sxs-lookup"><span data-stu-id="a3911-176">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="a3911-177">由于 `Prefer: outlook.timezone="Pacific Standard Time"` 请求标头，**start** 和 **end** 属性以 PST 表示。</span><span class="sxs-lookup"><span data-stu-id="a3911-177">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="a3911-178">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3911-178">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2985

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "uid":"04000000820089190544",
  "reminderMinutesBeforeStart":15,
  "isReminderOn":true,
  "hasAttachments":false,
  "hideAttendees": false,
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isDraft": false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
  "isOnlineMeeting":true,
  "onlineMeetingProvider":"unknown",
  "onlineMeeting":null,
  "allowNewTimeProposals": true,
  "responseStatus":{
    "response":"organizer",
    "time":"0001-01-01T00:00:00Z"
  },
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "recurrence":null,
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```


### <a name="example-3-create-a-weekly-recurring-event"></a><span data-ttu-id="a3911-179">示例 3：创建每周定期事件</span><span class="sxs-lookup"><span data-stu-id="a3911-179">Example 3: Create a weekly recurring event</span></span>

#### <a name="request"></a><span data-ttu-id="a3911-180">请求</span><span class="sxs-lookup"><span data-stu-id="a3911-180">Request</span></span>
<span data-ttu-id="a3911-181">第三个示例展示了如何创建每周发生一次的定期事件。</span><span class="sxs-lookup"><span data-stu-id="a3911-181">The third example shows how to create a recurring event that occurs once a week.</span></span> <span data-ttu-id="a3911-182">事件在 2017 年 9 月 4 日至年底期间每星期一的中午 12:00 点到下午 2:00 点之间发生。</span><span class="sxs-lookup"><span data-stu-id="a3911-182">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3911-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3911-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon time work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a3911-184">C#</span><span class="sxs-lookup"><span data-stu-id="a3911-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-recurring-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3911-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3911-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-recurring-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3911-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3911-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-recurring-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3911-187">Java</span><span class="sxs-lookup"><span data-stu-id="a3911-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-recurring-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a3911-188">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3911-188">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="a3911-189">响应</span><span class="sxs-lookup"><span data-stu-id="a3911-189">Response</span></span>
<span data-ttu-id="a3911-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a3911-190">Here is an example of the response.</span></span>
<span data-ttu-id="a3911-191">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3911-191">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isDraft": false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting":true,
    "onlineMeetingProvider":"unknown",
    "onlineMeeting":null,
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T14:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar",
        "locationType":"default",
        "uniqueId":"Harry's Bar",
        "uniqueIdType":"private"
    },
    "locations":[
        {
            "displayName":"Harry's Bar",
            "locationType":"default",
            "uniqueIdType":"unknown"
        }
    ],
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    },
    "OnlineMeeting":null
}
```

### <a name="example-4-create-a-daily-recurring-event"></a><span data-ttu-id="a3911-192">示例 4：创建每日定期事件</span><span class="sxs-lookup"><span data-stu-id="a3911-192">Example 4: Create a daily recurring event</span></span>

#### <a name="request"></a><span data-ttu-id="a3911-193">请求</span><span class="sxs-lookup"><span data-stu-id="a3911-193">Request</span></span>
<span data-ttu-id="a3911-194">第四个示例展示了如何创建每日定期事件。</span><span class="sxs-lookup"><span data-stu-id="a3911-194">The fourth example shows how to create a daily recurring event.</span></span> <span data-ttu-id="a3911-195">从 2020 年 2 月 25 日起，事件每天从下午 12：00 到下午 2：00 发生两次。</span><span class="sxs-lookup"><span data-stu-id="a3911-195">The event occurs from 12:00pm to 2:00pm, every day starting February 25, 2020, for two occurrences.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_event_recurring_daily"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2020-02-25T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2020-02-25T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AlexW@contoso.OnMicrosoft.com",
        "name": "Alex Wilbur"
      },
      "type": "required"
    }
  ],
  "recurrence": {
    "pattern": {
      "type": "daily",
      "interval": 1
    },
    "range": {
      "type": "numbered",
      "startDate": "2020-02-25",
      "numberOfOccurrences": 2
    }
  }
}
```


<span data-ttu-id="a3911-196">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3911-196">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="a3911-197">响应</span><span class="sxs-lookup"><span data-stu-id="a3911-197">Response</span></span>
<span data-ttu-id="a3911-198">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a3911-198">Here is an example of the response.</span></span>
<span data-ttu-id="a3911-199">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3911-199">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring_daily",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendar/events/$entity",
    "@odata.etag": "W/\"NDznl+Uh50WkanaCOKHkaQAAhrvLSg==\"",
    "id": "AAMkADU5NWAAA=",
    "createdDateTime": "2020-02-18T22:13:47.2967773Z",
    "lastModifiedDateTime": "2020-02-18T22:13:47.7398267Z",
    "changeKey": "NDznl+Uh50WkanaCOKHkaQAAhrvLSg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E0080000000027B6D5B0A8E6D50100000000000000001000000065CD4D206C79D44CBF53D42B6E79CE55",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "hideAttendees": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does noon work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADU5NWAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider": "unknown",
    "allowNewTimeProposals": true,
    "onlineMeeting": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes noon work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2020-02-25T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2020-02-25T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "recurrence": {
        "pattern": {
            "type": "daily",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "numbered",
            "startDate": "2020-02-25",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Pacific Standard Time",
            "numberOfOccurrences": 2
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Adele Vance",
            "address": "AdeleV@contoso.OnMicrosoft.com"
        }
    }
}
```


### <a name="example-5-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="a3911-200">示例 5：创建事件并启用为联机会议</span><span class="sxs-lookup"><span data-stu-id="a3911-200">Example 5: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="a3911-201">请求</span><span class="sxs-lookup"><span data-stu-id="a3911-201">Request</span></span>
<span data-ttu-id="a3911-202">下面是创建事件并将其启用为联机会议的请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3911-202">Here is an example of a request which creates an event and enables it as an online meeting.</span></span> <span data-ttu-id="a3911-203">它使用 `Prefer: outlook.timezone` 请求头指定响应中 **开始** 时间和 **结束** 时间的时区。</span><span class="sxs-lookup"><span data-stu-id="a3911-203">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3911-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3911-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="a3911-205">C#</span><span class="sxs-lookup"><span data-stu-id="a3911-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3911-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3911-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3911-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3911-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3911-208">Java</span><span class="sxs-lookup"><span data-stu-id="a3911-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-with-online-meeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a3911-209">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3911-209">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="a3911-210">响应</span><span class="sxs-lookup"><span data-stu-id="a3911-210">Response</span></span>
<span data-ttu-id="a3911-211">下面是一个响应示例，显示 **start** 和 **end** 属性使用 `Prefer: outlook.timezone` 标头中指定的时区。</span><span class="sxs-lookup"><span data-stu-id="a3911-211">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="a3911-212">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3911-212">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_with_online_meeting",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt8AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "uid":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does noon work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isDraft": false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+1 425 555 0123"
    }
}
```



## <a name="see-also"></a><span data-ttu-id="a3911-213">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a3911-213">See also</span></span>

- [<span data-ttu-id="a3911-214">在 Outlook 中将重复约会安排为定期事件</span><span class="sxs-lookup"><span data-stu-id="a3911-214">Schedule repeating appointments as recurring events in Outlook</span></span>](/graph/outlook-schedule-recurring-events)
- [<span data-ttu-id="a3911-215">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a3911-215">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a3911-216">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a3911-216">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a3911-217">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a3911-217">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


