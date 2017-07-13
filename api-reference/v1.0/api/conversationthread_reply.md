<span data-ttu-id="9ec65-p104">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9ec65-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="9ec65-127">示例</span><span class="sxs-lookup"><span data-stu-id="9ec65-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="9ec65-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9ec65-128">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="9ec65-129">请求</span><span class="sxs-lookup"><span data-stu-id="9ec65-129">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="9ec65-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ec65-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <span data-ttu-id="9ec65-131">响应</span><span class="sxs-lookup"><span data-stu-id="9ec65-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="9ec65-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9ec65-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
