<span data-ttu-id="cf745-p109">下面的示例查找了具有 `graphlearn_courses` 扩展且 `courseId` 属性值与 `123` 相匹配的组，获取了组属性 **displayName**、 **id** 和 **description**，以及 `graphlearn_courses` 扩展中的自定义数据。（在实际查询中，请确保根据需要应用 URL 编码。）</span><span class="sxs-lookup"><span data-stu-id="cf745-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

下面的示例查找了具有 `graphlearn_courses` 扩展且 `courseId` 属性值与 `123` 相匹配的组，获取了组属性 **displayName**、 **id** 和 **description**，以及 `graphlearn_courses` 扩展中的自定义数据。（在实际查询中，请确保根据需要应用 URL 编码。）

#### <span data-ttu-id="cf745-157">请求</span><span class="sxs-lookup"><span data-stu-id="cf745-157">Request</span></span>
<a id="request" class="xliff"></a>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <span data-ttu-id="cf745-158">响应</span><span class="sxs-lookup"><span data-stu-id="cf745-158">Response</span></span>
<a id="response" class="xliff"></a>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <span data-ttu-id="cf745-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cf745-159">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="cf745-160">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="cf745-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="cf745-161">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="cf745-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- <span data-ttu-id="cf745-162">
  [Office 365 域](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="cf745-162">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>
- [<span data-ttu-id="cf745-163">添加并验证新 Office 365 的域</span><span class="sxs-lookup"><span data-stu-id="cf745-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="cf745-164">schemaExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf745-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="cf745-165">列出 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cf745-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="cf745-166">创建 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cf745-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="cf745-167">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cf745-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="cf745-168">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cf745-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="cf745-169">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="cf745-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)
