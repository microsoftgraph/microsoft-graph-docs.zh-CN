<span data-ttu-id="5a768-p106">架构扩展适用的支持扩展的 Microsoft Graph 类型集。从**联系人**、**设备**、**事件**、**组**、**邮件**、**组织**、**帖子**或**用户**中选择。</span><span class="sxs-lookup"><span data-stu-id="5a768-p106">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to. Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|架构扩展适用的支持扩展的 Microsoft Graph 类型集。从**联系人**、**设备**、**事件**、**组**、**邮件**、**组织**、**帖子**或**用户**中选择。|

## <span data-ttu-id="5a768-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a768-166">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="5a768-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a768-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->