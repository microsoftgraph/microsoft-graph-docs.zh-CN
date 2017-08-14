<span data-ttu-id="8696b-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8696b-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="8696b-119">示例</span><span class="sxs-lookup"><span data-stu-id="8696b-119">Example</span></span>
<span data-ttu-id="8696b-120">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8696b-120">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8696b-121">请求</span><span class="sxs-lookup"><span data-stu-id="8696b-121">Request</span></span>
<span data-ttu-id="8696b-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8696b-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="8696b-123">响应</span><span class="sxs-lookup"><span data-stu-id="8696b-123">Response</span></span>
<span data-ttu-id="8696b-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8696b-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
