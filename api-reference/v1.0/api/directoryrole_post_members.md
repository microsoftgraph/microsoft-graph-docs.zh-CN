<span data-ttu-id="54c62-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54c62-p101">Bearer token. Required.</span></span>  | Bearer {token}。必需。 |
| <span data-ttu-id="54c62-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54c62-114">Content-Type</span></span>  | <span data-ttu-id="54c62-115">application/json</span><span class="sxs-lookup"><span data-stu-id="54c62-115">application/json</span></span>  |

## <span data-ttu-id="54c62-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="54c62-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="54c62-117">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54c62-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <span data-ttu-id="54c62-118">响应</span><span class="sxs-lookup"><span data-stu-id="54c62-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="54c62-119">如果成功，此方法返回 `204, No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="54c62-119">If successful, this method returns `204, No Content` response code.</span></span>

## <span data-ttu-id="54c62-120">示例</span><span class="sxs-lookup"><span data-stu-id="54c62-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="54c62-121">请求</span><span class="sxs-lookup"><span data-stu-id="54c62-121">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <span data-ttu-id="54c62-122">响应</span><span class="sxs-lookup"><span data-stu-id="54c62-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="54c62-123">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="54c62-123">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->