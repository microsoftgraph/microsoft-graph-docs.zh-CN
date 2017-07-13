<span data-ttu-id="d5845-p106">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d5845-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。|


## <span data-ttu-id="d5845-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5845-164">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="d5845-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5845-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
