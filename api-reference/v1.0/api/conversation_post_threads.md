<span data-ttu-id="c0a65-p103">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和新线程的 `id`。下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0a65-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>

如果成功，此方法在响应正文中返回 `201, Created` 响应代码和新线程的 `id`。下面是一个响应示例。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
