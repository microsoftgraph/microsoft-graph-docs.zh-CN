<span data-ttu-id="eb079-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb079-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="eb079-117">示例</span><span class="sxs-lookup"><span data-stu-id="eb079-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb079-118">请求</span><span class="sxs-lookup"><span data-stu-id="eb079-118">Request</span></span>
<span data-ttu-id="eb079-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb079-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/mba9a3254-9f18-4209-aeb3-9e42a35b5be4
```
##### <a name="response"></a><span data-ttu-id="eb079-120">响应</span><span class="sxs-lookup"><span data-stu-id="eb079-120">Response</span></span>
<span data-ttu-id="eb079-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb079-121">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->