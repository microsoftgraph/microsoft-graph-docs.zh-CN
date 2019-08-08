---
title: 创建事件
description: 使用此 API 在默认或指定的日历中创建新事件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5fa92f7657c69871af2f2661cde00b17d9499886
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245552"
---
# <a name="create-event"></a><span data-ttu-id="de156-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="de156-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de156-104">使用此 API 在日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="de156-104">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="de156-105">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="de156-105">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="de156-106">权限</span><span class="sxs-lookup"><span data-stu-id="de156-106">Permissions</span></span>
<span data-ttu-id="de156-107">根据在其中创建事件的日历类型以及请求的权限类型 (委派或应用程序), 需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="de156-107">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="de156-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de156-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de156-109">日历</span><span class="sxs-lookup"><span data-stu-id="de156-109">Calendar</span></span> | <span data-ttu-id="de156-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de156-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de156-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de156-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de156-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="de156-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="de156-113">用户日历</span><span class="sxs-lookup"><span data-stu-id="de156-113">user calendar</span></span> | <span data-ttu-id="de156-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de156-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="de156-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de156-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="de156-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de156-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="de156-117">组 日历</span><span class="sxs-lookup"><span data-stu-id="de156-117">group calendar</span></span> | <span data-ttu-id="de156-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de156-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="de156-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="de156-119">Not supported.</span></span> | <span data-ttu-id="de156-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="de156-120">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="de156-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de156-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="de156-122">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="de156-122">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="de156-123">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="de156-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="de156-124">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="de156-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="de156-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="de156-125">Request headers</span></span>
| <span data-ttu-id="de156-126">标头</span><span class="sxs-lookup"><span data-stu-id="de156-126">Header</span></span>       | <span data-ttu-id="de156-127">值</span><span class="sxs-lookup"><span data-stu-id="de156-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de156-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="de156-128">Authorization</span></span>  | <span data-ttu-id="de156-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de156-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de156-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de156-131">Content-Type</span></span>  | <span data-ttu-id="de156-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="de156-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de156-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="de156-134">Request body</span></span>
<span data-ttu-id="de156-135">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de156-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de156-136">响应</span><span class="sxs-lookup"><span data-stu-id="de156-136">Response</span></span>

<span data-ttu-id="de156-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de156-137">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de156-138">示例</span><span class="sxs-lookup"><span data-stu-id="de156-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de156-139">请求</span><span class="sxs-lookup"><span data-stu-id="de156-139">Request</span></span>
<span data-ttu-id="de156-140">下面的示例在已登录用户的指定日历中创建事件。</span><span class="sxs-lookup"><span data-stu-id="de156-140">The following example creates an event in the specified calendar of the signed-in user's.</span></span>

<span data-ttu-id="de156-141">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de156-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de156-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="de156-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="de156-143">C#</span><span class="sxs-lookup"><span data-stu-id="de156-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de156-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="de156-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de156-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="de156-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="de156-146">Java</span><span class="sxs-lookup"><span data-stu-id="de156-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de156-147">响应</span><span class="sxs-lookup"><span data-stu-id="de156-147">Response</span></span>
<span data-ttu-id="de156-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de156-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
