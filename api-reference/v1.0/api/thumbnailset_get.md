<span data-ttu-id="429e2-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="429e2-p101">Bearer {token}. Required.</span></span>  | Bearer {token}。必需。 |


## <a name="request-body"></a><span data-ttu-id="429e2-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="429e2-118">Request body</span></span>
<span data-ttu-id="429e2-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="429e2-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="429e2-120">响应</span><span class="sxs-lookup"><span data-stu-id="429e2-120">Response</span></span>

<span data-ttu-id="429e2-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thumbnailSet](../resources/thumbnailset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="429e2-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="429e2-122">示例</span><span class="sxs-lookup"><span data-stu-id="429e2-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="429e2-123">请求</span><span class="sxs-lookup"><span data-stu-id="429e2-123">Request</span></span>
<span data-ttu-id="429e2-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="429e2-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="429e2-125">响应</span><span class="sxs-lookup"><span data-stu-id="429e2-125">Response</span></span>
<span data-ttu-id="429e2-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="429e2-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
