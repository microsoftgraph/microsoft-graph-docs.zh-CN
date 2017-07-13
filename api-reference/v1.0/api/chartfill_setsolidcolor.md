<span data-ttu-id="55a18-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="55a18-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

## <span data-ttu-id="55a18-124">示例</span><span class="sxs-lookup"><span data-stu-id="55a18-124">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="55a18-125">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="55a18-125">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="55a18-126">请求</span><span class="sxs-lookup"><span data-stu-id="55a18-126">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="55a18-127">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55a18-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <span data-ttu-id="55a18-128">响应</span><span class="sxs-lookup"><span data-stu-id="55a18-128">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="55a18-129">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55a18-129">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->