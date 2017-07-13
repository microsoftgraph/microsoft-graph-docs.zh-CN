<span data-ttu-id="7d51e-p110">只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes)。</span><span class="sxs-lookup"><span data-stu-id="7d51e-p110">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
- 只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅[已知问题](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes)。

## <span data-ttu-id="7d51e-162">响应</span><span class="sxs-lookup"><span data-stu-id="7d51e-162">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="7d51e-163">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7d51e-163">If successful, this method returns a `204 No Content` response code.</span></span>

## <span data-ttu-id="7d51e-164">示例</span><span class="sxs-lookup"><span data-stu-id="7d51e-164">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="7d51e-165">请求</span><span class="sxs-lookup"><span data-stu-id="7d51e-165">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "update_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```

##### <span data-ttu-id="7d51e-166">响应</span><span class="sxs-lookup"><span data-stu-id="7d51e-166">Response</span></span>
<a id="response" class="xliff"></a>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->