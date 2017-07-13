<span data-ttu-id="98a48-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98a48-p101">Bearer token. Required.</span></span>  | Bearer {token}。必需。 |

## <span data-ttu-id="98a48-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="98a48-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="98a48-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98a48-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="98a48-119">响应</span><span class="sxs-lookup"><span data-stu-id="98a48-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="98a48-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98a48-120">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <span data-ttu-id="98a48-121">示例</span><span class="sxs-lookup"><span data-stu-id="98a48-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="98a48-122">请求</span><span class="sxs-lookup"><span data-stu-id="98a48-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="98a48-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98a48-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <span data-ttu-id="98a48-124">响应</span><span class="sxs-lookup"><span data-stu-id="98a48-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="98a48-125">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="98a48-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
