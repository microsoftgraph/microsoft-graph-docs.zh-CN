<span data-ttu-id="9f229-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9f229-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="9f229-126">示例</span><span class="sxs-lookup"><span data-stu-id="9f229-126">Example</span></span>
<span data-ttu-id="9f229-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9f229-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9f229-128">请求</span><span class="sxs-lookup"><span data-stu-id="9f229-128">Request</span></span>
<span data-ttu-id="9f229-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f229-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="9f229-130">响应</span><span class="sxs-lookup"><span data-stu-id="9f229-130">Response</span></span>
<span data-ttu-id="9f229-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9f229-131">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->