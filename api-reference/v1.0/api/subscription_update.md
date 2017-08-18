# <a name="update-subscription"></a><span data-ttu-id="20bdc-101">更新订阅</span><span class="sxs-lookup"><span data-stu-id="20bdc-101">Update subscription</span></span>

<span data-ttu-id="20bdc-102">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="20bdc-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="20bdc-p101">单个资源类型的禁止日期即为资源订阅的到期日期。应该在到期日期之前准时续订订阅，以免错过通知。请参阅 [订阅](../resources/subscription.md) 了解各到期日期。</span><span class="sxs-lookup"><span data-stu-id="20bdc-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20bdc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="20bdc-106">Prerequisites</span></span>

<span data-ttu-id="20bdc-107">下表列出了对各个资源所需权限的建议。</span><span class="sxs-lookup"><span data-stu-id="20bdc-107">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="20bdc-108">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="20bdc-108">Resource type / Item</span></span>        | <span data-ttu-id="20bdc-109">范围</span><span class="sxs-lookup"><span data-stu-id="20bdc-109">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="20bdc-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="20bdc-110">Contacts</span></span>                    | <span data-ttu-id="20bdc-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="20bdc-111">Contacts.Read</span></span>       |
| <span data-ttu-id="20bdc-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="20bdc-112">Conversations</span></span>               | <span data-ttu-id="20bdc-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="20bdc-113">Group.Read.All</span></span>      |
| <span data-ttu-id="20bdc-114">Events</span><span class="sxs-lookup"><span data-stu-id="20bdc-114">Events</span></span>                      | <span data-ttu-id="20bdc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20bdc-115">Calendars.Read</span></span>      |
| <span data-ttu-id="20bdc-116">Messages</span><span class="sxs-lookup"><span data-stu-id="20bdc-116">Messages</span></span>                    | <span data-ttu-id="20bdc-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20bdc-117">Mail.Read</span></span>           |
| <span data-ttu-id="20bdc-118">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="20bdc-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="20bdc-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20bdc-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="20bdc-120">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="20bdc-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="20bdc-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20bdc-121">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20bdc-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20bdc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="20bdc-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="20bdc-123">Request headers</span></span>
| <span data-ttu-id="20bdc-124">名称</span><span class="sxs-lookup"><span data-stu-id="20bdc-124">Name</span></span>       | <span data-ttu-id="20bdc-125">类型</span><span class="sxs-lookup"><span data-stu-id="20bdc-125">Type</span></span> | <span data-ttu-id="20bdc-126">说明</span><span class="sxs-lookup"><span data-stu-id="20bdc-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20bdc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="20bdc-127">Authorization</span></span>  | <span data-ttu-id="20bdc-128">string</span><span class="sxs-lookup"><span data-stu-id="20bdc-128">string</span></span>  | <span data-ttu-id="20bdc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20bdc-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="20bdc-131">响应</span><span class="sxs-lookup"><span data-stu-id="20bdc-131">Response</span></span>

<span data-ttu-id="20bdc-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20bdc-132">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20bdc-133">示例</span><span class="sxs-lookup"><span data-stu-id="20bdc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20bdc-134">请求</span><span class="sxs-lookup"><span data-stu-id="20bdc-134">Request</span></span>
<span data-ttu-id="20bdc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20bdc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="20bdc-136">响应</span><span class="sxs-lookup"><span data-stu-id="20bdc-136">Response</span></span>
<span data-ttu-id="20bdc-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="20bdc-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
