---
title: 创建事件
description: 在用户的默认日历或指定日历中创建事件。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bffe5bce27d8aa896d5f75550c1ce24f830797aa
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601473"
---
# <a name="create-event"></a><span data-ttu-id="b1cc1-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="b1cc1-103">Create Event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1cc1-104">在用户的默认日历或指定日历中创建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-104">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="b1cc1-105">可以将事件的各开始和结束时间的时区指定为这些值的一部分，因为**开始**和**结束**属性为 [dateTimeTimeZone](../resources/datetimetimezone.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-105">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span>

<span data-ttu-id="b1cc1-106">发送事件时，服务器会向所有与会者发送邀请。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-106">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="b1cc1-107">**在事件中设置地点**</span><span class="sxs-lookup"><span data-stu-id="b1cc1-107">**Setting the location in an event**</span></span>

<span data-ttu-id="b1cc1-108">Exchange 管理员可以为资源（如会议室）或设备（如投影仪）设置邮箱和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-108">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="b1cc1-109">然后，用户可以邀请资源作为会议与会者。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-109">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="b1cc1-110">服务器代表资源根据资源的忙/闲计划接受或拒绝会议请求。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-110">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span>
<span data-ttu-id="b1cc1-111">如果服务器接受资源的会议，则会在资源的日历中为会议创建一个事件。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-111">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="b1cc1-112">如果重新安排会议，则服务器会自动更新资源日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-112">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="b1cc1-113">为资源设置邮箱的另一个优点是可以控制资源调度，例如，仅主管或其代理人可以预订私人会议室。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-113">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="b1cc1-114">如果要组织涉及会议地点的事件：</span><span class="sxs-lookup"><span data-stu-id="b1cc1-114">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="b1cc1-115">相应地设置**事件**的 **location** 属性。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-115">Set the **location** property of the **event** accordingly.</span></span>
2. <span data-ttu-id="b1cc1-116">如果会议地点具有电子邮件地址，请设置可选 **locationEmailAddress** 属性。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-116">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="b1cc1-117">此外，如果会议地点已设置为资源，或者如果事件涉及某些已设置为资源的设备：</span><span class="sxs-lookup"><span data-stu-id="b1cc1-117">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="b1cc1-118">邀请该资源作为[与会者](../resources/attendee.md)。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-118">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="b1cc1-119">将与会者 **type** 属性设置为 `resource`。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-119">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="b1cc1-120">将与会者 **emailAddress** 设置为资源电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-120">Set the attendee **emailAddress** as the resource email address.</span></span>


## <a name="permissions"></a><span data-ttu-id="b1cc1-121">权限</span><span class="sxs-lookup"><span data-stu-id="b1cc1-121">Permissions</span></span>
<span data-ttu-id="b1cc1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1cc1-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1cc1-124">Permission type</span></span>      | <span data-ttu-id="b1cc1-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1cc1-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1cc1-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1cc1-126">Delegated (work or school account)</span></span> | <span data-ttu-id="b1cc1-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1cc1-127">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b1cc1-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1cc1-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1cc1-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1cc1-129">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b1cc1-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1cc1-130">Application</span></span> | <span data-ttu-id="b1cc1-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1cc1-131">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1cc1-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1cc1-132">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="b1cc1-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1cc1-133">Request headers</span></span>
| <span data-ttu-id="b1cc1-134">标头</span><span class="sxs-lookup"><span data-stu-id="b1cc1-134">Header</span></span>       | <span data-ttu-id="b1cc1-135">值</span><span class="sxs-lookup"><span data-stu-id="b1cc1-135">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="b1cc1-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1cc1-136">Authorization</span></span>  | <span data-ttu-id="b1cc1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1cc1-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1cc1-139">Content-Type</span></span>  | <span data-ttu-id="b1cc1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b1cc1-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1cc1-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1cc1-142">Request body</span></span>
<span data-ttu-id="b1cc1-143">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-143">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="b1cc1-144">由于**事件**资源支持[扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建事件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-144">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="b1cc1-145">响应</span><span class="sxs-lookup"><span data-stu-id="b1cc1-145">Response</span></span>

