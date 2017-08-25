# <a name="update-subscription"></a><span data-ttu-id="05c4b-101">更新订阅</span><span class="sxs-lookup"><span data-stu-id="05c4b-101">Update subscription</span></span>

<span data-ttu-id="05c4b-102">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="05c4b-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="05c4b-p101">单个资源类型的禁止日期即为资源订阅的到期日期。应该在到期日期之前准时续订订阅，以免错过通知。请参阅 [订阅](../resources/subscription.md) 了解各到期日期。</span><span class="sxs-lookup"><span data-stu-id="05c4b-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="permissions"></a><span data-ttu-id="05c4b-106">权限</span><span class="sxs-lookup"><span data-stu-id="05c4b-106">Permissions</span></span>

<span data-ttu-id="05c4b-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="05c4b-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="05c4b-109">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="05c4b-109">Resource type / Item</span></span>        | <span data-ttu-id="05c4b-110">权限</span><span class="sxs-lookup"><span data-stu-id="05c4b-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="05c4b-111">联系人</span><span class="sxs-lookup"><span data-stu-id="05c4b-111">Contacts</span></span>                    | <span data-ttu-id="05c4b-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="05c4b-112">Contacts.Read</span></span>       |
| <span data-ttu-id="05c4b-113">Conversations</span><span class="sxs-lookup"><span data-stu-id="05c4b-113">Conversations</span></span>               | <span data-ttu-id="05c4b-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05c4b-114">Group.Read.All</span></span>      |
| <span data-ttu-id="05c4b-115">Events</span><span class="sxs-lookup"><span data-stu-id="05c4b-115">Events</span></span>                      | <span data-ttu-id="05c4b-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="05c4b-116">Calendars.Read</span></span>      |
| <span data-ttu-id="05c4b-117">Messages</span><span class="sxs-lookup"><span data-stu-id="05c4b-117">Messages</span></span>                    | <span data-ttu-id="05c4b-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="05c4b-118">Mail.Read</span></span>           |
| <span data-ttu-id="05c4b-119">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="05c4b-119">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="05c4b-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05c4b-120">Files.ReadWrite</span></span>     |
| <span data-ttu-id="05c4b-121">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="05c4b-121">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="05c4b-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c4b-122">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05c4b-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05c4b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="05c4b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="05c4b-124">Request headers</span></span>
| <span data-ttu-id="05c4b-125">名称</span><span class="sxs-lookup"><span data-stu-id="05c4b-125">Name</span></span>       | <span data-ttu-id="05c4b-126">类型</span><span class="sxs-lookup"><span data-stu-id="05c4b-126">Type</span></span> | <span data-ttu-id="05c4b-127">说明</span><span class="sxs-lookup"><span data-stu-id="05c4b-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="05c4b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="05c4b-128">Authorization</span></span>  | <span data-ttu-id="05c4b-129">string</span><span class="sxs-lookup"><span data-stu-id="05c4b-129">string</span></span>  | <span data-ttu-id="05c4b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05c4b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="05c4b-132">响应</span><span class="sxs-lookup"><span data-stu-id="05c4b-132">Response</span></span>

<span data-ttu-id="05c4b-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05c4b-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05c4b-134">示例</span><span class="sxs-lookup"><span data-stu-id="05c4b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05c4b-135">请求</span><span class="sxs-lookup"><span data-stu-id="05c4b-135">Request</span></span>
<span data-ttu-id="05c4b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05c4b-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="05c4b-137">响应</span><span class="sxs-lookup"><span data-stu-id="05c4b-137">Response</span></span>
<span data-ttu-id="05c4b-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="05c4b-138">Here is an example of the response.</span></span>
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
