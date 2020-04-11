---
title: 使用 Outlook 组织和参加联机会议
description: 在 Outlook 中，会议组织者可以允许被邀请者建议备选会议时间。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6243e7d8458a7497ea2f01ad16ee67a9fc094dcb
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229512"
---
# <a name="use-outlook-to-organize-or-attend-meetings-online"></a><span data-ttu-id="9b2fd-103">使用 Outlook 组织或参加联机会议</span><span class="sxs-lookup"><span data-stu-id="9b2fd-103">Use Outlook to organize or attend meetings online</span></span>

<span data-ttu-id="9b2fd-104">在支持联机会议提供程序的机构中，管理员可以设置 Outlook 日历以支持使用这些提供程序（其中一个作为默认提供程序）的会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-104">In an organization that supports online meeting providers, administrators can set up Outlook calendars to support meetings that use these providers, with one of these providers being the default provider.</span></span> <span data-ttu-id="9b2fd-105">可以在 Outlook 中[创建](#create-and-enable-a-meeting-online)或[更新](#update-a-meeting-to-enable-it-online)[事件](/graph/api/resources/event)，并允许与会者使用支持的提供程序加入联机会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-105">You can [create](#create-and-enable-a-meeting-online) or [update](#update-a-meeting-to-enable-it-online) an [event](/graph/api/resources/event) in Outlook and allow attendees to join the meeting online using a supported provider.</span></span> <span data-ttu-id="9b2fd-106">你可以方便地[获取事件的联机会议信息](#get-information-to-join-meeting-online)\*\*\*\*，包括用于加入会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-106">You can conveniently [get the online meeting information](#get-information-to-join-meeting-online) of the **event**, including the URL to join the meeting.</span></span> 

## <a name="calendars-and-online-meeting-providers"></a><span data-ttu-id="9b2fd-107">日历和联机会议提供程序</span><span class="sxs-lookup"><span data-stu-id="9b2fd-107">Calendars and online meeting providers</span></span>

<span data-ttu-id="9b2fd-108">支持以下任何联机会议提供程序的机构可设置 Outlook 日历并支持组织联机会议：</span><span class="sxs-lookup"><span data-stu-id="9b2fd-108">An organization that supports any of the following online meeting providers can set up Outlook calendars and enable organizing meetings online:</span></span>

- <span data-ttu-id="9b2fd-109">Microsoft Teams，作为 Office 365 商业版或企业版套件的一部分获得</span><span class="sxs-lookup"><span data-stu-id="9b2fd-109">Microsoft Teams, acquired as part of an Office 365 business or enterprise suite</span></span>
- <span data-ttu-id="9b2fd-110">Skype</span><span class="sxs-lookup"><span data-stu-id="9b2fd-110">Skype</span></span>
- <span data-ttu-id="9b2fd-111">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="9b2fd-111">Skype for Business</span></span>

<span data-ttu-id="9b2fd-112">查找 **allowedOnlineMeetingProviders** 和 **defaultOnlineMeetingProvider** 属性，验证 Outlook [日历](/graph/api/resources/calendar)是否支持任何联机会议提供程序。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-112">Look for the **allowedOnlineMeetingProviders** and **defaultOnlineMeetingProvider** properties to verify if an Outlook [calendar](/graph/api/resources/calendar) supports any online meeting providers.</span></span> <span data-ttu-id="9b2fd-113">下面的示例演示登录用户的默认日历支持两个提供程序（Microsoft Teams 和 Skype for Business），并将 Microsoft Teams 用作默认的联机会议提供程序。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-113">The following example shows the signed-in user's default calendar supports two providers, Microsoft Teams and Skype for Business, and uses Microsoft Teams as the default online meeting provider.</span></span> 

### <a name="example-find-whether-a-calendar-supports-any-online-meeting-provider"></a><span data-ttu-id="9b2fd-114">示例：查找日历是否支持任何联机会议提供程序</span><span class="sxs-lookup"><span data-stu-id="9b2fd-114">Example: Find whether a calendar supports any online meeting provider</span></span>

#### <a name="request"></a><span data-ttu-id="9b2fd-115">请求</span><span class="sxs-lookup"><span data-stu-id="9b2fd-115">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b2fd-116">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b2fd-116">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_support_for_online_meeting_providers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="9b2fd-117">C#</span><span class="sxs-lookup"><span data-stu-id="9b2fd-117">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-support-for-online-meeting-providers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b2fd-118">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b2fd-118">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-support-for-online-meeting-providers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b2fd-119">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b2fd-119">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-support-for-online-meeting-providers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b2fd-120">响应</span><span class="sxs-lookup"><span data-stu-id="9b2fd-120">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "get_calendar_support_for_online_meeting_providers",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAwAGVAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "isDefaultCalendar": true,
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": false,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness",
        "skypeForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```

## <a name="create-and-enable-a-meeting-online"></a><span data-ttu-id="9b2fd-121">创建和启用联机会议</span><span class="sxs-lookup"><span data-stu-id="9b2fd-121">Create and enable a meeting online</span></span>

<span data-ttu-id="9b2fd-122">可通过将 **isOnlineMeeting** 设置为 `true`，并将 **onlineMeetingProvider** 设置为父日历所支持的提供程序之一，创建会议并允许与会者加入联机会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-122">You can create a meeting and allow attendees to join the meeting online, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the providers supported by the parent calendar.</span></span> <span data-ttu-id="9b2fd-123">下面的示例在已登录用户的默认日历中创建了一个会议，并允许与会者通过 Microsoft Teams 加入会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-123">The following example creates a meeting in the signed-in user's default calendar, and enables attendees to join the meeting via Microsoft Teams.</span></span> <span data-ttu-id="9b2fd-124">该响应包括一个带有 **onlineMeeting** 属性中指定的联机会议信息的**事件**。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-124">The response includes an **event** with online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="9b2fd-125">一旦启用联机会议，Microsoft Graph 便会在 **onlineMeeting** 中设置会议信息。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-125">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="9b2fd-126">随后，将不能更改 **onlineMeetingProvider** 属性，也不能将 **isOnlineMeeting** 设置为 `false` 以禁用联机会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-126">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-create-and-make-meeting-available-as-an-online-meeting"></a><span data-ttu-id="9b2fd-127">示例：创建会议并使会议成为联机会议</span><span class="sxs-lookup"><span data-stu-id="9b2fd-127">Example: Create and make meeting available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="9b2fd-128">请求</span><span class="sxs-lookup"><span data-stu-id="9b2fd-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b2fd-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b2fd-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_meeting_enable_online"
}-->

