---
title: 获取共享或委托的 Outlook 日历及其事件
description: 在 Outlook 中，日历所有者可与其他用户共享日历，并让他们查看或修改该日历中的事件；日历可以是自定义日历或主日历。 所有者还可以授权代理人代表其执行操作，接收或答复会议请求，或在电子邮件帐户的主日历中创建或更改项目。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: afa12541519f5f6f2db24ab5d68644dbdba8572b
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652021"
---
# <a name="get-shared-or-delegated-outlook-calendar-and-its-events"></a><span data-ttu-id="67b70-104">获取共享或委托的 Outlook 日历及其事件</span><span class="sxs-lookup"><span data-stu-id="67b70-104">Get shared or delegated Outlook calendar and its events</span></span>

<span data-ttu-id="67b70-105">在 Outlook 中，日历所有者可与其他用户共享日历，并让他们查看或修改该日历中的事件；共享日历可以是所有者的主日历或由所有者创建的自定义日历。</span><span class="sxs-lookup"><span data-stu-id="67b70-105">In Outlook, a calendar owner can share a calendar with other users and let them view or modify events in that calendar; the shared calendar can be the owner's primary calendar or a custom calendar created by the owner.</span></span> <span data-ttu-id="67b70-106">所有者还可以向其主日历授权代理人以代表其执行操作，接收或答复会议请求，或在主日历中创建或更改项目。</span><span class="sxs-lookup"><span data-stu-id="67b70-106">The owner can also grant a delegate to their primary calendar and act on their behalf, to receive or respond to meeting requests, or create or change items in the primary calendar.</span></span>