<span data-ttu-id="b1cc1-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-146">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1cc1-147">示例</span><span class="sxs-lookup"><span data-stu-id="b1cc1-147">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b1cc1-148">请求 1</span><span class="sxs-lookup"><span data-stu-id="b1cc1-148">Request 1</span></span>
<span data-ttu-id="b1cc1-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-149">Here is an example of the request.</span></span> <span data-ttu-id="b1cc1-150">它使用 `Prefer: outlook.timezone` 请求头指定响应中**开始**时间和**结束**时间的时区。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-150">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
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
  ]
}
```
<span data-ttu-id="b1cc1-151">在请求正文中，提供 JSON 表示形式的 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-151">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="b1cc1-152">响应 1</span><span class="sxs-lookup"><span data-stu-id="b1cc1-152">Response 1</span></span>
<span data-ttu-id="b1cc1-153">下面是一个响应示例，显示 **start** 和 **end** 属性使用 `Prefer: outlook.timezone` 标头中指定的时区。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-153">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="b1cc1-154">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1cc1-155">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-155">All of the properties will be returned from an actual call.</span></span>
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
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1cc1-156">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b1cc1-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1cc1-157">C#</span><span class="sxs-lookup"><span data-stu-id="b1cc1-157">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1cc1-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1cc1-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_from_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="b1cc1-159">请求 2</span><span class="sxs-lookup"><span data-stu-id="b1cc1-159">Request 2</span></span>
<span data-ttu-id="b1cc1-160">下一个示例请求指定组织者和与会者可参加会议的 3 个地点。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-160">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="b1cc1-161">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-161">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
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
  ]

}
```

##### <a name="response-2"></a><span data-ttu-id="b1cc1-162">响应 2</span><span class="sxs-lookup"><span data-stu-id="b1cc1-162">Response 2</span></span>
<span data-ttu-id="b1cc1-163">以下示例响应显示指定 3 个会议地点信息的已创建事件。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-163">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="b1cc1-164">由于 `Prefer: outlook.timezone="Pacific Standard Time"` 请求标头，**start** 和 **end** 属性以 PST 表示。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-164">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="b1cc1-165">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1cc1-166">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-166">All of the properties will be returned from an actual call.</span></span>
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
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1cc1-167">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b1cc1-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1cc1-168">C#</span><span class="sxs-lookup"><span data-stu-id="b1cc1-168">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_from_user_multiple_locations-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1cc1-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1cc1-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_from_user_multiple_locations-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-3"></a><span data-ttu-id="b1cc1-170">请求 3</span><span class="sxs-lookup"><span data-stu-id="b1cc1-170">Request 3</span></span>
<span data-ttu-id="b1cc1-171">第三个示例展示了如何创建定期事件。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-171">The third example shows how to create a recurring event.</span></span> <span data-ttu-id="b1cc1-172">事件在 2017 年 9 月 4 日至年底期间每星期一的中午 12:00 点到下午 2:00 点之间发生。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-172">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>
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
<span data-ttu-id="b1cc1-173">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-173">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="b1cc1-174">响应 3</span><span class="sxs-lookup"><span data-stu-id="b1cc1-174">Response 3</span></span>
<span data-ttu-id="b1cc1-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1cc1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1cc1-178">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b1cc1-178">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1cc1-179">C#</span><span class="sxs-lookup"><span data-stu-id="b1cc1-179">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_event_recurring-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1cc1-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1cc1-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_event_recurring-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]




## <a name="see-also"></a><span data-ttu-id="b1cc1-181">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b1cc1-181">See also</span></span>

- [<span data-ttu-id="b1cc1-182">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b1cc1-182">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b1cc1-183">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b1cc1-183">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b1cc1-184">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b1cc1-184">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/user-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-post-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