```http
POST https://graph.microsoft.com/beta/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Prep for customer meeting",
  "body": {
    "contentType": "HTML",
    "content": "Does this time work for you?"
  },
  "start": {
      "dateTime": "2019-11-20T13:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-11-20T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Cordova conference room"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.OnMicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="9b2fd-130">C#</span><span class="sxs-lookup"><span data-stu-id="9b2fd-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-meeting-enable-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b2fd-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b2fd-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-meeting-enable-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b2fd-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b2fd-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-meeting-enable-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b2fd-133">响应</span><span class="sxs-lookup"><span data-stu-id="9b2fd-133">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_meeting_enable_online",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUEsA==\"",
    "id": "AAMkADAAABIGYDZAAA=",
    "createdDateTime": "2019-11-15T01:55:54.8022848Z",
    "lastModifiedDateTime": "2019-11-15T01:55:56.5162924Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUEsA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E008000000006CF8FDD0579BD501000000000000000010000000A030302E234C194F90824DFA6A17FB61",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Prep for customer meeting",
    "bodyPreview": "Does this time work for you?\r\n________________________________________________________________________________\r\nJoin Microsoft Teams Meeting\r\n+1 323-555-0166   United States, Los Angeles (Toll)\r\nConference ID: 291 633 251#\r\nLocal numbers | Reset PIN | Lea",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAABIGYDZAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes this time work for you?\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n<div class=\"me-email-text\" style=\"color:#252424; font-family:'Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif\">\r\n<div style=\"margin-top:24px; margin-bottom:10px\"><a class=\"me-email-headline\" href=\"https://teams.microsoft.com/l/meetup-join/19%3ameeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d\" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:18px; font-family:'Segoe UI Semibold','Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif; text-decoration:underline; color:#6264a7\">Join\r\n Microsoft Teams Meeting</a> </div>\r\n<div>\r\n<div><a class=\"me-email-link\" href=\"tel:&#43;1 323-886-7531,,291633251# \" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:14px; text-decoration:none; color:#6264a7\">&#43;1 323-886-7531</a>\r\n<span style=\"font-size:12px\">&nbsp; United States, Los Angeles (Toll) </span></div>\r\n</div>\r\n<div style=\"margin-top:10px; margin-bottom:20px\"><span style=\"font-size:12px\">Conference ID:\r\n</span><span style=\"font-size:14px\">291 633 251# </span></div>\r\n<div style=\"margin-bottom:24px\"><a class=\"me-email-link\" target=\"_blank\" href=\"https://dialin.teams.microsoft.com/1f9a0550-737c-41bd-8c7d-4c81dc1c4070?id=291633251\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">Local\r\n numbers</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://mysettings.lync.com/pstnconferencing\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nReset PIN</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://aka.ms/JoinTeamsMeeting\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nLearn more about Teams</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://teams.microsoft.com/meetingOptions/?organizerId=64339082-ed84-4b0b-b4ab-004ae54f3747&amp;tenantId=98a79ebe-74bf-4e07-a017-7b410848cb32&amp;threadId=19_meeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj@thread.v2&amp;messageId=0&amp;language=en-US\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nMeeting options</a> </div>\r\n<div style=\"font-size:14px; margin-bottom:4px\"></div>\r\n<div style=\"font-size:12px\"></div>\r\n</div>\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-11-20T13:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-11-20T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Cordova conference room",
        "locationType": "default",
        "uniqueId": "Cordova conference room",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Cordova conference room",
            "locationType": "default",
            "uniqueId": "Cordova conference room",
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
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "291633251",
        "tollNumber": "+1 323-555-0166"
    }
}
```

