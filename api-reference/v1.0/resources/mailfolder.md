<span data-ttu-id="eaac8-p107">为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="eaac8-p107">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>| 为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。|


## <span data-ttu-id="eaac8-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eaac8-200">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="eaac8-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaac8-201">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <span data-ttu-id="eaac8-202">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eaac8-202">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="eaac8-203">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="eaac8-203">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="eaac8-204">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="eaac8-204">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
