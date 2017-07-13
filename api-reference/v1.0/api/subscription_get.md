<span data-ttu-id="af39d-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af39d-p101">Bearer token. Required.</span></span>  | Bearer {token}。必需。 |

## <span data-ttu-id="af39d-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="af39d-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="af39d-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af39d-117">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="af39d-118">响应</span><span class="sxs-lookup"><span data-stu-id="af39d-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="af39d-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af39d-119">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="af39d-120">示例</span><span class="sxs-lookup"><span data-stu-id="af39d-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="af39d-121">请求</span><span class="sxs-lookup"><span data-stu-id="af39d-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="af39d-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af39d-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="af39d-123">响应</span><span class="sxs-lookup"><span data-stu-id="af39d-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="af39d-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="af39d-124">Here is an example of the response.</span></span>
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
