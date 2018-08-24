# <a name="update-subscription"></a><span data-ttu-id="238bd-101">更新订阅</span><span class="sxs-lookup"><span data-stu-id="238bd-101">Update subscription</span></span>

<span data-ttu-id="238bd-102">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="238bd-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="238bd-103">超过资源类型确定的时间长度后订阅过期。</span><span class="sxs-lookup"><span data-stu-id="238bd-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="238bd-104">为了避免遗漏通知，应用程序应在订阅到期日之前续订订阅。</span><span class="sxs-lookup"><span data-stu-id="238bd-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="238bd-105">请参阅[订阅](../resources/subscription.md)，了解每个资源类型的最长订阅时间。</span><span class="sxs-lookup"><span data-stu-id="238bd-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="238bd-106">权限</span><span class="sxs-lookup"><span data-stu-id="238bd-106">Permissions</span></span>

<span data-ttu-id="238bd-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="238bd-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="238bd-109">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="238bd-109">Resource type / Item</span></span>        | <span data-ttu-id="238bd-110">权限</span><span class="sxs-lookup"><span data-stu-id="238bd-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="238bd-111">联系人</span><span class="sxs-lookup"><span data-stu-id="238bd-111">Contacts</span></span>                    | <span data-ttu-id="238bd-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="238bd-112">Contacts.Read</span></span>       |
| <span data-ttu-id="238bd-113">对话</span><span class="sxs-lookup"><span data-stu-id="238bd-113">Conversations</span></span>               | <span data-ttu-id="238bd-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="238bd-114">Group.Read.All</span></span>      |
| <span data-ttu-id="238bd-115">事件</span><span class="sxs-lookup"><span data-stu-id="238bd-115">Events</span></span>                      | <span data-ttu-id="238bd-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="238bd-116">Calendars.Read</span></span>      |
| <span data-ttu-id="238bd-117">消息</span><span class="sxs-lookup"><span data-stu-id="238bd-117">Messages</span></span>                    | <span data-ttu-id="238bd-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="238bd-118">Mail.Read</span></span>           |
| <span data-ttu-id="238bd-119">组</span><span class="sxs-lookup"><span data-stu-id="238bd-119">Groups</span></span>                      | <span data-ttu-id="238bd-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="238bd-120">Group.Read.All</span></span>      |
| <span data-ttu-id="238bd-121">用户</span><span class="sxs-lookup"><span data-stu-id="238bd-121">Users</span></span>                       | <span data-ttu-id="238bd-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="238bd-122">User.Read.All</span></span>       |
| <span data-ttu-id="238bd-123">驱动器（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="238bd-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="238bd-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="238bd-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="238bd-125">驱动器（SharePoint 共享的内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="238bd-125">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="238bd-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238bd-126">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="238bd-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="238bd-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="238bd-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="238bd-128">Request headers</span></span>

| <span data-ttu-id="238bd-129">名称</span><span class="sxs-lookup"><span data-stu-id="238bd-129">Name</span></span>       | <span data-ttu-id="238bd-130">类型</span><span class="sxs-lookup"><span data-stu-id="238bd-130">Type</span></span> | <span data-ttu-id="238bd-131">说明</span><span class="sxs-lookup"><span data-stu-id="238bd-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="238bd-132">授权</span><span class="sxs-lookup"><span data-stu-id="238bd-132">Authorization</span></span>  | <span data-ttu-id="238bd-133">字符串</span><span class="sxs-lookup"><span data-stu-id="238bd-133">string</span></span>  | <span data-ttu-id="238bd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="238bd-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="238bd-136">响应</span><span class="sxs-lookup"><span data-stu-id="238bd-136">Response</span></span>

<span data-ttu-id="238bd-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="238bd-137">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="238bd-138">示例</span><span class="sxs-lookup"><span data-stu-id="238bd-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="238bd-139">请求</span><span class="sxs-lookup"><span data-stu-id="238bd-139">Request</span></span>

<span data-ttu-id="238bd-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="238bd-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="238bd-141">响应</span><span class="sxs-lookup"><span data-stu-id="238bd-141">Response</span></span>

<span data-ttu-id="238bd-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="238bd-142">Here is an example of the response.</span></span>
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
