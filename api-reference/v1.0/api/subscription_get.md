# <a name="get-subscription"></a><span data-ttu-id="b25c0-101">获取订阅</span><span class="sxs-lookup"><span data-stu-id="b25c0-101">Get subscription</span></span>

<span data-ttu-id="b25c0-102">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b25c0-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="permissions"></a><span data-ttu-id="b25c0-103">权限</span><span class="sxs-lookup"><span data-stu-id="b25c0-103">Permissions</span></span>

<span data-ttu-id="b25c0-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b25c0-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b25c0-106">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="b25c0-106">Resource type / Item</span></span>        | <span data-ttu-id="b25c0-107">权限</span><span class="sxs-lookup"><span data-stu-id="b25c0-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b25c0-108">联系人</span><span class="sxs-lookup"><span data-stu-id="b25c0-108">Contacts</span></span>                    | <span data-ttu-id="b25c0-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b25c0-109">Contacts.Read</span></span>       |
| <span data-ttu-id="b25c0-110">Conversations</span><span class="sxs-lookup"><span data-stu-id="b25c0-110">Conversations</span></span>               | <span data-ttu-id="b25c0-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b25c0-111">Group.Read.All</span></span>      |
| <span data-ttu-id="b25c0-112">Events</span><span class="sxs-lookup"><span data-stu-id="b25c0-112">Events</span></span>                      | <span data-ttu-id="b25c0-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b25c0-113">Calendars.Read</span></span>      |
| <span data-ttu-id="b25c0-114">Messages</span><span class="sxs-lookup"><span data-stu-id="b25c0-114">Messages</span></span>                    | <span data-ttu-id="b25c0-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b25c0-115">Mail.Read</span></span>           |
| <span data-ttu-id="b25c0-116">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="b25c0-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b25c0-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b25c0-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b25c0-118">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="b25c0-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="b25c0-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b25c0-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b25c0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b25c0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b25c0-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b25c0-121">Optional query parameters</span></span>
<span data-ttu-id="b25c0-122">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b25c0-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b25c0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b25c0-123">Request headers</span></span>
| <span data-ttu-id="b25c0-124">名称</span><span class="sxs-lookup"><span data-stu-id="b25c0-124">Name</span></span>       | <span data-ttu-id="b25c0-125">类型</span><span class="sxs-lookup"><span data-stu-id="b25c0-125">Type</span></span> | <span data-ttu-id="b25c0-126">说明</span><span class="sxs-lookup"><span data-stu-id="b25c0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b25c0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b25c0-127">Authorization</span></span>  | <span data-ttu-id="b25c0-128">string</span><span class="sxs-lookup"><span data-stu-id="b25c0-128">string</span></span>  | <span data-ttu-id="b25c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b25c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b25c0-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b25c0-131">Request body</span></span>
<span data-ttu-id="b25c0-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b25c0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b25c0-133">响应</span><span class="sxs-lookup"><span data-stu-id="b25c0-133">Response</span></span>

<span data-ttu-id="b25c0-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b25c0-134">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b25c0-135">示例</span><span class="sxs-lookup"><span data-stu-id="b25c0-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b25c0-136">请求</span><span class="sxs-lookup"><span data-stu-id="b25c0-136">Request</span></span>
<span data-ttu-id="b25c0-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b25c0-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="b25c0-138">响应</span><span class="sxs-lookup"><span data-stu-id="b25c0-138">Response</span></span>
<span data-ttu-id="b25c0-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b25c0-139">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