<span data-ttu-id="67b70-107">Microsoft Graph 支持以编程方式读取和写入其他用户已共享的日历中的事件、读取共享日历以及更新共享者的日历名称。</span><span class="sxs-lookup"><span data-stu-id="67b70-107">Programmatically, Microsoft Graph supports reading and writing events in calendars that have been shared by other users, as well as reading the shared calendars, and updating the calendar name for sharees.</span></span> <span data-ttu-id="67b70-108">此支持还适用于已委托的日历。</span><span class="sxs-lookup"><span data-stu-id="67b70-108">The support also applies to calendars that have been delegated.</span></span> <span data-ttu-id="67b70-109">本文的其余部分介绍如何在共享或委托的日历中读取事件。</span><span class="sxs-lookup"><span data-stu-id="67b70-109">The rest of this article describes reading events in a shared or delegated calendar.</span></span> <span data-ttu-id="67b70-110">有关创建事件的信息，请参阅[在共享日历或委托的日历中创建 Outlook 事件](outlook-create-event-in-shared-delegated-calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="67b70-110">For creating events, refer to [Create Outlook events in a shared or delegated calendar](outlook-create-event-in-shared-delegated-calendar.md).</span></span>

## <a name="sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox"></a><span data-ttu-id="67b70-111">共享者：直接从日历所有者的邮箱获取共享日历或其事件</span><span class="sxs-lookup"><span data-stu-id="67b70-111">Sharee: Get a shared calendar or its events directly from calendar owner's mailbox</span></span>

<span data-ttu-id="67b70-112">以下三个示例假设这样的情景：在 Outlook 中，Alex 向 Megan 共享了他的主日历，并给予 Megan 读取权限。</span><span class="sxs-lookup"><span data-stu-id="67b70-112">The three examples below use this scenario: in Outlook, Alex has shared his primary calendar with Megan and given Megan read permissions.</span></span> <span data-ttu-id="67b70-113">如果 Megan 登录你的应用，并提供_委托权限_ (Calendars.Read.Shared or Calendars.ReadWrite.Shared)，代表 Megan，你的应用可以直接从 Alex 的邮箱中访问 Alex 的主日历及其事件。</span><span class="sxs-lookup"><span data-stu-id="67b70-113">If Megan signs into your app and provides _delegated permissions_ (Calendars.Read.Shared or Calendars.ReadWrite.Shared), on behalf of Megan, your app can access Alex' primary calendar and its events directly from Alex' mailbox.</span></span>

<span data-ttu-id="67b70-114">三个示例指定了所有者的标识（Alex 的用户 ID 或用户主体名称）和 `calendar` 快捷方式。</span><span class="sxs-lookup"><span data-stu-id="67b70-114">The three examples specify the owner's identity (Alex' user ID or user principal name) and the `calendar` shortcut.</span></span> <span data-ttu-id="67b70-115">这些示例仅访问与所有者的邮箱对应的日历和事件 ID。</span><span class="sxs-lookup"><span data-stu-id="67b70-115">They access calendar and event IDs that correspond to only the owner's mailbox.</span></span> <span data-ttu-id="67b70-116">在共享者的邮箱（Megan 的用户 ID 或用户主体名称）中指定这些日历和事件 ID 将返回错误。</span><span class="sxs-lookup"><span data-stu-id="67b70-116">Specifying these calendar and event IDs in the sharee's mailbox (Megan's user ID or user principal name) would return an error.</span></span> <span data-ttu-id="67b70-117">若要使用与共享者的邮箱对应的日历和事件 ID，请参阅[共享者：从共享者的邮箱获取共享的自定义日历或其事件](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="67b70-117">To use calendar and event IDs that correspond to the sharee's mailbox, see [Sharee: Get shared, custom calendar or its events from sharee's mailbox](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span></span> 

> <span data-ttu-id="67b70-118">**注意**：通过共享权限（Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），你可以在共享或委托的日历中读取或写入事件。</span><span class="sxs-lookup"><span data-stu-id="67b70-118">**Note**: The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="67b70-119">它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="67b70-119">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="67b70-120">若要对租户中共享、委托或任何其他用户或资源日历中的事件设置更改通知订阅，请使用应用程序权限 Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="67b70-120">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

### <a name="megan-get-the-shared-primary-calendar-directly-from-alex-mailbox"></a><span data-ttu-id="67b70-121">Megan：直接从 Alex 的邮箱获取共享的主日历</span><span class="sxs-lookup"><span data-stu-id="67b70-121">Megan: Get the shared, primary calendar directly from Alex' mailbox</span></span>

<span data-ttu-id="67b70-122">以 Megan 的身份登录，直接从 Alex 的邮箱获取 Alex 向 Megan 共享的主日历：</span><span class="sxs-lookup"><span data-stu-id="67b70-122">Signed in as Megan, get the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar
```

<span data-ttu-id="67b70-123">成功完成后，你将收到 HTTP 200 OK 消息和一个[日历](/graph/api/resources/calendar?view=graph-rest-1.0)实例，该实例表示 Alex 在Alex 的邮箱中共享的主日历。</span><span class="sxs-lookup"><span data-stu-id="67b70-123">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Alex' shared, primary calendar, in Alex' mailbox.</span></span>

### <a name="megan-get-an-event-in-the-shared-primary-calendar-directly-from-alex-mailbox"></a><span data-ttu-id="67b70-124">Megan：直接从 Alex 的邮箱获取共享主日历中的事件</span><span class="sxs-lookup"><span data-stu-id="67b70-124">Megan: Get an event in the shared, primary calendar directly from Alex' mailbox</span></span>

<span data-ttu-id="67b70-125">以 Megan 的身份登录，你的应用可以直接从 Alex 的邮箱获取 Alex 向 Megan 共享的主日历中的特定事件：</span><span class="sxs-lookup"><span data-stu-id="67b70-125">Signed in as Megan, your app can get a specific event in the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="67b70-126">成功完成后，你将收到 HTTP 200 OK 消息以及 Alex 的主日历中由 `{id}` 标识的[事件](/graph/api/resources/event?view=graph-rest-1.0)实例（直接从 Alex 的邮箱获取）。</span><span class="sxs-lookup"><span data-stu-id="67b70-126">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` in Alex' primary calendar, directly from Alex' mailbox.</span></span>

### <a name="megan-get-all-the-events-in-the-shared-primary-calendar-from-alex-mailbox"></a><span data-ttu-id="67b70-127">Megan：从 Alex 的邮箱获取共享主日历中的所有事件</span><span class="sxs-lookup"><span data-stu-id="67b70-127">Megan: Get all the events in the shared, primary calendar from Alex' mailbox</span></span>

<span data-ttu-id="67b70-128">以 Megan 的身份登录，直接从 Alex 的邮箱获取 Alex 向 Megan 共享的主日历中的所有事件：</span><span class="sxs-lookup"><span data-stu-id="67b70-128">Signed in as Megan, get all the events in the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events
```

<span data-ttu-id="67b70-129">成功完成后，你将收到 HTTP 200 OK 消息以及 Alex 的主日历中的一组[事件](/graph/api/resources/event?view=graph-rest-1.0)实例（直接从 Alex 的邮箱获取）。</span><span class="sxs-lookup"><span data-stu-id="67b70-129">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Alex' primary calendar, directly from Alex' mailbox.</span></span>

<span data-ttu-id="67b70-130">如果 Alex 已委托 Megan 访问 Alex 的主日历，或者 Alex 向 Megan 委托了其整个邮箱，则将适用同样的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="67b70-130">The same GET capabilities apply if Alex has delegated Megan access to Alex' primary calendar, or if Alex has delegated Megan his entire mailbox.</span></span>

<span data-ttu-id="67b70-131">如果 Alex 尚未向 Megan 共享也未委托其主日历，则在前面的 GET 操作中指定 Alex 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="67b70-131">If Alex has not shared nor delegated his primary calendar with Megan, specifying Alex’s user ID or user principal name in the preceding GET operations will return an error.</span></span> 


## <a name="sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox"></a><span data-ttu-id="67b70-132">共享者：从共享者的邮箱获取共享的自定义日历或其事件</span><span class="sxs-lookup"><span data-stu-id="67b70-132">Sharee: Get shared, custom calendar or its events from sharee's mailbox</span></span>

<span data-ttu-id="67b70-133">如果 Alex 向 Adele 共享了一个_自定义_日历（例如，名为“Kids parties”的日历），并且 Adele 提供了委托权限（Calendars.Read 或 Calendars.ReadWrite），则你的应用可以从 Adele 邮箱中的 Alex 日历本地副本获取事件或日历，如下所述。</span><span class="sxs-lookup"><span data-stu-id="67b70-133">If Alex has shared a _custom_ calendar (as an example, a calendar named "Kids parties") with Adele, and Adele has provided delegated permissions (Calendars.Read or Calendars.ReadWrite), your app can get the events or calendar from the local copy of Alex' calendar in Adele's mailbox, as described below.</span></span>

1. <span data-ttu-id="67b70-134">以 Adele 的身份登录，使用以下任一请求获取 Adele 有权访问的所有日历，包括共享的自定义日历。</span><span class="sxs-lookup"><span data-stu-id="67b70-134">Signed in as Adele, use either of the following requests to get all the calendars that Adele has access to, including the shared custom calendar.</span></span>

    <!-- {
      "blockType": "request",
      "name": "get_all_Adele_calendars"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars
    ```

    <span data-ttu-id="67b70-135">成功后的响应包括响应代码 HTTP 200 以及 Adele 有权访问的一组日历，包括所有者名称为“Alex Wilber”的日历（“Kids parties”），作为响应中的第二个日历。</span><span class="sxs-lookup"><span data-stu-id="67b70-135">A successful response includes the response code HTTP 200, and the collection of calendars that Adele has access to, including the calendar ("Kids parties") that has the owner name as "Alex Wilber" as the second calendar in the response.</span></span> <span data-ttu-id="67b70-136">对于共享者“Adele”，共享日历的 **canShare** 属性始终为 false。</span><span class="sxs-lookup"><span data-stu-id="67b70-136">For a sharee, Adele, the **canShare** property of the shared calendar is always false.</span></span>

    <!-- {
      "blockType": "response",
      "name": "get_all_Adele_calendars",
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
                "id": "AQMkADU5NAAAJMjAAAAA==",
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
                "id": "AAMkADAABf0JlyAAA=",
                "name": "Kids parties",
                "color": "lightYellow",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAYumJRQ==",
                "canShare": false,
                "canViewPrivateItems": false,
                "canEdit": false,
                "owner": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            }
        ]
    }
    ```

2. <span data-ttu-id="67b70-137">以 Adele 的身份登录，获取共享日历或获取共享日历中的一个或多个事件（使用步骤 1 的响应中的第二个日历 ID）。</span><span class="sxs-lookup"><span data-stu-id="67b70-137">Signed in as Adele, get the shared calendar, or get one or more events in the shared calendar, using the second calendar ID in the response from step 1.</span></span> <span data-ttu-id="67b70-138">共享日历的 ID 及其事件对应于 Adele 邮箱中的 Alex 日历本地副本。</span><span class="sxs-lookup"><span data-stu-id="67b70-138">The IDs of the shared calendar and its event correspond to the local copy of Alex' calendar in Adele's mailbox.</span></span>

    <!-- { "blockType": "ignored" } -->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events/{id}
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events/{id}

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events
    ```

<span data-ttu-id="67b70-139">成功完成后，你将收到 HTTP 200 OK 消息以及所请求的一个或多个事件或 Alex 向 Adele 共享的日历。</span><span class="sxs-lookup"><span data-stu-id="67b70-139">On successful completion, you'll get HTTP 200 OK and the requested event, events, or calendar that Alex has shared with Adele.</span></span>


## <a name="next-steps"></a><span data-ttu-id="67b70-140">后续步骤</span><span class="sxs-lookup"><span data-stu-id="67b70-140">Next steps</span></span>

<span data-ttu-id="67b70-141">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="67b70-141">Find out more about:</span></span>

- [<span data-ttu-id="67b70-142">在共享或委托的日历中创建 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="67b70-142">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="67b70-143">在 Outlook 中共享或委托日历（预览版）</span><span class="sxs-lookup"><span data-stu-id="67b70-143">Share or delegate a calendar in Outlook (preview)</span></span>](outlook-share-or-delegate-calendar.md)
- [<span data-ttu-id="67b70-144">为什么要与 Outlook 日历集成</span><span class="sxs-lookup"><span data-stu-id="67b70-144">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="67b70-145">Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="67b70-145">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
