<span data-ttu-id="40bfb-p103">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="40bfb-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。|
|<span data-ttu-id="40bfb-135">references</span><span class="sxs-lookup"><span data-stu-id="40bfb-135">references</span></span>|[<span data-ttu-id="40bfb-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="40bfb-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="40bfb-137">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="40bfb-137">The collection of references on the task.</span></span>|

## <span data-ttu-id="40bfb-138">关系</span><span class="sxs-lookup"><span data-stu-id="40bfb-138">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="40bfb-139">无</span><span class="sxs-lookup"><span data-stu-id="40bfb-139">None</span></span>


## <span data-ttu-id="40bfb-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40bfb-140">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="40bfb-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40bfb-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->