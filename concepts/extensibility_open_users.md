<span data-ttu-id="0bd84-p107">用户决定不再使用漫游配置文件，因此将其删除。这可以通过开放扩展值上的 ```DELETE``` 请求完成。</span><span class="sxs-lookup"><span data-stu-id="0bd84-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>
用户决定不再使用漫游配置文件，因此将其删除。这可以通过开放扩展值上的 ```DELETE``` 请求完成。

##### <a name="request"></a><span data-ttu-id="0bd84-135">请求</span><span class="sxs-lookup"><span data-stu-id="0bd84-135">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="0bd84-136">响应</span><span class="sxs-lookup"><span data-stu-id="0bd84-136">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="0bd84-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0bd84-137">See also</span></span>

- [<span data-ttu-id="0bd84-138">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0bd84-138">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="0bd84-139">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0bd84-139">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)
- [<span data-ttu-id="0bd84-140">openTypeExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bd84-140">openTypeExtension resource type</span></span>](../api-reference/v1.0/resources/opentypeextension.md)
- [<span data-ttu-id="0bd84-141">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="0bd84-141">Create open extension</span></span>](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)
- [<span data-ttu-id="0bd84-142">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="0bd84-142">Get open extension</span></span>](../api-reference/v1.0/api/opentypeextension_get.md)
- [<span data-ttu-id="0bd84-143">更新开放扩展</span><span class="sxs-lookup"><span data-stu-id="0bd84-143">Update open extension</span></span>](../api-reference/v1.0/api/opentypeextension_update.md)
- [<span data-ttu-id="0bd84-144">删除开放扩展</span><span class="sxs-lookup"><span data-stu-id="0bd84-144">Delete open extension</span></span>](../api-reference/v1.0/api/opentypeextension_delete.md)