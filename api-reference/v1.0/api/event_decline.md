<span data-ttu-id="dc31e-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dc31e-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="dc31e-135">示例</span><span class="sxs-lookup"><span data-stu-id="dc31e-135">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="dc31e-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dc31e-136">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="dc31e-137">请求</span><span class="sxs-lookup"><span data-stu-id="dc31e-137">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="dc31e-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc31e-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <span data-ttu-id="dc31e-139">响应</span><span class="sxs-lookup"><span data-stu-id="dc31e-139">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="dc31e-140">响应</span><span class="sxs-lookup"><span data-stu-id="dc31e-140">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="dc31e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dc31e-141">Here is an example of the response.</span></span>
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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
