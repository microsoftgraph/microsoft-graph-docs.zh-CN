<span data-ttu-id="185e4-p103">**注意：**将项目移动到 OneDrive 的根目录下时不能使用 `"id:" "root"` 语法。需要使用根文件夹的真实 ID，或对父引用使用 `{"path": "/drive/root"}`。</span><span class="sxs-lookup"><span data-stu-id="185e4-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

**注意：**将项目移动到 OneDrive 的根目录下时不能使用 `"id:" "root"` 语法。需要使用根文件夹的真实 ID，或对父引用使用 `{"path": "/drive/root"}`。

## <span data-ttu-id="185e4-125">响应</span><span class="sxs-lookup"><span data-stu-id="185e4-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="185e4-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="185e4-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="185e4-127">示例</span><span class="sxs-lookup"><span data-stu-id="185e4-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="185e4-128">本示例将 {item-id} 指定的项目移动到用户 OneDrive 的**文档**文件夹中。</span><span class="sxs-lookup"><span data-stu-id="185e4-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

## <span data-ttu-id="185e4-129">响应</span><span class="sxs-lookup"><span data-stu-id="185e4-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="185e4-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="185e4-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
