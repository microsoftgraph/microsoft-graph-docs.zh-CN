# <a name="update-subscription"></a><span data-ttu-id="6ccf4-101">更新订阅</span><span class="sxs-lookup"><span data-stu-id="6ccf4-101">Update subscription</span></span>

<span data-ttu-id="6ccf4-102">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6ccf4-103">订阅过期后一个随资源类型的时间长度。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6ccf4-104">为了避免丢失通知，应用程序应更新其订阅之前其到期日期。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6ccf4-105">请参阅最大长度为每个资源类型订阅的[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ccf4-106">权限</span><span class="sxs-lookup"><span data-stu-id="6ccf4-106">Permissions</span></span>

<span data-ttu-id="6ccf4-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6ccf4-109">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="6ccf4-109">Resource type / Item</span></span>        | <span data-ttu-id="6ccf4-110">权限</span><span class="sxs-lookup"><span data-stu-id="6ccf4-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6ccf4-111">联系人</span><span class="sxs-lookup"><span data-stu-id="6ccf4-111">Contacts</span></span>                    | <span data-ttu-id="6ccf4-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6ccf4-112">Contacts.Read</span></span>       |
| <span data-ttu-id="6ccf4-113">Conversations</span><span class="sxs-lookup"><span data-stu-id="6ccf4-113">Conversations</span></span>               | <span data-ttu-id="6ccf4-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ccf4-114">Group.Read.All</span></span>      |
| <span data-ttu-id="6ccf4-115">Events</span><span class="sxs-lookup"><span data-stu-id="6ccf4-115">Events</span></span>                      | <span data-ttu-id="6ccf4-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6ccf4-116">Calendars.Read</span></span>      |
| <span data-ttu-id="6ccf4-117">Messages</span><span class="sxs-lookup"><span data-stu-id="6ccf4-117">Messages</span></span>                    | <span data-ttu-id="6ccf4-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6ccf4-118">Mail.Read</span></span>           |
| <span data-ttu-id="6ccf4-119">Groups</span><span class="sxs-lookup"><span data-stu-id="6ccf4-119">Groups</span></span>                      | <span data-ttu-id="6ccf4-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ccf4-120">Group.Read.All</span></span>      |
| <span data-ttu-id="6ccf4-121">Users</span><span class="sxs-lookup"><span data-stu-id="6ccf4-121">Users</span></span>                       | <span data-ttu-id="6ccf4-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ccf4-122">User.Read.All</span></span>       |
| <span data-ttu-id="6ccf4-123">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="6ccf4-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6ccf4-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ccf4-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6ccf4-125">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="6ccf4-125">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="6ccf4-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ccf4-126">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="6ccf4-127">安全警报</span><span class="sxs-lookup"><span data-stu-id="6ccf4-127">Security alert</span></span>| <span data-ttu-id="6ccf4-128">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ccf4-128">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ccf4-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ccf4-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6ccf4-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ccf4-130">Request headers</span></span>

| <span data-ttu-id="6ccf4-131">名称</span><span class="sxs-lookup"><span data-stu-id="6ccf4-131">Name</span></span>       | <span data-ttu-id="6ccf4-132">类型</span><span class="sxs-lookup"><span data-stu-id="6ccf4-132">Type</span></span> | <span data-ttu-id="6ccf4-133">说明</span><span class="sxs-lookup"><span data-stu-id="6ccf4-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ccf4-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ccf4-134">Authorization</span></span>  | <span data-ttu-id="6ccf4-135">string</span><span class="sxs-lookup"><span data-stu-id="6ccf4-135">string</span></span>  | <span data-ttu-id="6ccf4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6ccf4-138">响应</span><span class="sxs-lookup"><span data-stu-id="6ccf4-138">Response</span></span>

<span data-ttu-id="6ccf4-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-139">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ccf4-140">示例</span><span class="sxs-lookup"><span data-stu-id="6ccf4-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6ccf4-141">请求</span><span class="sxs-lookup"><span data-stu-id="6ccf4-141">Request</span></span>

<span data-ttu-id="6ccf4-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="6ccf4-143">响应</span><span class="sxs-lookup"><span data-stu-id="6ccf4-143">Response</span></span>

<span data-ttu-id="6ccf4-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6ccf4-144">Here is an example of the response.</span></span>
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
