---
title: 创建事件
description: 使用此 API 在默认或指定的日历中创建新事件。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a78006e5ce1364191ed125f374ff1dc6d774ed6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518789"
---
# <a name="create-event"></a><span data-ttu-id="ca40d-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="ca40d-103">Create event</span></span>

<span data-ttu-id="ca40d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca40d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca40d-105">使用此 API 在日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="ca40d-105">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="ca40d-106">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="ca40d-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ca40d-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca40d-107">Permissions</span></span>
<span data-ttu-id="ca40d-108">根据创建事件的日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ca40d-108">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="ca40d-109">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca40d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca40d-110">日历</span><span class="sxs-lookup"><span data-stu-id="ca40d-110">Calendar</span></span> | <span data-ttu-id="ca40d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca40d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca40d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca40d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca40d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca40d-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="ca40d-114">用户日历</span><span class="sxs-lookup"><span data-stu-id="ca40d-114">user calendar</span></span> | <span data-ttu-id="ca40d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca40d-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="ca40d-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca40d-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="ca40d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca40d-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="ca40d-118">组日历</span><span class="sxs-lookup"><span data-stu-id="ca40d-118">group calendar</span></span> | <span data-ttu-id="ca40d-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca40d-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="ca40d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca40d-120">Not supported.</span></span> | <span data-ttu-id="ca40d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca40d-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca40d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca40d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ca40d-123">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ca40d-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="ca40d-124">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ca40d-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="ca40d-125">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ca40d-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="ca40d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca40d-126">Request headers</span></span>
| <span data-ttu-id="ca40d-127">标头</span><span class="sxs-lookup"><span data-stu-id="ca40d-127">Header</span></span>       | <span data-ttu-id="ca40d-128">值</span><span class="sxs-lookup"><span data-stu-id="ca40d-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca40d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca40d-129">Authorization</span></span>  | <span data-ttu-id="ca40d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca40d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ca40d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca40d-132">Content-Type</span></span>  | <span data-ttu-id="ca40d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ca40d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca40d-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca40d-135">Request body</span></span>
<span data-ttu-id="ca40d-136">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca40d-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca40d-137">响应</span><span class="sxs-lookup"><span data-stu-id="ca40d-137">Response</span></span>

<span data-ttu-id="ca40d-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca40d-138">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca40d-139">示例</span><span class="sxs-lookup"><span data-stu-id="ca40d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca40d-140">请求</span><span class="sxs-lookup"><span data-stu-id="ca40d-140">Request</span></span>
<span data-ttu-id="ca40d-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca40d-141">Here is an example of the request.</span></span>
<span data-ttu-id="ca40d-142">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca40d-142">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca40d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca40d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does mid month work for you?"
  },
  "start": {
      "dateTime": "2019-03-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ca40d-144">C#</span><span class="sxs-lookup"><span data-stu-id="ca40d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca40d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca40d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca40d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca40d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca40d-147">Java</span><span class="sxs-lookup"><span data-stu-id="ca40d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ca40d-148">响应</span><span class="sxs-lookup"><span data-stu-id="ca40d-148">Response</span></span>
<span data-ttu-id="ca40d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca40d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA=",
    "createdDateTime": "2019-02-28T21:17:57.56197Z",
    "lastModifiedDateTime": "2019-02-28T21:17:59.044919Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E641B4C",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes mid month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-15T14:00:00.0000000",
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
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