## <a name="get-information-to-join-meeting-online"></a><span data-ttu-id="9b2fd-134">获取有关加入联机会议的信息</span><span class="sxs-lookup"><span data-stu-id="9b2fd-134">Get information to join meeting online</span></span>

<span data-ttu-id="9b2fd-135">与会者和组织者可以使用 \*\*isOnlineMeeting \*\*" 属性验证是否已启用[事件](/graph/api/resources/event)以进行联机参与。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-135">Attendees and organizers can use the **isOnlineMeeting** property to verify if an [event](/graph/api/resources/event) is enabled for online participation.</span></span> <span data-ttu-id="9b2fd-136">他们可以使用 **onlineMeetingProvider** 属性来确定会议提供程序，使用 **onlineMeeting** 属性获取连接信息，包括 **joinUrl**。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-136">They can use the **onlineMeetingProvider** property to determine the meeting provider, and the **onlineMeeting** property for connection information including **joinUrl**.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="9b2fd-137">使用通过**事件**的 **onlineMeeting** 属性提供的 **joinUrl** 访问 URL 以加入会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-137">Access the URL to join a meeting using **joinUrl**, available via the **onlineMeeting** property of the **event**.</span></span> <span data-ttu-id="9b2fd-138">不要使用**事件**的 **onlineMeetingUrl** 属性，因为 **onlineMeetingUrl** 即将过时。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-138">Do not use the **onlineMeetingUrl** property of the **event** because **onlineMeetingUrl** will soon be deprecated.</span></span>

### <a name="example-get-online-meeting-information"></a><span data-ttu-id="9b2fd-139">示例：获取联机会议信息</span><span class="sxs-lookup"><span data-stu-id="9b2fd-139">Example: Get online meeting information</span></span>

