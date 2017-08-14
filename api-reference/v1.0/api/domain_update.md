<span data-ttu-id="61b08-p102">在请求正文中，提供要更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，仅包含已更改的值。</span><span class="sxs-lookup"><span data-stu-id="61b08-p102">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

在请求正文中，提供要更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，仅包含已更改的值。

## <a name="response"></a><span data-ttu-id="61b08-120">响应</span><span class="sxs-lookup"><span data-stu-id="61b08-120">Response</span></span>

<span data-ttu-id="61b08-121">如果成功，此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="61b08-121">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="61b08-122">示例</span><span class="sxs-lookup"><span data-stu-id="61b08-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61b08-123">请求</span><span class="sxs-lookup"><span data-stu-id="61b08-123">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="61b08-124">响应</span><span class="sxs-lookup"><span data-stu-id="61b08-124">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->