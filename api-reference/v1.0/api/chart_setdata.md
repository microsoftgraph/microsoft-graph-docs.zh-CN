<span data-ttu-id="e0072-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0072-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="e0072-130">示例</span><span class="sxs-lookup"><span data-stu-id="e0072-130">Example</span></span>
<span data-ttu-id="e0072-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0072-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0072-132">请求</span><span class="sxs-lookup"><span data-stu-id="e0072-132">Request</span></span>
<span data-ttu-id="e0072-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0072-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="e0072-134">响应</span><span class="sxs-lookup"><span data-stu-id="e0072-134">Response</span></span>
<span data-ttu-id="e0072-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0072-135">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->