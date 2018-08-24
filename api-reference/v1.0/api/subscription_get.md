# <a name="get-subscription"></a><span data-ttu-id="a7bca-101">获取订阅</span><span class="sxs-lookup"><span data-stu-id="a7bca-101">Get subscription</span></span>

<span data-ttu-id="a7bca-102">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7bca-102">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7bca-103">权限</span><span class="sxs-lookup"><span data-stu-id="a7bca-103">Permissions</span></span>

<span data-ttu-id="a7bca-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a7bca-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a7bca-106">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="a7bca-106">Resource type / Item</span></span>        | <span data-ttu-id="a7bca-107">权限</span><span class="sxs-lookup"><span data-stu-id="a7bca-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="a7bca-108">联系人</span><span class="sxs-lookup"><span data-stu-id="a7bca-108">Contacts</span></span>                    | <span data-ttu-id="a7bca-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a7bca-109">Contacts.Read</span></span>       |
| <span data-ttu-id="a7bca-110">对话</span><span class="sxs-lookup"><span data-stu-id="a7bca-110">Conversations</span></span>               | <span data-ttu-id="a7bca-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7bca-111">Group.Read.All</span></span>      |
| <span data-ttu-id="a7bca-112">事件</span><span class="sxs-lookup"><span data-stu-id="a7bca-112">Events</span></span>                      | <span data-ttu-id="a7bca-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a7bca-113">Calendars.Read</span></span>      |
| <span data-ttu-id="a7bca-114">消息</span><span class="sxs-lookup"><span data-stu-id="a7bca-114">Messages</span></span>                    | <span data-ttu-id="a7bca-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7bca-115">Mail.Read</span></span>           |
| <span data-ttu-id="a7bca-116">组</span><span class="sxs-lookup"><span data-stu-id="a7bca-116">Groups</span></span>                      | <span data-ttu-id="a7bca-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7bca-117">Group.Read.All</span></span>      |
| <span data-ttu-id="a7bca-118">用户</span><span class="sxs-lookup"><span data-stu-id="a7bca-118">Users</span></span>                       | <span data-ttu-id="a7bca-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7bca-119">User.Read.All</span></span>       |
| <span data-ttu-id="a7bca-120">驱动器（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="a7bca-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a7bca-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7bca-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a7bca-122">驱动器（SharePoint 共享的内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="a7bca-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="a7bca-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7bca-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7bca-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7bca-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7bca-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7bca-125">Optional query parameters</span></span>

<span data-ttu-id="a7bca-126">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7bca-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7bca-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7bca-127">Request headers</span></span>

| <span data-ttu-id="a7bca-128">名称</span><span class="sxs-lookup"><span data-stu-id="a7bca-128">Name</span></span>       | <span data-ttu-id="a7bca-129">类型</span><span class="sxs-lookup"><span data-stu-id="a7bca-129">Type</span></span> | <span data-ttu-id="a7bca-130">说明</span><span class="sxs-lookup"><span data-stu-id="a7bca-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7bca-131">授权</span><span class="sxs-lookup"><span data-stu-id="a7bca-131">Authorization</span></span>  | <span data-ttu-id="a7bca-132">字符串</span><span class="sxs-lookup"><span data-stu-id="a7bca-132">string</span></span>  | <span data-ttu-id="a7bca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7bca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7bca-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7bca-135">Request body</span></span>

<span data-ttu-id="a7bca-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7bca-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7bca-137">响应</span><span class="sxs-lookup"><span data-stu-id="a7bca-137">Response</span></span>

<span data-ttu-id="a7bca-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7bca-138">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7bca-139">示例</span><span class="sxs-lookup"><span data-stu-id="a7bca-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a7bca-140">请求</span><span class="sxs-lookup"><span data-stu-id="a7bca-140">Request</span></span>

<span data-ttu-id="a7bca-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7bca-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="a7bca-142">响应</span><span class="sxs-lookup"><span data-stu-id="a7bca-142">Response</span></span>

<span data-ttu-id="a7bca-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a7bca-143">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
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
