# <a name="get-subscription"></a><span data-ttu-id="d37f8-101">获取订阅</span><span class="sxs-lookup"><span data-stu-id="d37f8-101">Get subscription</span></span>

<span data-ttu-id="d37f8-102">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d37f8-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d37f8-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="d37f8-103">Prerequisites</span></span>

<span data-ttu-id="d37f8-104">下表列出了对各个资源所需权限的建议。</span><span class="sxs-lookup"><span data-stu-id="d37f8-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="d37f8-105">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="d37f8-105">Resource type / Item</span></span>        | <span data-ttu-id="d37f8-106">范围</span><span class="sxs-lookup"><span data-stu-id="d37f8-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="d37f8-107">Contacts</span><span class="sxs-lookup"><span data-stu-id="d37f8-107">Contacts</span></span>                    | <span data-ttu-id="d37f8-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d37f8-108">Contacts.Read</span></span>       |
| <span data-ttu-id="d37f8-109">Conversations</span><span class="sxs-lookup"><span data-stu-id="d37f8-109">Conversations</span></span>               | <span data-ttu-id="d37f8-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d37f8-110">Group.Read.All</span></span>      |
| <span data-ttu-id="d37f8-111">Events</span><span class="sxs-lookup"><span data-stu-id="d37f8-111">Events</span></span>                      | <span data-ttu-id="d37f8-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d37f8-112">Calendars.Read</span></span>      |
| <span data-ttu-id="d37f8-113">Messages</span><span class="sxs-lookup"><span data-stu-id="d37f8-113">Messages</span></span>                    | <span data-ttu-id="d37f8-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d37f8-114">Mail.Read</span></span>           |
| <span data-ttu-id="d37f8-115">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d37f8-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d37f8-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d37f8-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d37f8-117">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="d37f8-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="d37f8-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37f8-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d37f8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d37f8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d37f8-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d37f8-120">Optional query parameters</span></span>
<span data-ttu-id="d37f8-121">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d37f8-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d37f8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d37f8-122">Request headers</span></span>
| <span data-ttu-id="d37f8-123">名称</span><span class="sxs-lookup"><span data-stu-id="d37f8-123">Name</span></span>       | <span data-ttu-id="d37f8-124">类型</span><span class="sxs-lookup"><span data-stu-id="d37f8-124">Type</span></span> | <span data-ttu-id="d37f8-125">说明</span><span class="sxs-lookup"><span data-stu-id="d37f8-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d37f8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d37f8-126">Authorization</span></span>  | <span data-ttu-id="d37f8-127">string</span><span class="sxs-lookup"><span data-stu-id="d37f8-127">string</span></span>  | <span data-ttu-id="d37f8-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d37f8-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d37f8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d37f8-130">Request body</span></span>
<span data-ttu-id="d37f8-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d37f8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d37f8-132">响应</span><span class="sxs-lookup"><span data-stu-id="d37f8-132">Response</span></span>

<span data-ttu-id="d37f8-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d37f8-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d37f8-134">示例</span><span class="sxs-lookup"><span data-stu-id="d37f8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d37f8-135">请求</span><span class="sxs-lookup"><span data-stu-id="d37f8-135">Request</span></span>
<span data-ttu-id="d37f8-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d37f8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="d37f8-137">响应</span><span class="sxs-lookup"><span data-stu-id="d37f8-137">Response</span></span>
<span data-ttu-id="d37f8-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d37f8-138">Here is an example of the response.</span></span>
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
