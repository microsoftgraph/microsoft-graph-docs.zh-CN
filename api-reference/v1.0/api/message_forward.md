<span data-ttu-id="fc07a-p105">如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fc07a-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `202, Accepted` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="fc07a-134">示例</span><span class="sxs-lookup"><span data-stu-id="fc07a-134">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="fc07a-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc07a-135">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="fc07a-136">请求</span><span class="sxs-lookup"><span data-stu-id="fc07a-136">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="fc07a-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc07a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <span data-ttu-id="fc07a-138">响应</span><span class="sxs-lookup"><span data-stu-id="fc07a-138">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="fc07a-139">响应</span><span class="sxs-lookup"><span data-stu-id="fc07a-139">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="fc07a-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fc07a-140">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
