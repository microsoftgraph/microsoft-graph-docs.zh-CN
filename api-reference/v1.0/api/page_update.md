<span data-ttu-id="e2316-p103">如果成功，此方法返回 `204 No Content` 响应代码。PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="e2316-p103">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
如果成功，此方法返回 `204 No Content` 响应代码。PATCH 请求未返回任何 JSON 数据。
## <span data-ttu-id="e2316-123">示例</span><span class="sxs-lookup"><span data-stu-id="e2316-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="e2316-124">请求</span><span class="sxs-lookup"><span data-stu-id="e2316-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e2316-125">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2316-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <span data-ttu-id="e2316-126">响应</span><span class="sxs-lookup"><span data-stu-id="e2316-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e2316-127">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2316-127">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
