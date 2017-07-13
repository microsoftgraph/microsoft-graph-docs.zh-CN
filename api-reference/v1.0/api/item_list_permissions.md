<span data-ttu-id="67199-p103">调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="67199-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。

## <span data-ttu-id="67199-138">示例</span><span class="sxs-lookup"><span data-stu-id="67199-138">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="67199-139">请求</span><span class="sxs-lookup"><span data-stu-id="67199-139">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="67199-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67199-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <span data-ttu-id="67199-141">响应</span><span class="sxs-lookup"><span data-stu-id="67199-141">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="67199-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="67199-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

<span data-ttu-id="67199-143">有关检索单个权限资源的详细信息，请参阅 [获取权限](permission_get.md)。</span><span class="sxs-lookup"><span data-stu-id="67199-143">See [Get permission](permission_get.md) for more details on retrieving a single permission resource.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
