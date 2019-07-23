---
title: 创建事件
description: 在用户的默认日历或指定日历中创建事件。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: fe9864474a83a827430b539d80127441b548ecb1
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805093"
---
# <a name="create-event"></a><span data-ttu-id="b2ca8-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="b2ca8-103">Create Event</span></span>

<span data-ttu-id="b2ca8-104">在用户的默认日历或指定日历中创建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-104">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="b2ca8-105">可以将事件的各开始和结束时间的时区指定为其值的一部分，因为**开始**和**结束**属性为 [dateTimeTimeZone](../resources/datetimetimezone.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-105">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> <span data-ttu-id="b2ca8-106">首先[找到支持的时区](outlookuser-supportedtimezones.md)，以确保仅设置针对用户的邮箱服务器配置的时区。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-106">First [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

<span data-ttu-id="b2ca8-107">发送事件时，服务器会向所有与会者发送邀请。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-107">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="b2ca8-108">**在事件中设置地点**</span><span class="sxs-lookup"><span data-stu-id="b2ca8-108">**Setting the location in an event**</span></span>

<span data-ttu-id="b2ca8-109">Exchange 管理员可以为资源（如会议室）或设备（如投影仪）设置邮箱和电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-109">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="b2ca8-110">然后，用户可以邀请资源作为会议与会者。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-110">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="b2ca8-111">服务器代表资源根据资源的忙/闲计划接受或拒绝会议请求。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-111">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="b2ca8-112">如果服务器接受资源的会议，则会在资源的日历中为会议创建一个事件。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-112">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="b2ca8-113">如果重新安排会议，则服务器会自动更新资源日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-113">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="b2ca8-114">为资源设置邮箱的另一个优点是可以控制资源调度，例如，仅主管或其代理人可以预订私人会议室。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-114">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="b2ca8-115">如果要组织涉及会议地点的事件：</span><span class="sxs-lookup"><span data-stu-id="b2ca8-115">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="b2ca8-116">相应地设置**事件**的 **location** 属性。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-116">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="b2ca8-117">如果会议地点具有电子邮件地址，请设置可选 **locationEmailAddress** 属性。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-117">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="b2ca8-118">此外，如果会议地点已设置为资源，或者如果事件涉及某些已设置为资源的设备：</span><span class="sxs-lookup"><span data-stu-id="b2ca8-118">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="b2ca8-119">邀请该资源作为[与会者](../resources/attendee.md)。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-119">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="b2ca8-120">将与会者 **type** 属性设置为 `resource`。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-120">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="b2ca8-121">将与会者 **emailAddress** 设置为资源电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-121">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="b2ca8-122">权限</span><span class="sxs-lookup"><span data-stu-id="b2ca8-122">Permissions</span></span>
<span data-ttu-id="b2ca8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2ca8-125">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2ca8-125">Permission type</span></span>      | <span data-ttu-id="b2ca8-126">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2ca8-126">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2ca8-127">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2ca8-127">Delegated (work or school account)</span></span> | <span data-ttu-id="b2ca8-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2ca8-128">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b2ca8-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2ca8-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2ca8-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2ca8-130">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b2ca8-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2ca8-131">Application</span></span> | <span data-ttu-id="b2ca8-132">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2ca8-132">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2ca8-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2ca8-133">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="b2ca8-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2ca8-134">Request headers</span></span>
| <span data-ttu-id="b2ca8-135">标头</span><span class="sxs-lookup"><span data-stu-id="b2ca8-135">Header</span></span>       | <span data-ttu-id="b2ca8-136">值</span><span class="sxs-lookup"><span data-stu-id="b2ca8-136">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="b2ca8-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2ca8-137">Authorization</span></span>  | <span data-ttu-id="b2ca8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b2ca8-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2ca8-140">Content-Type</span></span>  | <span data-ttu-id="b2ca8-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b2ca8-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2ca8-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2ca8-143">Request body</span></span>
<span data-ttu-id="b2ca8-144">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-144">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="b2ca8-145">由于**事件**资源支持[扩展](/graph/extensibility-overview)因此可以使用 `POST` 操作，并在创建事件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-145">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="b2ca8-146">响应</span><span class="sxs-lookup"><span data-stu-id="b2ca8-146">Response</span></span>

