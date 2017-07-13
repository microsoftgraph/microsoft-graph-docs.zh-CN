<span data-ttu-id="72b09-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="72b09-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="72b09-130">示例</span><span class="sxs-lookup"><span data-stu-id="72b09-130">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="72b09-131">请求</span><span class="sxs-lookup"><span data-stu-id="72b09-131">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="72b09-132">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="72b09-132">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <span data-ttu-id="72b09-133">响应</span><span class="sxs-lookup"><span data-stu-id="72b09-133">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="72b09-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="72b09-134">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
