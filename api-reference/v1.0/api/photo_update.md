<span data-ttu-id="db90b-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="db90b-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| <span data-ttu-id="db90b-118">属性</span><span class="sxs-lookup"><span data-stu-id="db90b-118">Property</span></span>     | <span data-ttu-id="db90b-119">类型</span><span class="sxs-lookup"><span data-stu-id="db90b-119">Type</span></span>   |<span data-ttu-id="db90b-120">说明</span><span class="sxs-lookup"><span data-stu-id="db90b-120">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="db90b-121">响应</span><span class="sxs-lookup"><span data-stu-id="db90b-121">Response</span></span>

<span data-ttu-id="db90b-122">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db90b-122">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db90b-123">示例</span><span class="sxs-lookup"><span data-stu-id="db90b-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db90b-124">请求</span><span class="sxs-lookup"><span data-stu-id="db90b-124">Request</span></span>
<span data-ttu-id="db90b-125">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db90b-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="db90b-126">响应</span><span class="sxs-lookup"><span data-stu-id="db90b-126">Response</span></span>
<span data-ttu-id="db90b-127">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="db90b-127">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
