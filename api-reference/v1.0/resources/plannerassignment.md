<span data-ttu-id="51079-p103">用于对任务中的代理人进行排序的提示。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="51079-p103">Hint used to order assignees in a task. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|用于对任务中的代理人进行排序的提示。[此处](planner_order_hint_format.md)概述了此格式。|

## <span data-ttu-id="51079-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51079-120">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="51079-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51079-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->