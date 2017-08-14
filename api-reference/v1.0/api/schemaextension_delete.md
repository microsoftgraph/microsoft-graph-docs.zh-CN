<span data-ttu-id="7c8c8-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c8c8-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="7c8c8-119">示例</span><span class="sxs-lookup"><span data-stu-id="7c8c8-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c8c8-120">请求</span><span class="sxs-lookup"><span data-stu-id="7c8c8-120">Request</span></span>
<span data-ttu-id="7c8c8-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c8c8-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="7c8c8-122">响应</span><span class="sxs-lookup"><span data-stu-id="7c8c8-122">Response</span></span>
<span data-ttu-id="7c8c8-123">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7c8c8-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="7c8c8-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7c8c8-124">See also</span></span>

- [<span data-ttu-id="7c8c8-125">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7c8c8-125">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="7c8c8-126">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7c8c8-126">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->