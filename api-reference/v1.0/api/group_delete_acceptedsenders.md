<span data-ttu-id="17fcc-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="17fcc-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="17fcc-117">示例</span><span class="sxs-lookup"><span data-stu-id="17fcc-117">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="17fcc-118">请求</span><span class="sxs-lookup"><span data-stu-id="17fcc-118">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="17fcc-119">下面是几个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17fcc-119">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id="users/{id}"

DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id="groups/{id}"
```

##### <span data-ttu-id="17fcc-120">响应</span><span class="sxs-lookup"><span data-stu-id="17fcc-120">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="17fcc-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="17fcc-121">Here is an example of the response.</span></span> 
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