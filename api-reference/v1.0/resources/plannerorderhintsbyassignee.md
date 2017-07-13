<span data-ttu-id="cb33d-p102">开放类型的属性可以由客户端定义。在这种情况下，客户必须将已分配到任务的用户 ID 作为属性名称，并且将有效的[排序提示](planner_order_hint_format.md)作为值。无法从此类型中删除属性。更新对包含的 [plannerTask](plannerTask.md) 的分配后服务将自动删除值。</span><span class="sxs-lookup"><span data-stu-id="cb33d-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner_order_hint_format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannerTask.md) are updated.</span></span>
开放类型的属性可以由客户端定义。在这种情况下，客户必须将已分配到任务的用户 ID 作为属性名称，并且将有效的[排序提示](planner_order_hint_format.md)作为值。无法从此类型中删除属性。更新对包含的 [plannerTask](plannerTask.md) 的分配后服务将自动删除值。

<span data-ttu-id="cb33d-110">示例：</span><span class="sxs-lookup"><span data-stu-id="cb33d-110">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->