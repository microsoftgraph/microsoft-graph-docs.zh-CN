# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="3a80e-101">获取共享或委派日历中 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="3a80e-101">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="3a80e-102">在 Outlook 中，客户可以与其他用户共享日历，并让他们查看或修改该日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="3a80e-102">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="3a80e-103">客户还可以授予委托代表他们行事，以接收或回复会议请求，或创建或更改日历中的项。</span><span class="sxs-lookup"><span data-stu-id="3a80e-103">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="3a80e-104">Microsoft Graph 以编程方式支持获取已由其他用户共享的日历中的事件，以及获取共享日历本身。</span><span class="sxs-lookup"><span data-stu-id="3a80e-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="3a80e-105">该支持还适用于已委派的日历。</span><span class="sxs-lookup"><span data-stu-id="3a80e-105">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="3a80e-106">例如，Garth 与 John 共享了他的默认日历，并授予 John 读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="3a80e-106">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="3a80e-107">如果 John 已登录你的应用并提供了委派权限 (Calendars.Read.Shared or Calendars.ReadWrite.Shared)，则你的应用将能够访问 Garth 在该日历中的默认日历和事件，如下所述。</span><span class="sxs-lookup"><span data-stu-id="3a80e-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="3a80e-108">获取共享日历中的事件</span><span class="sxs-lookup"><span data-stu-id="3a80e-108">Get an event in the shared calendar</span></span>

<span data-ttu-id="3a80e-109">你可以获取 Garth 的共享的默认日历中的特定事件：</span><span class="sxs-lookup"><span data-stu-id="3a80e-109">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="3a80e-110">成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 默认日历中由`{id}`标识的[事件](../api-reference/v1.0/resources/event.md)实例。</span><span class="sxs-lookup"><span data-stu-id="3a80e-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/event.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="3a80e-111">获取共享日历中的所有事件</span><span class="sxs-lookup"><span data-stu-id="3a80e-111">Get all the events in the shared calendar</span></span>

<span data-ttu-id="3a80e-112">获取 Garth 与 John 共享的默认日历中的所有事件：</span><span class="sxs-lookup"><span data-stu-id="3a80e-112">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="3a80e-113">成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 的默认日历中的[事件](../api-reference/v1.0/resources/event.md)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="3a80e-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/event.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="3a80e-114">获取共享的日历</span><span class="sxs-lookup"><span data-stu-id="3a80e-114">Get the shared folder</span></span>

<span data-ttu-id="3a80e-115">获取 Garth 与 John 共享的默认日历。</span><span class="sxs-lookup"><span data-stu-id="3a80e-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="3a80e-116">成功完成后，你将收到“HTTP 200 正常”消息以及表示 Garth 默认文件夹的[日历](../api-reference/v1.0/resources/calendar.md)实例。</span><span class="sxs-lookup"><span data-stu-id="3a80e-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/calendar.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="3a80e-117">如果 Garth 已经委派 John 进一步访问他的默认日历，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="3a80e-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="3a80e-118">如果 Garth 未与 John 共享他的默认日历，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="3a80e-118">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="3a80e-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3a80e-119">Next steps</span></span>

<span data-ttu-id="3a80e-120">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="3a80e-120">Find out more about:</span></span>

- [<span data-ttu-id="3a80e-121">为什么与 Outlook 日历集成</span><span class="sxs-lookup"><span data-stu-id="3a80e-121">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="3a80e-122">Microsoft Graph v1.0 中的 [日历 API](../api-reference/v1.0/resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="3a80e-122">The [calendar API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1.0.</span></span>