<span data-ttu-id="59596-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="59596-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a><span data-ttu-id="59596-123">示例</span><span class="sxs-lookup"><span data-stu-id="59596-123">Example</span></span>

##### <a name="request"></a><span data-ttu-id="59596-124">请求</span><span class="sxs-lookup"><span data-stu-id="59596-124">Request</span></span>

<span data-ttu-id="59596-125">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59596-125">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="59596-126">响应</span><span class="sxs-lookup"><span data-stu-id="59596-126">Response</span></span>

<span data-ttu-id="59596-127">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="59596-127">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="59596-128">注解</span><span class="sxs-lookup"><span data-stu-id="59596-128">Remarks</span></span>

* <span data-ttu-id="59596-129">具有 `personal`（OneDrive 个人版）**driveType** 的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="59596-129">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
