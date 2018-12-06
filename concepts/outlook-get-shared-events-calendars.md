---
title: 共享或委派的日历中获取 Outlook 事件
description: 在 Outlook 中，客户可以与其他用户共享日历并让他人查看或修改该日历中的事件。 客户还可以授予其代表，以接收或响应会议请求，或者创建或更改日历中的项目的代理人。
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091821"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="a04c2-104">共享或委派的日历中获取 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="a04c2-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="a04c2-105">在 Outlook 中，客户可以与其他用户共享日历并让他人查看或修改该日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="a04c2-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="a04c2-106">客户还可以授予其代表，以接收或响应会议请求，或者创建或更改日历中的项目的代理人。</span><span class="sxs-lookup"><span data-stu-id="a04c2-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="a04c2-107">以编程方式，Microsoft Graph 支持获取已由其他用户共享的日历中的事件，以及获取共享日历本身。</span><span class="sxs-lookup"><span data-stu-id="a04c2-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="a04c2-108">支持也适用于已委派的日历。</span><span class="sxs-lookup"><span data-stu-id="a04c2-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="a04c2-109">例如，Garth 具有与 John 共享其默认日历和授予 John 读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="a04c2-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="a04c2-110">如果 John 已登录到您的应用程序，并提供委派的权限 （Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），您的应用程序都将能够访问 Garth 的默认日历和事件，如下所述的日历中。</span><span class="sxs-lookup"><span data-stu-id="a04c2-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="a04c2-111">共享日历中获取事件</span><span class="sxs-lookup"><span data-stu-id="a04c2-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="a04c2-112">您可以获取 Garth 的共享的默认日历中的特定事件：</span><span class="sxs-lookup"><span data-stu-id="a04c2-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="a04c2-113">在操作成功完成，您将获取 HTTP 200 确定和[事件](/graph/api/resources/event?view=graph-rest-1.0)实例由标识`{id}`Garth 的默认日历。</span><span class="sxs-lookup"><span data-stu-id="a04c2-113">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="a04c2-114">共享日历中获取所有事件</span><span class="sxs-lookup"><span data-stu-id="a04c2-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="a04c2-115">获取与 John 共享 Garth 默认日历中的所有事件：</span><span class="sxs-lookup"><span data-stu-id="a04c2-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="a04c2-116">在操作成功完成，您将获取 HTTP 200 确定和 Garth 的默认日历中的[事件](/graph/api/resources/event?view=graph-rest-1.0)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="a04c2-116">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="a04c2-117">获取共享的日历</span><span class="sxs-lookup"><span data-stu-id="a04c2-117">Get the shared calendar</span></span>

<span data-ttu-id="a04c2-118">获取与 John 共享 Garth 的默认日历。</span><span class="sxs-lookup"><span data-stu-id="a04c2-118">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="a04c2-119">在操作成功完成，您将获取 HTTP 200 确定和代表 Garth 的默认文件夹的[日历](/graph/api/resources/calendar?view=graph-rest-1.0)实例。</span><span class="sxs-lookup"><span data-stu-id="a04c2-119">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="a04c2-120">如果 Garth 具有委派 John 进一步访问 Garth 的默认日历，或者 Garth 具有委派 John 其整个邮箱将应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="a04c2-120">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="a04c2-121">如果 Garth 不具有与 John、 共享其默认日历也有他代理其邮箱到 John，这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="a04c2-121">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="a04c2-122">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a04c2-122">Next steps</span></span>

<span data-ttu-id="a04c2-123">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="a04c2-123">Find out more about:</span></span>

- [<span data-ttu-id="a04c2-124">为什么与 Outlook 日历集成</span><span class="sxs-lookup"><span data-stu-id="a04c2-124">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="a04c2-125">Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar?view=graph-rest-1.0) 。</span><span class="sxs-lookup"><span data-stu-id="a04c2-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>