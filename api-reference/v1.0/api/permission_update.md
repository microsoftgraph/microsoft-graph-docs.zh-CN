<span data-ttu-id="45279-p101">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="45279-p101">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| <span data-ttu-id="45279-120">属性</span><span class="sxs-lookup"><span data-stu-id="45279-120">Property</span></span>     | <span data-ttu-id="45279-121">类型</span><span class="sxs-lookup"><span data-stu-id="45279-121">Type</span></span>   | <span data-ttu-id="45279-122">说明</span><span class="sxs-lookup"><span data-stu-id="45279-122">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="45279-123">**角色**</span><span class="sxs-lookup"><span data-stu-id="45279-123">**roles**</span></span>    | <span data-ttu-id="45279-124">String</span><span class="sxs-lookup"><span data-stu-id="45279-124">String</span></span> | <span data-ttu-id="45279-125">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="45279-125">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="45279-126">响应</span><span class="sxs-lookup"><span data-stu-id="45279-126">Response</span></span>

<span data-ttu-id="45279-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45279-127">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45279-128">示例</span><span class="sxs-lookup"><span data-stu-id="45279-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="45279-129">请求</span><span class="sxs-lookup"><span data-stu-id="45279-129">Request</span></span>

<span data-ttu-id="45279-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45279-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="45279-131">响应</span><span class="sxs-lookup"><span data-stu-id="45279-131">Response</span></span>

<span data-ttu-id="45279-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="45279-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
