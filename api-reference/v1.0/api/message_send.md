<span data-ttu-id="b1f0b-p103">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b1f0b-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="b1f0b-120">示例</span><span class="sxs-lookup"><span data-stu-id="b1f0b-120">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="b1f0b-121">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b1f0b-121">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="b1f0b-122">请求</span><span class="sxs-lookup"><span data-stu-id="b1f0b-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="b1f0b-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1f0b-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <span data-ttu-id="b1f0b-124">响应</span><span class="sxs-lookup"><span data-stu-id="b1f0b-124">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="b1f0b-125">响应</span><span class="sxs-lookup"><span data-stu-id="b1f0b-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b1f0b-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b1f0b-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
