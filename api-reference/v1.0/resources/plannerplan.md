<span data-ttu-id="ecffe-p109">只读。可为 Null。计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="ecffe-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>| 只读。可为 Null。计划中的任务集合。|

## <span data-ttu-id="ecffe-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecffe-171">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="ecffe-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecffe-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->