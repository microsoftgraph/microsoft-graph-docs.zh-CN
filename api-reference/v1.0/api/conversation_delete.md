<span data-ttu-id="b10bf-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b10bf-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="b10bf-117">示例</span><span class="sxs-lookup"><span data-stu-id="b10bf-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b10bf-118">请求</span><span class="sxs-lookup"><span data-stu-id="b10bf-118">Request</span></span>
<span data-ttu-id="b10bf-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b10bf-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="b10bf-120">响应</span><span class="sxs-lookup"><span data-stu-id="b10bf-120">Response</span></span>
<span data-ttu-id="b10bf-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b10bf-121">Here is an example of the response.</span></span> 
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
