<span data-ttu-id="77995-p104">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，提示值用于为任务板 AssignedTo 视图上的任务排序。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="77995-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，提示值用于为任务板 AssignedTo 视图上的任务排序。[此处](planner_order_hint_format.md)概述了此格式。|

## <span data-ttu-id="77995-133">关系</span><span class="sxs-lookup"><span data-stu-id="77995-133">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="77995-134">无</span><span class="sxs-lookup"><span data-stu-id="77995-134">None</span></span>


## <span data-ttu-id="77995-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77995-135">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="77995-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77995-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->