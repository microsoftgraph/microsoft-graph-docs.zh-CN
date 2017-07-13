<span data-ttu-id="f25d8-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f25d8-p101">Bearer token. Required.</span></span>  | Bearer {token}。必需。 |

## <span data-ttu-id="f25d8-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="f25d8-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="f25d8-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f25d8-116">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="f25d8-117">响应</span><span class="sxs-lookup"><span data-stu-id="f25d8-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f25d8-118">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和图像或文件二进制数据。</span><span class="sxs-lookup"><span data-stu-id="f25d8-118">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="f25d8-119">注意：图像无法直接在浏览器中呈现，因为与页面内容的其他部分一样，检索它们需要授权。</span><span class="sxs-lookup"><span data-stu-id="f25d8-119">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <span data-ttu-id="f25d8-120">示例</span><span class="sxs-lookup"><span data-stu-id="f25d8-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="f25d8-121">请求</span><span class="sxs-lookup"><span data-stu-id="f25d8-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="f25d8-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f25d8-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <span data-ttu-id="f25d8-123">响应</span><span class="sxs-lookup"><span data-stu-id="f25d8-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="f25d8-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f25d8-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
