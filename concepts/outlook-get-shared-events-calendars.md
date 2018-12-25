---
title: 获取共享日历或委托日历中的 Outlook 事件
description: 在 Outlook 中，客户可以与其他用户共享日历，并允许其他用户查看或修改此日历中的事件。 客户还可以授权代理代表自己执行操作、接收或答复会议请求，或在日历中创建或更改项。
author: angelgolfer-ms
ms.openlocfilehash: ef4de6cedeeb9a5688f250652eef0cd6cd5f5183
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413146"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="30c1e-104">获取共享日历或委托日历中的 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="30c1e-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="30c1e-105">在 Outlook 中，客户可以与其他用户共享日历，并允许其他用户查看或修改此日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="30c1e-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="30c1e-106">客户还可以授权代理代表自己执行操作、接收或答复会议请求，或在日历中创建或更改项。</span><span class="sxs-lookup"><span data-stu-id="30c1e-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="30c1e-107">Microsoft Graph 支持以编程方式获取其他用户已共享日历中的事件，以及共享日历本身。</span><span class="sxs-lookup"><span data-stu-id="30c1e-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="30c1e-108">此支持还适用于已委托的日历。</span><span class="sxs-lookup"><span data-stu-id="30c1e-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="30c1e-109">例如，Garth 已与 John 共享自己的默认日历，并向 John 授予读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="30c1e-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="30c1e-110">如果 John 已登录应用并授予委托的权限（Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），应用便能访问 Garth 的默认日历及其中的事件，如下所述。</span><span class="sxs-lookup"><span data-stu-id="30c1e-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

> <span data-ttu-id="30c1e-111">**注意**通过共享权限（Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），你可以在共享或委托日历中读取或写入事件。</span><span class="sxs-lookup"><span data-stu-id="30c1e-111">**Note** The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="30c1e-112">它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="30c1e-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="30c1e-113">若要对租户中共享、委托或任何其他用户或资源日历中的事件设置更改通知订阅，请使用应用程序权限 Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="30c1e-113">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="30c1e-114">获取共享日历中的事件</span><span class="sxs-lookup"><span data-stu-id="30c1e-114">Get an event in the shared calendar</span></span>

<span data-ttu-id="30c1e-115">可以获取 Garth 共享的默认日历中的特定事件：</span><span class="sxs-lookup"><span data-stu-id="30c1e-115">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="30c1e-116">成功完成后，便会收到“HTTP 200 正常”消息，以及 Garth 默认日历中由 `{id}` 标识的 [event](/graph/api/resources/event?view=graph-rest-1.0) 实例。</span><span class="sxs-lookup"><span data-stu-id="30c1e-116">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="30c1e-117">获取共享日历中的所有事件</span><span class="sxs-lookup"><span data-stu-id="30c1e-117">Get all the events in the shared calendar</span></span>

<span data-ttu-id="30c1e-118">获取 Garth 已与 John 共享的默认日历中的所有事件：</span><span class="sxs-lookup"><span data-stu-id="30c1e-118">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="30c1e-119">成功完成后，便会收到“HTTP 200 正常”消息，以及 Garth 默认日历中的 [event](/graph/api/resources/event?view=graph-rest-1.0) 实例集合。</span><span class="sxs-lookup"><span data-stu-id="30c1e-119">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="30c1e-120">获取共享日历</span><span class="sxs-lookup"><span data-stu-id="30c1e-120">Get the shared calendar</span></span>

<span data-ttu-id="30c1e-121">获取 Garth 已与 John 共享的默认日历。</span><span class="sxs-lookup"><span data-stu-id="30c1e-121">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="30c1e-122">成功完成后，便会收到“HTTP 200 正常”消息，以及表示 Garth 默认文件夹的 [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) 实例。</span><span class="sxs-lookup"><span data-stu-id="30c1e-122">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="30c1e-123">如果 Garth 已委托 John 进一步访问自己的默认日历，或如果 Garth 已将自己的整个邮箱委托给 John，那么相同的 GET 功能适用。</span><span class="sxs-lookup"><span data-stu-id="30c1e-123">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="30c1e-124">如果 Garth 既未与 John 共享自己的默认日历，也未将自己的邮箱委托给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称便会返回错误。</span><span class="sxs-lookup"><span data-stu-id="30c1e-124">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="30c1e-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="30c1e-125">Next steps</span></span>

<span data-ttu-id="30c1e-126">详细了解：</span><span class="sxs-lookup"><span data-stu-id="30c1e-126">Find out more about:</span></span>

- [<span data-ttu-id="30c1e-127">为什么要与 Outlook 日历集成</span><span class="sxs-lookup"><span data-stu-id="30c1e-127">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="30c1e-128">Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="30c1e-128">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>