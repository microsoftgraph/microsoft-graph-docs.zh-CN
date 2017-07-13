<span data-ttu-id="4e90d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e90d-p102">Bearer token. Required.</span></span>  | Bearer {token}。必需。 |

## <span data-ttu-id="4e90d-117">响应</span><span class="sxs-lookup"><span data-stu-id="4e90d-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4e90d-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e90d-118">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="4e90d-119">示例</span><span class="sxs-lookup"><span data-stu-id="4e90d-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="4e90d-120">请求</span><span class="sxs-lookup"><span data-stu-id="4e90d-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="4e90d-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e90d-121">Here is an example of the request.</span></span>
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

##### <span data-ttu-id="4e90d-122">响应</span><span class="sxs-lookup"><span data-stu-id="4e90d-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4e90d-123">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e90d-123">Here is an example of the response.</span></span>
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
