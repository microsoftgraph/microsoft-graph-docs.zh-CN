---
title: 在共享或委托日历中创建 Outlook 事件
description: 在 Outlook 中，客户可以与其他用户共享日历，并允许其他用户查看或修改此日历中的事件。 客户还可以授权代理代表自己执行操作、接收或答复会议请求，或在日历中创建或更改项。
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e09b3552ca0d4a3ecd85855c471ec1cc16950abf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941398"
---
# <a name="create-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="3ef21-104">在共享或委托日历中创建 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="3ef21-104">Create Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="3ef21-105">在 Outlook 中，客户可以与其他用户共享日历，并让他们查看、创建或修改该日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="3ef21-105">In Outlook, customers can share a calendar with other users and let them view, create, or modify events in that calendar.</span></span> <span data-ttu-id="3ef21-106">客户还可以授权代理代表自己执行操作、接收或答复会议请求，或在日历中创建或更改项。</span><span class="sxs-lookup"><span data-stu-id="3ef21-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="3ef21-107">Microsoft Graph 支持以编程方式读取或写入其他用户已共享日历中的事件、读取共享日历以及更新共享者的日历名称。</span><span class="sxs-lookup"><span data-stu-id="3ef21-107">Programmatically, Microsoft Graph supports reading or writing events in calendars that have been shared by other users, as well as reading the shared calendars, and updating the calendar name for sharees.</span></span> <span data-ttu-id="3ef21-108">此支持还适用于已委托的日历。</span><span class="sxs-lookup"><span data-stu-id="3ef21-108">The support also applies to calendars that have been delegated.</span></span> <span data-ttu-id="3ef21-109">本文的其余部分介绍了如何在共享或委托日历中创建会议事件。</span><span class="sxs-lookup"><span data-stu-id="3ef21-109">The rest of this article walks through creating a meeting event in a shared or delegated calendar.</span></span> <span data-ttu-id="3ef21-110">有关获取事件，请参阅[获取共享日历或委托日历中的 Outlook 事件](outlook-get-shared-events-calendars.md)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-110">For getting events, refer to [Get Outlook events in a shared or delegated calendar](outlook-get-shared-events-calendars.md).</span></span>

