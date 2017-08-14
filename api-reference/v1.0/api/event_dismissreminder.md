<span data-ttu-id="d6d6c-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d6d6c-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="d6d6c-118">示例</span><span class="sxs-lookup"><span data-stu-id="d6d6c-118">Example</span></span>
<span data-ttu-id="d6d6c-119">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d6d6c-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d6d6c-120">请求</span><span class="sxs-lookup"><span data-stu-id="d6d6c-120">Request</span></span>
<span data-ttu-id="d6d6c-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6d6c-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

##### <a name="response"></a><span data-ttu-id="d6d6c-122">响应</span><span class="sxs-lookup"><span data-stu-id="d6d6c-122">Response</span></span>
##### <a name="response"></a><span data-ttu-id="d6d6c-123">响应</span><span class="sxs-lookup"><span data-stu-id="d6d6c-123">Response</span></span>
<span data-ttu-id="d6d6c-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d6d6c-124">Here is an example of the response.</span></span>
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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
