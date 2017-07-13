<span data-ttu-id="ebb9a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebb9a-p102">Bearer token. Required.</span></span>  | Bearer {token}。必需。  |

## <span data-ttu-id="ebb9a-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebb9a-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="ebb9a-116">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="ebb9a-116">In the request body, supply the id of a user or group object.</span></span>


## <span data-ttu-id="ebb9a-117">响应</span><span class="sxs-lookup"><span data-stu-id="ebb9a-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ebb9a-118">此方法返回 `204, No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="ebb9a-118">This method returns `204, No Content` response code and no response body.</span></span>

## <span data-ttu-id="ebb9a-119">示例</span><span class="sxs-lookup"><span data-stu-id="ebb9a-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="ebb9a-120">请求</span><span class="sxs-lookup"><span data-stu-id="ebb9a-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="ebb9a-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebb9a-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <span data-ttu-id="ebb9a-122">响应</span><span class="sxs-lookup"><span data-stu-id="ebb9a-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ebb9a-123">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebb9a-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
