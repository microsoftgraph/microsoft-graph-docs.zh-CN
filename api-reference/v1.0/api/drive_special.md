<span data-ttu-id="cc394-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc394-p103">Bearer {token}. Required.</span></span> | Bearer {token}。必需。 |


## <a name="request-body"></a><span data-ttu-id="cc394-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc394-128">Request body</span></span>
<span data-ttu-id="cc394-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc394-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc394-130">响应</span><span class="sxs-lookup"><span data-stu-id="cc394-130">Response</span></span>

<span data-ttu-id="cc394-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc394-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc394-132">示例</span><span class="sxs-lookup"><span data-stu-id="cc394-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cc394-133">请求</span><span class="sxs-lookup"><span data-stu-id="cc394-133">Request</span></span>
<span data-ttu-id="cc394-134">下面是一个请求用户驱动器的示例。</span><span class="sxs-lookup"><span data-stu-id="cc394-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="cc394-135">响应</span><span class="sxs-lookup"><span data-stu-id="cc394-135">Response</span></span>
<span data-ttu-id="cc394-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc394-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="cc394-137">注解</span><span class="sxs-lookup"><span data-stu-id="cc394-137">Remarks</span></span>

<span data-ttu-id="cc394-138">若要请求特殊文件夹的子文件夹，则可以请求 `children` 集合，或使用 [展开](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 选项展开子集合。</span><span class="sxs-lookup"><span data-stu-id="cc394-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