#### <a name="request"></a><span data-ttu-id="9b2fd-140">请求</span><span class="sxs-lookup"><span data-stu-id="9b2fd-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b2fd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b2fd-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_online_meeting_info"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGu0AABIGYDZAAA=?$select=isOnlineMeeting,onlineMeetingProvider,onlineMeeting
```
# <a name="c"></a>[<span data-ttu-id="9b2fd-142">C#</span><span class="sxs-lookup"><span data-stu-id="9b2fd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-online-meeting-info-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b2fd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b2fd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-online-meeting-info-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b2fd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b2fd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-online-meeting-info-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b2fd-145">响应</span><span class="sxs-lookup"><span data-stu-id="9b2fd-145">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_online_meeting_info",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(isOnlineMeeting,onlineMeetingProvider,onlineMeeting)/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUExA==\"",
    "id": "AAMkADAGu0AABIGYDZAAA=",
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "291633251",
        "tollNumber": "+1 323-555-0166"
    }
}
```


## <a name="update-a-meeting-to-enable-it-online"></a><span data-ttu-id="9b2fd-146">更新会议以使其联机</span><span class="sxs-lookup"><span data-stu-id="9b2fd-146">Update a meeting to enable it online</span></span>
<span data-ttu-id="9b2fd-147">可通过将 **isOnlineMeeting** 设置为 `true`，并将 **onlineMeetingProvider** 设置为父日历所支持的联机会议提供程序之一，更改现有**事件**并使其成为联机会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-147">You can change an existing **event** to make it available as an online meeting, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the online meeting providers supported by the parent calendar.</span></span> <span data-ttu-id="9b2fd-148">该响应包括使用 **onlineMeeting** 属性中指定的相应联机会议信息更新的**事件**。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-148">The response includes the updated **event** with the corresponding online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="9b2fd-149">一旦启用联机会议，Microsoft Graph 便会在 **onlineMeeting** 中设置会议信息。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-149">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="9b2fd-150">随后，将不能更改 **onlineMeetingProvider** 属性，也不能将 **isOnlineMeeting** 设置为 `false` 以禁用联机会议。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-150">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-update-a-meeting-to-make-it-available-as-an-online-meeting"></a><span data-ttu-id="9b2fd-151">示例：更新会议以使其成为联机会议</span><span class="sxs-lookup"><span data-stu-id="9b2fd-151">Example: Update a meeting to make it available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="9b2fd-152">请求</span><span class="sxs-lookup"><span data-stu-id="9b2fd-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b2fd-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b2fd-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_meeting_online"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/events/AAMkADAGu0AABIGYDaAAA=