<span data-ttu-id="b2ca8-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-147">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2ca8-148">示例</span><span class="sxs-lookup"><span data-stu-id="b2ca8-148">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b2ca8-149">请求 1</span><span class="sxs-lookup"><span data-stu-id="b2ca8-149">Request 1</span></span>
<span data-ttu-id="b2ca8-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-150">Here is an example of the request.</span></span> <span data-ttu-id="b2ca8-151">它使用 `Prefer: outlook.timezone` 请求头指定响应中**开始**时间和**结束**时间的时区。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-151">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2ca8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2ca8-152">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2ca8-153">C#</span><span class="sxs-lookup"><span data-stu-id="b2ca8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2ca8-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="b2ca8-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2ca8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2ca8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b2ca8-156">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-156">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="b2ca8-157">响应 1</span><span class="sxs-lookup"><span data-stu-id="b2ca8-157">Response 1</span></span>
<span data-ttu-id="b2ca8-158">下面是一个响应示例，显示 **start** 和 **end** 属性使用 `Prefer: outlook.timezone` 标头中指定的时区。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-158">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="b2ca8-159">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2ca8-160">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-160">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
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


##### <a name="request-2"></a><span data-ttu-id="b2ca8-161">请求 2</span><span class="sxs-lookup"><span data-stu-id="b2ca8-161">Request 2</span></span>
<span data-ttu-id="b2ca8-162">下一个示例请求指定组织者和与会者可参加会议的 3 个地点。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-162">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="b2ca8-163">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-163">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2ca8-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2ca8-164">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2ca8-165">C#</span><span class="sxs-lookup"><span data-stu-id="b2ca8-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2ca8-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="b2ca8-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2ca8-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2ca8-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="b2ca8-168">响应 2</span><span class="sxs-lookup"><span data-stu-id="b2ca8-168">Response 2</span></span>
<span data-ttu-id="b2ca8-169">以下示例响应显示指定 3 个会议地点信息的已创建事件。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-169">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="b2ca8-170">由于 `Prefer: outlook.timezone="Pacific Standard Time"` 请求标头，**start** 和 **end** 属性以 PST 表示。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-170">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="b2ca8-171">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-171">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2ca8-172">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-172">All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "iCalUId":"04000000820089190544",
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


##### <a name="request-3"></a><span data-ttu-id="b2ca8-173">请求 3</span><span class="sxs-lookup"><span data-stu-id="b2ca8-173">Request 3</span></span>
<span data-ttu-id="b2ca8-174">第三个示例展示了如何创建定期事件。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-174">The third example shows how to create a recurring event.</span></span> <span data-ttu-id="b2ca8-175">事件在 2017 年 9 月 4 日至年底期间每星期一的中午 12:00 点到下午 2:00 点之间发生。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-175">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2ca8-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2ca8-176">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2ca8-177">C#</span><span class="sxs-lookup"><span data-stu-id="b2ca8-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-recurring-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2ca8-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="b2ca8-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-recurring-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2ca8-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2ca8-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-recurring-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b2ca8-180">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-180">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="b2ca8-181">响应 3</span><span class="sxs-lookup"><span data-stu-id="b2ca8-181">Response 3</span></span>
<span data-ttu-id="b2ca8-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2ca8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
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


## <a name="see-also"></a><span data-ttu-id="b2ca8-185">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b2ca8-185">See also</span></span>

- [<span data-ttu-id="b2ca8-186">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b2ca8-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b2ca8-187">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b2ca8-187">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b2ca8-188">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b2ca8-188">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
