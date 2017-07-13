<span data-ttu-id="4df9f-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4df9f-p101">Bearer token. Required.</span></span>  | Bearer {token}。必需。 |

## <span data-ttu-id="4df9f-114">请求正文</span><span class="sxs-lookup"><span data-stu-id="4df9f-114">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="4df9f-115">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4df9f-115">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="4df9f-116">响应</span><span class="sxs-lookup"><span data-stu-id="4df9f-116">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4df9f-117">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4df9f-117">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="4df9f-118">示例</span><span class="sxs-lookup"><span data-stu-id="4df9f-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="4df9f-119">请求</span><span class="sxs-lookup"><span data-stu-id="4df9f-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="4df9f-120">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4df9f-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="4df9f-121">响应</span><span class="sxs-lookup"><span data-stu-id="4df9f-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4df9f-122">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4df9f-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