<span data-ttu-id="3ef21-111">下面的演练使用示例方案，其中 Alex 在 Outlook 中将其主要日历委派给 Adele，并保留默认的 Outlook 邮箱设置以将会议请求和响应仅定向给委托人。</span><span class="sxs-lookup"><span data-stu-id="3ef21-111">The walkthrough below uses the example scenario where Alex has delegated his primary calendar to Adele in Outlook, and kept the default Outlook mailbox setting to direct meeting requests and responses to only delegates.</span></span> <span data-ttu-id="3ef21-112">（此设置对应于设置为默认值 `sendToDelegateOnly` 的 Alex [mailboxSettings](/graph/api/resources/mailboxsettings) 的 **delegateMeetingMessageDeliveryOptions** 属性。）</span><span class="sxs-lookup"><span data-stu-id="3ef21-112">(This setting corresponds to the **delegateMeetingMessageDeliveryOptions** property of Alex' [mailboxSettings](/graph/api/resources/mailboxsettings) set as the default value `sendToDelegateOnly`.)</span></span> 

<span data-ttu-id="3ef21-113">本演练介绍了几个后续步骤：</span><span class="sxs-lookup"><span data-stu-id="3ef21-113">The walkthrough describes a few subsequent steps:</span></span>
1. <span data-ttu-id="3ef21-114">[Adele 获取由 Alex 委派给她的日历](#step-1-adele-gets-the-delegated-calendar)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-114">[Adele gets the calendar that Alex has delegated to her](#step-1-adele-gets-the-delegated-calendar).</span></span>
2. <span data-ttu-id="3ef21-115">[Adele 代表 Alex 将会议邀请发送给 Christie 和 Megan](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-115">[Adele sends a meeting invitation to Christie and Megan on Alex' behalf](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf).</span></span> 
3. <span data-ttu-id="3ef21-116">[Christie 收到会议请求，并检查其日历中的关联事件](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-116">[Christie receives the meeting request, and inspects the associated event in her calendar](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar).</span></span>
4. <span data-ttu-id="3ef21-117">[Christie 对邀请做出暂定响应](#step-4-christie-responds-to-the-meeting-request)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-117">[Christie responds tentative to the invitation](#step-4-christie-responds-to-the-meeting-request).</span></span>
5. <span data-ttu-id="3ef21-118">[Adele 收到 Christie 的响应邮件](#step-5-adele-receives-the-response-message)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-118">[Adele receives Christie's response message](#step-5-adele-receives-the-response-message).</span></span>
6. <span data-ttu-id="3ef21-119">[作为活动的一部分，Alex 检查与会者的响应](#step-6-alex-accesses-responses-as-part-of-the-event)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-119">[Alex checks attendees' responses as part of the event](#step-6-alex-accesses-responses-as-part-of-the-event).</span></span>

<span data-ttu-id="3ef21-120">如果 Alex 已与 Adele 共享其日历，但未向 Adele 委派该日历：</span><span class="sxs-lookup"><span data-stu-id="3ef21-120">If Alex has shared and not delegated his calendar with Adele:</span></span>

- <span data-ttu-id="3ef21-121">如果以 Adele 的身份登录，则应用可以[获取 Alex 与 Adele 共享的日历](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-121">Signed in as Adele, an app can [get the calendar that Alex has shared with Adele](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span></span>
- <span data-ttu-id="3ef21-122">应用可以使用步骤 2 到 4 中的请求和响应，以与委派日历相同的方式应用于共享日历。</span><span class="sxs-lookup"><span data-stu-id="3ef21-122">The app can use the requests and responses in steps 2 to 4 to apply to the shared calendar the same way as the delegated calendar.</span></span>
- <span data-ttu-id="3ef21-123">在步骤 5 中，应用以 Alex 而不是 Adele 的身份登录，以接收 Christie 的响应邮件。</span><span class="sxs-lookup"><span data-stu-id="3ef21-123">In step 5, the app can sign in as Alex, instead of Adele, to receive Christie's response message.</span></span>

## <a name="step-1-adele-gets-the-delegated-calendar"></a><span data-ttu-id="3ef21-124">步骤 1：Adele 获取委派的日历</span><span class="sxs-lookup"><span data-stu-id="3ef21-124">Step 1: Adele gets the delegated calendar</span></span>

<span data-ttu-id="3ef21-125">以 Adele 的身份登录，获取她有权访问的日历并识别由 Alex 向她委派的日历，以便在下一步中使用它在该日历中创建事件。</span><span class="sxs-lookup"><span data-stu-id="3ef21-125">Signed in as Adele, get the calendars she has access to and identify the one Alex has delegated to her, so to use it in the next step to create an event in that calendar.</span></span> 

<span data-ttu-id="3ef21-126">**Microsoft Graph 权限**</span><span class="sxs-lookup"><span data-stu-id="3ef21-126">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3ef21-127">使用权限最 `Calendars.Read.Shared`的权限。</span><span class="sxs-lookup"><span data-stu-id="3ef21-127">Use the least privileged delegated permission, `Calendars.Read.Shared`.</span></span> <span data-ttu-id="3ef21-128">有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-128">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="3ef21-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef21-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_Adele_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="3ef21-130">C#</span><span class="sxs-lookup"><span data-stu-id="3ef21-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adele-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef21-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef21-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adele-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef21-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef21-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adele-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef21-133">Java</span><span class="sxs-lookup"><span data-stu-id="3ef21-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adele-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3ef21-134">请注意，成功响应包括响应代码 HTTP 200、Adele 自己的主要日历以及由 Alex 在 Adele 的邮箱中委派的日历副本，其中包含以下属性：</span><span class="sxs-lookup"><span data-stu-id="3ef21-134">Notice a successful response includes the response code HTTP 200, Adele's own primary calendar, and a copy of the calendar delegated by Alex in Adele's mailbox, with the following properties:</span></span>

- <span data-ttu-id="3ef21-135">**canShare** 为 false，因为 Adele 只是委托人，而不是日历所有者。</span><span class="sxs-lookup"><span data-stu-id="3ef21-135">**canShare** is false since Adele is only a delegate and not the calendar owner.</span></span>
- <span data-ttu-id="3ef21-136">**canEdit** 为 true，因为作为委托人，Adele 对委派日历中的非私人活动具有写入访问权限。</span><span class="sxs-lookup"><span data-stu-id="3ef21-136">**canEdit** is true since as delegate, Adele has write access to non-private events in the delegated calendar.</span></span>
- <span data-ttu-id="3ef21-137">**owner** 为 `Alex Wilber`，表示它是 Alex 的日历。</span><span class="sxs-lookup"><span data-stu-id="3ef21-137">**owner** is `Alex Wilber` indicating it is Alex' calendar.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_Adele_calendars",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
    "value": [
        {
            "id": "AQMkADGkAAAJMjAAAAA==",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
            "canShare": true,
            "canViewPrivateItems": true,
            "canEdit": true,
            "owner": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "AAMkADRpAABf0JlzAAA=",
            "name": "Alex Wilber",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m4eQ==",
            "canShare": false,
            "canViewPrivateItems": false,
            "canEdit": true,
            "owner": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    ]
}
```

> <span data-ttu-id="3ef21-138">**注意** 以 Adele 的身份登录，你也可以直接从 Alex 的邮箱获取委派的日历，方法是指定 Alex 的身份和 `calendar` 快捷方式，如 `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar` 中所示。</span><span class="sxs-lookup"><span data-stu-id="3ef21-138">**NOTE** Signed in as Adele, you can alternatively get the delegated calendar directly from Alex' mailbox, by specifying Alex' identity and the `calendar` shortcut, as in `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar`.</span></span> <span data-ttu-id="3ef21-139">返回的日历 ID 仅对应于 Alex 的邮箱。</span><span class="sxs-lookup"><span data-stu-id="3ef21-139">The returned calendar ID corresponds to only Alex' mailbox.</span></span> 

## <a name="step-2-adele-creates-and-sends-an-invitation-on-alex-behalf"></a><span data-ttu-id="3ef21-140">步骤 2：Adele 代表 Alex 创建并发送邀请</span><span class="sxs-lookup"><span data-stu-id="3ef21-140">Step 2: Adele creates and sends an invitation on Alex' behalf</span></span>

<span data-ttu-id="3ef21-141">以 Adele 身份登录，使用从步骤 1 获取的日历 ID 在委派日历创建 [事件](/graph/api/resources/event) ，并代表 Alex 将其发送给 Christie 和 Megan。</span><span class="sxs-lookup"><span data-stu-id="3ef21-141">Signed in as Adele, use the calendar ID obtained from step 1 to create an [event](/graph/api/resources/event) in the delegated calendar and send it to Christie and Megan, on Alex' behalf.</span></span>

<span data-ttu-id="3ef21-142">**Microsoft Graph 权限**</span><span class="sxs-lookup"><span data-stu-id="3ef21-142">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3ef21-143">使用权限最 `Calendars.ReadWrite.Shared`的权限。</span><span class="sxs-lookup"><span data-stu-id="3ef21-143">Use the least privileged delegated permission, `Calendars.ReadWrite.Shared`.</span></span> <span data-ttu-id="3ef21-144">有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-144">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADRpAABf0JlzAAA="],
  "name": "create_send_invitation"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkADRpAABf0JlzAAA=/events

Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Christmas dinner",
  "body": {
    "contentType": "HTML",
    "content": "Happy holidays!"
  },
  "start": {
      "dateTime": "2019-12-25T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-12-25T22:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Alex' home"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"meganb@contoso.onmicrosoft.com",
        "name": "Megan Bowen"
      },
      "type": "required"
    },
    {
      "emailAddress": {
        "address":"ChristieC@contoso.onmicrosoft.com",
        "name": "Christie Cline"
      },
      "type": "required"
    }
  ]
}
```

<span data-ttu-id="3ef21-145">请注意，成功响应包括 HTTP 201 和以下 [event](/graph/api/resources/event) 属性：</span><span class="sxs-lookup"><span data-stu-id="3ef21-145">Notice a successful response includes HTTP 201 and the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="3ef21-146">**isOrganizer** 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3ef21-146">**isOrganizer** is set to true.</span></span> <span data-ttu-id="3ef21-147">通常情况下，如果日历所有者 (Alex) 是会议的组织者，则此属性为 true。</span><span class="sxs-lookup"><span data-stu-id="3ef21-147">In general, this property is true if the calendar owner (Alex) is the organizer of the meeting.</span></span> <span data-ttu-id="3ef21-148">这也适用于委托人 (Adele) 代表所有者组织会议的情形。</span><span class="sxs-lookup"><span data-stu-id="3ef21-148">This also applies if a delegate (Adele) organized the meeting on behalf of the owner.</span></span>
- <span data-ttu-id="3ef21-149">**attendees** 集合指定 Megan 和 Christie。</span><span class="sxs-lookup"><span data-stu-id="3ef21-149">The **attendees** collection specifies Megan and Christie.</span></span>
- <span data-ttu-id="3ef21-150">**organizer** 设置为 Alex，因为邀请是由 Alex 的委托人 (Adele) 在 Alex 的主要日历中发送的。</span><span class="sxs-lookup"><span data-stu-id="3ef21-150">**organizer** is set to Alex, since the invitation was sent by Alex' delegate (Adele) in Alex' primary calendar.</span></span>
- <span data-ttu-id="3ef21-151">**attendees** 或 **organizer** 都未指定委托人 (Adele)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-151">Neither the **attendees** nor **organizer** specifies the delegate (Adele).</span></span>

<!-- {
  "blockType": "response",
  "name": "create_send_invitation",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars('AAMkADRpAABf0JlzAAA%3D')/events/$entity",
    "@odata.etag": "W/\"NDznl+Uh50WkanaCOKHkaQAAX8m47Q==\"",
    "id": "AAMkADI4oeRpAABf0LrcAAA=",
    "createdDateTime": "2019-12-21T04:59:01.9766929Z",
    "lastModifiedDateTime": "2019-12-21T04:59:02.0214967Z",
    "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m47Q==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": false,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI4oeRpAABf0LrcAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-25T18:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-12-25T22:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
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
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar"></a><span data-ttu-id="3ef21-152">步骤 3：Christie 收到会议请求，并检查其日历中的关联事件</span><span class="sxs-lookup"><span data-stu-id="3ef21-152">Step 3: Christie receives meeting request and inspects the associated event in her calendar</span></span>

<span data-ttu-id="3ef21-153">传递会议请求时，Outlook 会自动在 Christie 的日历中创建暂定 [event](/graph/api/resources/event)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-153">Upon delivering the meeting request, Outlook automatically creates a tentative [event](/graph/api/resources/event) in Christie's calendar.</span></span>

<span data-ttu-id="3ef21-154">以 Christie 的身份登录，获取与步骤 2 中的会议请求相关联的 [eventMessage](/graph/api/resources/eventmessage) 和 **event**：</span><span class="sxs-lookup"><span data-stu-id="3ef21-154">Signed in as Christie, get the [eventMessage](/graph/api/resources/eventmessage) and **event** that are associated with the meeting request from step 2.</span></span>

<span data-ttu-id="3ef21-155">**Microsoft Graph 权限**</span><span class="sxs-lookup"><span data-stu-id="3ef21-155">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3ef21-156">使用权限最少的委派每一个、 `Mail.Read` 和 `Calendar.Read.Shared`。</span><span class="sxs-lookup"><span data-stu-id="3ef21-156">Use the least privileged delegated permisson, `Mail.Read` and `Calendar.Read.Shared`.</span></span> <span data-ttu-id="3ef21-157">有关详细信息，请参阅 [权限](permissions-reference.md#mail-permissions) 以及 [权限](permissions-reference.md#calendars-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-157">For more information, see [mail permissions](permissions-reference.md#mail-permissions) and [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="3ef21-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef21-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5hYdAAA="],
  "name": "get_eventmessage_and_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADADVj3fyAABZ5hYdAAA=?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[<span data-ttu-id="3ef21-159">C#</span><span class="sxs-lookup"><span data-stu-id="3ef21-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-and-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef21-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef21-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-and-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef21-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef21-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-and-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef21-162">Java</span><span class="sxs-lookup"><span data-stu-id="3ef21-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-and-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3ef21-163">请注意，成功响应包括响应代码 HTTP 200 和以下 [eventMessage](/graph/api/resources/eventmessage) 属性：</span><span class="sxs-lookup"><span data-stu-id="3ef21-163">Notice a successful response includes the response code HTTP 200 and the following [eventMessage](/graph/api/resources/eventmessage) properties:</span></span>

- <span data-ttu-id="3ef21-164">**meetingMessageType** 指定此邮件为 `meetingRequest`。</span><span class="sxs-lookup"><span data-stu-id="3ef21-164">**meetingMessageType** specifies this message is `meetingRequest`.</span></span>
- <span data-ttu-id="3ef21-165">**sender** 是 Adele。</span><span class="sxs-lookup"><span data-stu-id="3ef21-165">**sender** is Adele.</span></span>
- <span data-ttu-id="3ef21-166">**from** 是 Alex。</span><span class="sxs-lookup"><span data-stu-id="3ef21-166">**from** is Alex.</span></span>
- <span data-ttu-id="3ef21-167">**toRecipients** 包括 Megan 和 Christie。</span><span class="sxs-lookup"><span data-stu-id="3ef21-167">**toRecipients** include Megan and Christie.</span></span>

<span data-ttu-id="3ef21-168">添加以下 [event](/graph/api/resources/event) 属性：</span><span class="sxs-lookup"><span data-stu-id="3ef21-168">And the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="3ef21-169">**attendees** 包括 Alex、Megan 和 Christie。</span><span class="sxs-lookup"><span data-stu-id="3ef21-169">**attendees** include Alex, Megan, and Christie.</span></span>
- <span data-ttu-id="3ef21-170">**organizer** 是 Alex。</span><span class="sxs-lookup"><span data-stu-id="3ef21-170">**organizer** is Alex.</span></span>

<span data-ttu-id="3ef21-171">Adele 的身份仅显示在 **eventMessage** 的 **sender** 属性中，而不是显示在关联的 **event** 中。</span><span class="sxs-lookup"><span data-stu-id="3ef21-171">Adele's identity appears only in the **sender** property of the **eventMessage** and not in the associated **event**.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages(microsoft.graph.eventMessage/event())/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h\"",
    "id": "AAMkADADVj3fyAABZ5hYdAAA=",
    "createdDateTime": "2019-12-21T04:59:03Z",
    "lastModifiedDateTime": "2019-12-21T04:59:04Z",
    "changeKey": "CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h",
    "categories": [],
    "receivedDateTime": "2019-12-21T04:59:03Z",
    "sentDateTime": "2019-12-21T04:59:01Z",
    "hasAttachments": false,
    "internetMessageId": "<DM6PR17MB3593711A1C0A098167F5A977A12C0@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "parentFolderId": "AQMkADIAAAIBDAAAAA==",
    "conversationId": "AAQkADNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADADVj3fyAABZ5hYdAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingRequest",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Adele Vance",
            "address": "AdeleV@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    },
    "event@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages('AAMkADADVj3fyAABZ5hYdAAA%3D')/microsoft.graph.eventMessage/microsoft.graph.eventMessage/event/$entity",
    "event": {
        "@odata.etag": "W/\"yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==\"",
        "id": "AAMkADADVj3fyAABZ5ieyAAA=",
        "createdDateTime": "2019-12-21T04:59:03.4336242Z",
        "lastModifiedDateTime": "2019-12-27T01:38:32.3766961Z",
        "changeKey": "yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==",
        "categories": [],
        "originalStartTimeZone": "Pacific Standard Time",
        "originalEndTimeZone": "Pacific Standard Time",
        "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
        "reminderMinutesBeforeStart": 15,
        "isReminderOn": true,
        "hasAttachments": false,
        "subject": "Christmas dinner",
        "bodyPreview": "Happy holidays!",
        "importance": "normal",
        "sensitivity": "normal",
        "isAllDay": false,
        "isCancelled": false,
        "isOrganizer": false,
        "responseRequested": true,
        "seriesMasterId": null,
        "showAs": "tentative",
        "type": "singleInstance",
        "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADADVj3fyAABZ5ieyAAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl": null,
        "recurrence": null,
        "responseStatus": {
            "response": "none",
            "time": "2019-12-21T05:16:48.8931825Z"
        },
        "body": {
            "contentType": "html",
            "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
        },
        "start": {
            "dateTime": "2019-12-26T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "end": {
            "dateTime": "2019-12-26T06:00:00.0000000",
            "timeZone": "UTC"
        },
        "location": {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        },
        "locations": [
            {
                "displayName": "Alex' home",
                "locationType": "default",
                "uniqueId": "1396aaf3-e344-4567-a4e3-797557ec24c8",
                "uniqueIdType": "locationStore"
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
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Christie Cline",
                    "address": "ChristieC@contoso.OnMicrosoft.com"
                }
            }
        ],
        "organizer": {
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    }
}
```


## <a name="step-4-christie-responds-to-the-meeting-request"></a><span data-ttu-id="3ef21-172">步骤 4：Christie 响应会议请求</span><span class="sxs-lookup"><span data-stu-id="3ef21-172">Step 4: Christie responds to the meeting request</span></span>

<span data-ttu-id="3ef21-173">以 Christie 的身份登录，将 **event** 答复为暂定，并在响应中包括答复邮件：</span><span class="sxs-lookup"><span data-stu-id="3ef21-173">Signed in as Christie, reply to the **event** as tentative, and include a reply message in the response:</span></span>

<span data-ttu-id="3ef21-174">**Microsoft Graph 权限**</span><span class="sxs-lookup"><span data-stu-id="3ef21-174">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3ef21-175">使用权限最 `Calendars.ReadWrite.Shared`的权限。</span><span class="sxs-lookup"><span data-stu-id="3ef21-175">Use the least privileged delegated permission, `Calendars.ReadWrite.Shared`.</span></span> <span data-ttu-id="3ef21-176">有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-176">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="3ef21-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef21-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5ieyAAA="],
  "name": "event_reply_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADADVj3fyAABZ5ieyAAA=/tentativelyAccept
Content-type: application/json

{
  "comment": "I will probably be able to make it.",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="3ef21-178">C#</span><span class="sxs-lookup"><span data-stu-id="3ef21-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-reply-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef21-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef21-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-reply-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef21-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef21-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-reply-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef21-181">Java</span><span class="sxs-lookup"><span data-stu-id="3ef21-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-reply-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3ef21-182">成功响应将返回“HTTP 202 已接受”。</span><span class="sxs-lookup"><span data-stu-id="3ef21-182">A successful response returns HTTP 202 Accepted.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


## <a name="step-5-adele-receives-the-response-message"></a><span data-ttu-id="3ef21-183">步骤 5：Adele 收到响应邮件</span><span class="sxs-lookup"><span data-stu-id="3ef21-183">Step 5: Adele receives the response message</span></span>

<span data-ttu-id="3ef21-184">由于 Adele 是 Alex 的主要日历的委托人，Adele 代表 Alex 收到了该日历的所有会议响应。</span><span class="sxs-lookup"><span data-stu-id="3ef21-184">Because Adele is a delegate of Alex' primary calendar, Adele receives all meeting responses for that calendar on Alex' behalf.</span></span>

<span data-ttu-id="3ef21-185">以 Adele 的身份登录，获取 [eventMessage](/graph/api/resources/eventmessage)，它表示由 Christie 在步骤 4 中做出的响应：</span><span class="sxs-lookup"><span data-stu-id="3ef21-185">Signed in as Adele, get the [eventMessage](/graph/api/resources/eventmessage) that represents the response from Christie in step 4.</span></span>

<span data-ttu-id="3ef21-186">**Microsoft Graph 权限**</span><span class="sxs-lookup"><span data-stu-id="3ef21-186">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3ef21-187">使用权限最 `Mail.Read.Shared`的权限。</span><span class="sxs-lookup"><span data-stu-id="3ef21-187">Use the least privileged delegated permission, `Mail.Read.Shared`.</span></span> <span data-ttu-id="3ef21-188">有关详细信息，请参阅 [邮件权限](permissions-reference.md#mail-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-188">For more information, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="3ef21-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef21-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI4oeRpAABf0HJUAAA="],
  "name": "message_get_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI4oeRpAABf0HJUAAA=
```
# <a name="c"></a>[<span data-ttu-id="3ef21-190">C#</span><span class="sxs-lookup"><span data-stu-id="3ef21-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef21-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef21-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef21-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef21-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef21-193">Java</span><span class="sxs-lookup"><span data-stu-id="3ef21-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3ef21-194">请注意，成功响应包括响应代码 HTTP 200 和以下 [eventMessage](/graph/api/resources/eventmessage) 属性：</span><span class="sxs-lookup"><span data-stu-id="3ef21-194">Notice a successful response includes the response code HTTP 200 and the following [eventMessage](/graph/api/resources/eventmessage) properties:</span></span>

- <span data-ttu-id="3ef21-195">**meetingMessageType** 为 `meetingTenativelyAccepted`。</span><span class="sxs-lookup"><span data-stu-id="3ef21-195">**meetingMessageType** is `meetingTenativelyAccepted`.</span></span>
- <span data-ttu-id="3ef21-196">**from** 是 Christie。</span><span class="sxs-lookup"><span data-stu-id="3ef21-196">**from** is Christie.</span></span>
- <span data-ttu-id="3ef21-197">**toRecipients** 仅包括 Adele，而不是日历所有者 Alex。</span><span class="sxs-lookup"><span data-stu-id="3ef21-197">**toRecipients** includes only Adele, but not the calendar owner Alex.</span></span> <span data-ttu-id="3ef21-198">这是因为 Alex 保留了让 Outlook 将所有会议响应仅定向给委托人的默认设置。</span><span class="sxs-lookup"><span data-stu-id="3ef21-198">This is because Alex kept the default to have Outlook direct all meeting responses to only delegates.</span></span>

<!-- {
  "blockType": "response",
  "name": "message_get_reply",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/messages/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT\"",
    "id": "AAMkADI4oeRpAABf0HJUAAA=",
    "createdDateTime": "2019-12-21T05:16:55Z",
    "lastModifiedDateTime": "2019-12-21T05:16:57Z",
    "changeKey": "DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT",
    "categories": [],
    "receivedDateTime": "2019-12-21T05:16:56Z",
    "sentDateTime": "2019-12-21T05:16:49Z",
    "hasAttachments": false,
    "internetMessageId": "<86880ccb8ec64184996e46eaddaed279@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Tentative: Christmas dinner",
    "bodyPreview": "I will probably be able to make it.",
    "importance": "normal",
    "parentFolderId": "AQMkAD5GkAAAIBDAAAAA==",
    "conversationId": "AAQkADK25bhNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAwAAoBoZ",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": false,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADI4oeRpAABf0HJUAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingTenativelyAccepted",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nI will probably be able to make it.\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

## <a name="step-6-alex-accesses-responses-as-part-of-the-event"></a><span data-ttu-id="3ef21-199">步骤 6：作为活动的一部分，Alex 访问响应</span><span class="sxs-lookup"><span data-stu-id="3ef21-199">Step 6: Alex accesses responses as part of the event</span></span>

<span data-ttu-id="3ef21-200">由于 Alex 保留了让 Outlook 将所有会议请求和响应仅定向给委托人的默认设置，Alex 不会收到 Christie 在步骤 4 中做出的响应。</span><span class="sxs-lookup"><span data-stu-id="3ef21-200">Because Alex kept the default to have Outlook direct all meeting requests and responses to only delegates, Alex does not receive Christie's response from step 4.</span></span> <span data-ttu-id="3ef21-201">但是，他可以通过其主要日历中的 [event](/graph/api/resources/event) 获取响应。</span><span class="sxs-lookup"><span data-stu-id="3ef21-201">He can however get the response through the [event](/graph/api/resources/event) in his primary calendar.</span></span>

<span data-ttu-id="3ef21-202">以 Alex 登录，获取 [Adele 在步骤 2](/graph/api/resources/event) 中创建的  事件，并获取来自 **"** 答复。</span><span class="sxs-lookup"><span data-stu-id="3ef21-202">Signed in as Alex, get the [event](/graph/api/resources/event) that Adele created in step 2 and get responses from the **attendees** property.</span></span>

<span data-ttu-id="3ef21-203">**Microsoft Graph 权限**</span><span class="sxs-lookup"><span data-stu-id="3ef21-203">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="3ef21-204">使用权限最 `Calendars.Read`的权限。</span><span class="sxs-lookup"><span data-stu-id="3ef21-204">Use the least privileged delegated permission, `Calendars.Read`.</span></span> <span data-ttu-id="3ef21-205">有关详细信息，请参阅[日历权限](permissions-reference.md#calendars-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-205">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="3ef21-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef21-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADJXJGu0AABf02qwAAA="],
  "name": "event_get_responses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events/AAMkADJXJGu0AABf02qwAAA=
```
# <a name="c"></a>[<span data-ttu-id="3ef21-207">C#</span><span class="sxs-lookup"><span data-stu-id="3ef21-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-responses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef21-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef21-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-responses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef21-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef21-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-responses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ef21-210">Java</span><span class="sxs-lookup"><span data-stu-id="3ef21-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-responses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3ef21-211">请注意，成功响应包括响应代码 HTTP 200 和以下 [event](/graph/api/resources/event) 属性：</span><span class="sxs-lookup"><span data-stu-id="3ef21-211">Notice a successful response includes the response code HTTP 200 and the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="3ef21-212">**isOrganizer** 为 true。</span><span class="sxs-lookup"><span data-stu-id="3ef21-212">**isOrganizer** is true.</span></span>
- <span data-ttu-id="3ef21-213">**attendees** 仅包括 Megan 和 Christie。</span><span class="sxs-lookup"><span data-stu-id="3ef21-213">**attendees** include only Megan and Christie.</span></span>
- <span data-ttu-id="3ef21-214">每个 **attendee** 实例的 **status** 属性均指示参与者的任何响应：</span><span class="sxs-lookup"><span data-stu-id="3ef21-214">The **status** property of each **attendee** instance indicates any response from the attendee:</span></span>
  - <span data-ttu-id="3ef21-215">Megan 的响应是 `none`。</span><span class="sxs-lookup"><span data-stu-id="3ef21-215">Megan's response is `none`.</span></span>
  - <span data-ttu-id="3ef21-216">Christie 的响应是 `tentativelyAccepted`。</span><span class="sxs-lookup"><span data-stu-id="3ef21-216">Christie's response is `tentativelyAccepted`.</span></span>
- <span data-ttu-id="3ef21-217">**organizer** 是 Alex。</span><span class="sxs-lookup"><span data-stu-id="3ef21-217">**organizer** is Alex.</span></span>
- <span data-ttu-id="3ef21-218">返回的 **event** 中没有任何属性指示委托人 Adele。</span><span class="sxs-lookup"><span data-stu-id="3ef21-218">No property in the returned **event** indicates the delegate, Adele.</span></span>

<!-- {
  "blockType": "response",
  "name": "event_get_responses",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AQMkADAw7QAAAJfygAAAA%3D%3D')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==\"",
    "id": "AAMkADJXJGu0AABf02qwAAA=",
    "createdDateTime": "2019-12-21T04:59:01.4435895Z",
    "lastModifiedDateTime": "2019-12-21T05:16:54.689345Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADJXJGu0AABf02qwAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-26T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-12-26T06:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
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
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "tentativelyAccepted",
                "time": "2019-12-21T05:16:48.8931825Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="next-steps"></a><span data-ttu-id="3ef21-219">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3ef21-219">Next steps</span></span>

<span data-ttu-id="3ef21-220">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="3ef21-220">Find out more about:</span></span>

- [<span data-ttu-id="3ef21-221">获取共享日历或委托日历中的 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="3ef21-221">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="3ef21-222">在 Outlook（预览版）中共享或委派日历</span><span class="sxs-lookup"><span data-stu-id="3ef21-222">Share or delegate a calendar in Outlook (preview)</span></span>](outlook-share-or-delegate-calendar.md)
- [<span data-ttu-id="3ef21-223">为什么要与 Outlook 日历集成</span><span class="sxs-lookup"><span data-stu-id="3ef21-223">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="3ef21-224">Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar)。</span><span class="sxs-lookup"><span data-stu-id="3ef21-224">The [calendar API](/graph/api/resources/calendar) in Microsoft Graph v1.0.</span></span>