{
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="9b2fd-154">C#</span><span class="sxs-lookup"><span data-stu-id="9b2fd-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-meeting-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b2fd-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b2fd-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-meeting-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b2fd-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b2fd-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-meeting-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b2fd-157">响应</span><span class="sxs-lookup"><span data-stu-id="9b2fd-157">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "update_meeting_online",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUFEA==\"",
    "id": "AAMkADAGu0AABIGYDaAAA=",
    "createdDateTime": "2019-11-15T02:13:38.5558455Z",
    "lastModifiedDateTime": "2019-11-15T02:15:00.0654529Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUFEA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000CD93094B5A9BD501000000000000000010000000A16AF77C6F6C254EA13F69C3B2808B4A",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Price strategy",
    "bodyPreview": "Let's define our strategy.\r\n________________________________________________________________________________\r\nJoin Microsoft Teams Meeting\r\n+1 323-555-0166   United States, Los Angeles (Toll)\r\nConference ID: 275 984 951#\r\nLocal numbers | Reset PIN | Learn",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAGu0AABIGYDaAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\n<div>Let's define our strategy.</div>\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n<div class=\"me-email-text\" style=\"color:#252424; font-family:'Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif\">\r\n<div style=\"margin-top:24px; margin-bottom:10px\"><a class=\"me-email-headline\" href=\"https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d\" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:18px; font-family:'Segoe UI Semibold','Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif; text-decoration:underline; color:#6264a7\">Join\r\n Microsoft Teams Meeting</a> </div>\r\n<div>\r\n<div><a class=\"me-email-link\" href=\"tel:&#43;1 323-886-7531,,275984951# \" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:14px; text-decoration:none; color:#6264a7\">&#43;1 323-886-7531</a>\r\n<span style=\"font-size:12px\">&nbsp; United States, Los Angeles (Toll) </span></div>\r\n</div>\r\n<div style=\"margin-top:10px; margin-bottom:20px\"><span style=\"font-size:12px\">Conference ID:\r\n</span><span style=\"font-size:14px\">275 984 951# </span></div>\r\n<div style=\"margin-bottom:24px\"><a class=\"me-email-link\" target=\"_blank\" href=\"https://dialin.teams.microsoft.com/1f9a0550-737c-41bd-8c7d-4c81dc1c4070?id=275984951\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">Local\r\n numbers</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://mysettings.lync.com/pstnconferencing\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nReset PIN</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://aka.ms/JoinTeamsMeeting\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nLearn more about Teams</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://teams.microsoft.com/meetingOptions/?organizerId=64339082-ed84-4b0b-b4ab-004ae54f3747&amp;tenantId=98a79ebe-74bf-4e07-a017-7b410848cb32&amp;threadId=19_meeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi@thread.v2&amp;messageId=0&amp;language=en-US\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nMeeting options</a> </div>\r\n<div style=\"font-size:14px; margin-bottom:4px\"></div>\r\n<div style=\"font-size:12px\"></div>\r\n</div>\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-11-18T23:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-11-19T00:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Conf Room Baker",
        "locationUri": "Baker@contoso.onmicrosoft.com",
        "locationType": "conferenceRoom",
        "uniqueId": "Baker@contoso.onmicrosoft.com",
        "uniqueIdType": "directory",
        "address": {
            "type": "unknown",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {}
    },
    "locations": [
        {
            "displayName": "Conf Room Baker",
            "locationUri": "Baker@contoso.onmicrosoft.com",
            "locationType": "conferenceRoom",
            "uniqueId": "Baker@contoso.onmicrosoft.com",
            "uniqueIdType": "directory",
            "address": {
                "type": "unknown",
                "street": "",
                "city": "",
                "state": "",
                "countryOrRegion": "",
                "postalCode": ""
            },
            "coordinates": {}
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
        },
        {
            "type": "resource",
            "status": {
                "response": "accepted",
                "time": "2019-11-15T02:13:42.6568849Z"
            },
            "emailAddress": {
                "name": "Conf Room Baker",
                "address": "Baker@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "275984951",
        "tollNumber": "+1 323-555-0166"
    }
}
```



## <a name="see-also"></a><span data-ttu-id="9b2fd-158">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9b2fd-158">See also</span></span>
- <span data-ttu-id="9b2fd-159">有关 Microsoft Teams 与 Office 365 的互操作性的详细信息，请参阅[共存和升级设置](https://docs.microsoft.com/microsoftteams/setting-your-coexistence-and-upgrade-settings)。</span><span class="sxs-lookup"><span data-stu-id="9b2fd-159">For information on Microsoft Teams interoperability with Office 365, see [coexistence and upgrade settings](https://docs.microsoft.com/microsoftteams/setting-your-coexistence-and-upgrade-settings).</span></span>
- [<span data-ttu-id="9b2fd-160">在 Outlook 日历中查找可能会议时间</span><span class="sxs-lookup"><span data-stu-id="9b2fd-160">Finding possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
- [<span data-ttu-id="9b2fd-161">获取用户和资源的忙/闲日程安排</span><span class="sxs-lookup"><span data-stu-id="9b2fd-161">Getting the free/busy schedule for users and resources</span></span>](outlook-get-free-busy-schedule.md)
- [<span data-ttu-id="9b2fd-162">在 Outlook 日历中建议会议时间（预览）</span><span class="sxs-lookup"><span data-stu-id="9b2fd-162">Propose meeting times in an Outlook calendar (preview)</span></span>](outlook-calendar-meeting-proposals.md)
- [<span data-ttu-id="9b2fd-163">在 Outlook 中将重复约会安排为定期事件</span><span class="sxs-lookup"><span data-stu-id="9b2fd-163">Scheduling repeating appointments as recurring events in Outlook</span></span>](outlook-schedule-recurring-events.md)
