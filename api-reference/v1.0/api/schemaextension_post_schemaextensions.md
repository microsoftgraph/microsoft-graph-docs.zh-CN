<span data-ttu-id="d09c4-p108">该响应包括一个基于请求中提供的架构名称的 **id** 属性中唯一的字符串，以及新创建的架构定义的其余部分。响应中的 **id** 中的值采用此格式：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d09c4-p108">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

该响应包括一个基于请求中提供的架构名称的 **id** 属性中唯一的字符串，以及新创建的架构定义的其余部分。响应中的 **id** 中的值采用此格式：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="d09c4-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d09c4-161">See also</span></span>

- [<span data-ttu-id="d09c4-162">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d09c4-162">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d09c4-163">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d09c4-163">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->