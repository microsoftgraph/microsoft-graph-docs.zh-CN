<span data-ttu-id="080a2-p104">用于设置检查表中的项目的相对顺序。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="080a2-p104">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|用于设置检查表中的项目的相对顺序。[此处](planner_order_hint_format.md)概述了此格式。|
|<span data-ttu-id="080a2-125">title</span><span class="sxs-lookup"><span data-stu-id="080a2-125">title</span></span>|<span data-ttu-id="080a2-126">String</span><span class="sxs-lookup"><span data-stu-id="080a2-126">String</span></span>|<span data-ttu-id="080a2-127">检查表项目的标题</span><span class="sxs-lookup"><span data-stu-id="080a2-127">Title of the checklist item</span></span>|

## <span data-ttu-id="080a2-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="080a2-128">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="080a2-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="080a2-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->