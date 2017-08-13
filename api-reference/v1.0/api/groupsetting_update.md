<span data-ttu-id="c6278-p102">更新的值集。注意：必须提供整个集合组。无法更新单个值集合。</span><span class="sxs-lookup"><span data-stu-id="c6278-p102">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> | 更新的值集。注意：必须提供整个集合组。无法更新单个值集合。 |

## <a name="response"></a><span data-ttu-id="c6278-126">响应</span><span class="sxs-lookup"><span data-stu-id="c6278-126">Response</span></span>

<span data-ttu-id="c6278-127">如果成功，此方法在响应正文中返回 `204 OK` 响应代码和更新的 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6278-127">If successful, this method returns a `204 OK` response code and [directoryObject](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6278-128">示例</span><span class="sxs-lookup"><span data-stu-id="c6278-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6278-129">请求</span><span class="sxs-lookup"><span data-stu-id="c6278-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="c6278-130">响应</span><span class="sxs-lookup"><span data-stu-id="c6278-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->