<span data-ttu-id="470d5-p107">架构扩展适用的支持扩展的 Microsoft Graph 类型集。仅允许增量更改。</span><span class="sxs-lookup"><span data-stu-id="470d5-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|架构扩展适用的支持扩展的 Microsoft Graph 类型集。仅允许增量更改。|

## <span data-ttu-id="470d5-142">响应</span><span class="sxs-lookup"><span data-stu-id="470d5-142">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="470d5-143">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="470d5-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <span data-ttu-id="470d5-144">示例</span><span class="sxs-lookup"><span data-stu-id="470d5-144">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="470d5-145">请求</span><span class="sxs-lookup"><span data-stu-id="470d5-145">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="470d5-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="470d5-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <span data-ttu-id="470d5-147">响应</span><span class="sxs-lookup"><span data-stu-id="470d5-147">Response</span></span>
<a id="response" class="xliff"></a>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="470d5-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="470d5-148">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="470d5-149">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="470d5-149">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="470d5-150">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="470d5-150">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->