<span data-ttu-id="a3afb-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a3afb-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

### <span data-ttu-id="a3afb-119">示例</span><span class="sxs-lookup"><span data-stu-id="a3afb-119">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="a3afb-120">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a3afb-120">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="a3afb-121">请求</span><span class="sxs-lookup"><span data-stu-id="a3afb-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="a3afb-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3afb-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <span data-ttu-id="a3afb-123">响应</span><span class="sxs-lookup"><span data-stu-id="a3afb-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a3afb-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a3afb-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
