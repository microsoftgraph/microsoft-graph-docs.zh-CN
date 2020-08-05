---
title: 在 Outlook 日历中将事件启用为联机会议
description: 在支持联机会议提供程序的机构中，管理员可以设置 Outlook 日历以支持使用这些提供程序的会议。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 03c628cd87ef9a6905898fdbc11dded437f4b8cc
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567423"
---
# <a name="enable-an-event-as-an-online-meeting-in-an-outlook-calendar"></a><span data-ttu-id="97e82-103">在 Outlook 日历中将事件启用为联机会议</span><span class="sxs-lookup"><span data-stu-id="97e82-103">Enable an event as an online meeting in an Outlook calendar</span></span> 

<span data-ttu-id="97e82-104">使用 Outlook 日历 API 组织事件，会议受邀者可在其中单击加入 URL，并在 Microsoft Teams 或 Skype 中参加联机会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-104">Use the Outlook calendar API to organize an event where meeting invitees can click a join URL, and attend the meeting online in Microsoft Teams or Skype.</span></span>

<span data-ttu-id="97e82-105">在支持联机会议提供程序的机构中，管理员可以设置 Outlook 日历以支持使用这些提供程序（其中一个作为默认提供程序）的会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-105">In an organization that supports online meeting providers, administrators can set up Outlook calendars to support meetings that use these providers, with one of these providers being the default provider.</span></span> <span data-ttu-id="97e82-106">可以在 Outlook 中[创建](#create-and-enable-a-meeting-online)或[更新](#update-a-meeting-to-enable-it-online)[事件](/graph/api/resources/event)，并允许与会者使用支持的提供程序加入联机会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-106">You can [create](#create-and-enable-a-meeting-online) or [update](#update-a-meeting-to-enable-it-online) an [event](/graph/api/resources/event) in Outlook and allow attendees to join the meeting online using a supported provider.</span></span> <span data-ttu-id="97e82-107">你可以方便地[获取事件的联机会议信息](#get-information-to-join-meeting-online)\*\*\*\*，包括用于加入会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="97e82-107">You can conveniently [get the online meeting information](#get-information-to-join-meeting-online) of the **event**, including the URL to join the meeting.</span></span> 

> <span data-ttu-id="97e82-108">**注意** 日历 API 可让你方便地在 Outlook 日历中设置一个联机会议，与会者可在该日历中单击加入会议，并在 Teams 或 Skype 中继续其体验。</span><span class="sxs-lookup"><span data-stu-id="97e82-108">**Note** The calendar API lets you conveniently set up an online meeting in an Outlook calendar where attendees can click to join the meeting and continue their experience in Teams or Skype.</span></span> <span data-ttu-id="97e82-109">若要与 Teams 或 Skype 进行更具个性化、更丰富的集成，请使用云通信 API。</span><span class="sxs-lookup"><span data-stu-id="97e82-109">For a more customized, richer integration with Teams or Skype, use the cloud communications API.</span></span> <span data-ttu-id="97e82-110">有关详细信息，请参阅[在 Microsoft Graph 中选择 API 以创建和加入联机会议](choose-online-meeting-api.md)。</span><span class="sxs-lookup"><span data-stu-id="97e82-110">See [Choose an API in Microsoft Graph to create and join online meetings](choose-online-meeting-api.md) for more information.</span></span>

## <a name="calendars-and-online-meeting-providers"></a><span data-ttu-id="97e82-111">日历和联机会议提供程序</span><span class="sxs-lookup"><span data-stu-id="97e82-111">Calendars and online meeting providers</span></span>

<span data-ttu-id="97e82-112">支持以下任何联机会议提供程序的机构可设置 Outlook 日历并支持组织联机会议：</span><span class="sxs-lookup"><span data-stu-id="97e82-112">An organization that supports any of the following online meeting providers can set up Outlook calendars and enable organizing meetings online:</span></span>

- <span data-ttu-id="97e82-113">Microsoft Teams，作为 Microsoft 365 商业版或企业版套件的一部分获得</span><span class="sxs-lookup"><span data-stu-id="97e82-113">Microsoft Teams, acquired as part of a Microsoft 365 business or enterprise suite</span></span>
- <span data-ttu-id="97e82-114">Skype</span><span class="sxs-lookup"><span data-stu-id="97e82-114">Skype</span></span>
- <span data-ttu-id="97e82-115">Skype for Business（将被 [Microsoft Teams 取代](https://www.microsoft.com/microsoft-365/previous-versions/skype-for-business-online)）</span><span class="sxs-lookup"><span data-stu-id="97e82-115">Skype for Business (which is being [superceded by Microsoft Teams](https://www.microsoft.com/microsoft-365/previous-versions/skype-for-business-online))</span></span>

<span data-ttu-id="97e82-116">查找 **allowedOnlineMeetingProviders** 和 **defaultOnlineMeetingProvider** 属性，验证 Outlook [日历](/graph/api/resources/calendar)是否支持任何联机会议提供程序。</span><span class="sxs-lookup"><span data-stu-id="97e82-116">Look for the **allowedOnlineMeetingProviders** and **defaultOnlineMeetingProvider** properties to verify if an Outlook [calendar](/graph/api/resources/calendar) supports any online meeting providers.</span></span> <span data-ttu-id="97e82-117">下面的示例演示登录用户的默认日历支持两个提供程序（Microsoft Teams 和 Skype for Business），并将 Microsoft Teams 用作默认的联机会议提供程序。</span><span class="sxs-lookup"><span data-stu-id="97e82-117">The following example shows the signed-in user's default calendar supports two providers, Microsoft Teams and Skype for Business, and uses Microsoft Teams as the default online meeting provider.</span></span> 

### <a name="example-find-whether-a-calendar-supports-any-online-meeting-provider"></a><span data-ttu-id="97e82-118">示例：查找日历是否支持任何联机会议提供程序</span><span class="sxs-lookup"><span data-stu-id="97e82-118">Example: Find whether a calendar supports any online meeting provider</span></span>

#### <a name="request"></a><span data-ttu-id="97e82-119">请求</span><span class="sxs-lookup"><span data-stu-id="97e82-119">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97e82-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e82-120">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_support_for_online_meeting_providers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="97e82-121">C#</span><span class="sxs-lookup"><span data-stu-id="97e82-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-support-for-online-meeting-providers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97e82-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97e82-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-support-for-online-meeting-providers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97e82-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97e82-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-support-for-online-meeting-providers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97e82-124">Java</span><span class="sxs-lookup"><span data-stu-id="97e82-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-support-for-online-meeting-providers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97e82-125">响应</span><span class="sxs-lookup"><span data-stu-id="97e82-125">Response</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAwAGVAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
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

## <a name="create-and-enable-a-meeting-online"></a><span data-ttu-id="97e82-126">创建和启用联机会议</span><span class="sxs-lookup"><span data-stu-id="97e82-126">Create and enable a meeting online</span></span>

<span data-ttu-id="97e82-127">可通过将 **isOnlineMeeting** 设置为 `true`，并将 **onlineMeetingProvider** 设置为父日历所支持的提供程序之一，创建会议并允许与会者加入联机会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-127">You can create a meeting and allow attendees to join the meeting online, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the providers supported by the parent calendar.</span></span> <span data-ttu-id="97e82-128">下面的示例在已登录用户的默认日历中创建了一个会议，并允许与会者通过 Microsoft Teams 加入会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-128">The following example creates a meeting in the signed-in user's default calendar, and enables attendees to join the meeting via Microsoft Teams.</span></span> <span data-ttu-id="97e82-129">该响应包括一个带有 **onlineMeeting** 属性中指定的联机会议信息的**事件**。</span><span class="sxs-lookup"><span data-stu-id="97e82-129">The response includes an **event** with online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="97e82-130">一旦启用联机会议，Microsoft Graph 便会在 **onlineMeeting** 中设置会议信息。</span><span class="sxs-lookup"><span data-stu-id="97e82-130">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="97e82-131">随后，将不能更改 **onlineMeetingProvider** 属性，也不能将 **isOnlineMeeting** 设置为 `false` 以禁用联机会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-131">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-create-and-make-meeting-available-as-an-online-meeting"></a><span data-ttu-id="97e82-132">示例：创建会议并使会议成为联机会议</span><span class="sxs-lookup"><span data-stu-id="97e82-132">Example: Create and make meeting available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="97e82-133">请求</span><span class="sxs-lookup"><span data-stu-id="97e82-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97e82-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e82-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_meeting_enable_online"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events
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
# <a name="c"></a>[<span data-ttu-id="97e82-135">C#</span><span class="sxs-lookup"><span data-stu-id="97e82-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-meeting-enable-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97e82-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97e82-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-meeting-enable-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97e82-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97e82-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-meeting-enable-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97e82-138">Java</span><span class="sxs-lookup"><span data-stu-id="97e82-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-meeting-enable-online-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97e82-139">响应</span><span class="sxs-lookup"><span data-stu-id="97e82-139">Response</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUEsA==\"",
    "id": "AAMkADAAABIGYDZAAA=",
    "createdDateTime": "2019-11-15T01:55:54.8022848Z",
    "lastModifiedDateTime": "2019-11-15T01:55:56.5162924Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUEsA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E0080000000076B29D94B32CD6010000000000000000100000005F31C591C3C328459653D025BD277439",
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

## <a name="get-information-to-join-meeting-online"></a><span data-ttu-id="97e82-140">获取有关加入联机会议的信息</span><span class="sxs-lookup"><span data-stu-id="97e82-140">Get information to join meeting online</span></span>

<span data-ttu-id="97e82-141">与会者和组织者可以使用 \*\*isOnlineMeeting \*\*" 属性验证是否已启用[事件](/graph/api/resources/event)以进行联机参与。</span><span class="sxs-lookup"><span data-stu-id="97e82-141">Attendees and organizers can use the **isOnlineMeeting** property to verify if an [event](/graph/api/resources/event) is enabled for online participation.</span></span> <span data-ttu-id="97e82-142">他们可以使用 **onlineMeetingProvider** 属性来确定会议提供程序，使用 **onlineMeeting** 属性获取连接信息，包括 **joinUrl**。</span><span class="sxs-lookup"><span data-stu-id="97e82-142">They can use the **onlineMeetingProvider** property to determine the meeting provider, and the **onlineMeeting** property for connection information including **joinUrl**.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="97e82-143">使用通过**事件**的 **onlineMeeting** 属性提供的 **joinUrl** 访问 URL 以加入会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-143">Access the URL to join a meeting using **joinUrl**, available via the **onlineMeeting** property of the **event**.</span></span> <span data-ttu-id="97e82-144">不要使用**事件**的 **onlineMeetingUrl** 属性，因为 **onlineMeetingUrl** 即将过时。</span><span class="sxs-lookup"><span data-stu-id="97e82-144">Do not use the **onlineMeetingUrl** property of the **event** because **onlineMeetingUrl** will soon be deprecated.</span></span>

### <a name="example-get-online-meeting-information"></a><span data-ttu-id="97e82-145">示例：获取联机会议信息</span><span class="sxs-lookup"><span data-stu-id="97e82-145">Example: Get online meeting information</span></span>

#### <a name="request"></a><span data-ttu-id="97e82-146">请求</span><span class="sxs-lookup"><span data-stu-id="97e82-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97e82-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e82-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_online_meeting_info"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGu0AABIGYDZAAA=?$select=isOnlineMeeting,onlineMeetingProvider,onlineMeeting
```
# <a name="c"></a>[<span data-ttu-id="97e82-148">C#</span><span class="sxs-lookup"><span data-stu-id="97e82-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-online-meeting-info-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97e82-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97e82-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-online-meeting-info-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97e82-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97e82-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-online-meeting-info-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97e82-151">Java</span><span class="sxs-lookup"><span data-stu-id="97e82-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-online-meeting-info-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97e82-152">响应</span><span class="sxs-lookup"><span data-stu-id="97e82-152">Response</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(isOnlineMeeting,onlineMeetingProvider,onlineMeeting)/$entity",
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


## <a name="update-a-meeting-to-enable-it-online"></a><span data-ttu-id="97e82-153">更新会议以使其联机</span><span class="sxs-lookup"><span data-stu-id="97e82-153">Update a meeting to enable it online</span></span>
<span data-ttu-id="97e82-154">可通过将 **isOnlineMeeting** 设置为 `true`，并将 **onlineMeetingProvider** 设置为父日历所支持的联机会议提供程序之一，更改现有**事件**并使其成为联机会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-154">You can change an existing **event** to make it available as an online meeting, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the online meeting providers supported by the parent calendar.</span></span> <span data-ttu-id="97e82-155">该响应包括使用 **onlineMeeting** 属性中指定的相应联机会议信息更新的**事件**。</span><span class="sxs-lookup"><span data-stu-id="97e82-155">The response includes the updated **event** with the corresponding online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="97e82-156">一旦启用联机会议，Microsoft Graph 便会在 **onlineMeeting** 中设置会议信息。</span><span class="sxs-lookup"><span data-stu-id="97e82-156">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="97e82-157">随后，将不能更改 **onlineMeetingProvider** 属性，也不能将 **isOnlineMeeting** 设置为 `false` 以禁用联机会议。</span><span class="sxs-lookup"><span data-stu-id="97e82-157">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-update-a-meeting-to-make-it-available-as-an-online-meeting"></a><span data-ttu-id="97e82-158">示例：更新会议以使其成为联机会议</span><span class="sxs-lookup"><span data-stu-id="97e82-158">Example: Update a meeting to make it available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="97e82-159">请求</span><span class="sxs-lookup"><span data-stu-id="97e82-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97e82-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e82-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_meeting_online"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/events/AAMkADAGu0AABIGYDaAAA=

{
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="97e82-161">C#</span><span class="sxs-lookup"><span data-stu-id="97e82-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-meeting-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97e82-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97e82-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-meeting-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97e82-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97e82-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-meeting-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97e82-164">Java</span><span class="sxs-lookup"><span data-stu-id="97e82-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-meeting-online-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97e82-165">响应</span><span class="sxs-lookup"><span data-stu-id="97e82-165">Response</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUFEA==\"",
    "id": "AAMkADAGu0AABIGYDaAAA=",
    "createdDateTime": "2019-11-15T02:13:38.5558455Z",
    "lastModifiedDateTime": "2019-11-15T02:15:00.0654529Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUFEA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000CD93094B5A9BD501000000000000000010000000A16AF77C6F6C254EA13F69C3B2808B4A",
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
        "locationType": "conferenceRoom",
        "uniqueId": "Baker@contoso.onmicrosoft.com",
        "uniqueIdType": "directory"
    },
    "locations": [
        {
            "displayName": "Conf Room Baker",
            "locationType": "conferenceRoom",
            "uniqueId": "Baker@contoso.onmicrosoft.com",
            "uniqueIdType": "directory"
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
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "275984951",
        "tollNumber": "+1 323-555-0166"
    }
}
```



## <a name="see-also"></a><span data-ttu-id="97e82-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="97e82-166">See also</span></span>
- <span data-ttu-id="97e82-167">有关 Microsoft Teams 与 Microsoft 365 互操作性的信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="97e82-167">For information on Microsoft Teams interoperability with Microsoft 365, see:</span></span>
  - [<span data-ttu-id="97e82-168">Exchange 与 Microsoft Teams 如何交互</span><span class="sxs-lookup"><span data-stu-id="97e82-168">How Exchange and Microsoft Teams interact</span></span>](/microsoftteams/exchange-teams-interact)
  - [<span data-ttu-id="97e82-169">设置共存和升级设置</span><span class="sxs-lookup"><span data-stu-id="97e82-169">Setting your coexistence and upgrade settings</span></span>](/microsoftteams/setting-your-coexistence-and-upgrade-settings)
- [<span data-ttu-id="97e82-170">在 Microsoft Graph 中选择 API 以创建和加入联机会议</span><span class="sxs-lookup"><span data-stu-id="97e82-170">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)
- [<span data-ttu-id="97e82-171">在 Outlook 日历中查找可能会议时间</span><span class="sxs-lookup"><span data-stu-id="97e82-171">Finding possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
- [<span data-ttu-id="97e82-172">获取用户和资源的忙/闲日程安排</span><span class="sxs-lookup"><span data-stu-id="97e82-172">Getting the free/busy schedule for users and resources</span></span>](outlook-get-free-busy-schedule.md)
- [<span data-ttu-id="97e82-173">在 Outlook 日历中建议会议时间（预览）</span><span class="sxs-lookup"><span data-stu-id="97e82-173">Propose meeting times in an Outlook calendar (preview)</span></span>](outlook-calendar-meeting-proposals.md)
- [<span data-ttu-id="97e82-174">在 Outlook 中将重复约会安排为定期事件</span><span class="sxs-lookup"><span data-stu-id="97e82-174">Scheduling repeating appointments as recurring events in Outlook</span></span>](outlook-schedule-recurring-events.md)
