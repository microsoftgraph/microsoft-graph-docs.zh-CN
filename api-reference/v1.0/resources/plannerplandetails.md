<span data-ttu-id="69abb-p103">此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="69abb-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。 |

## <span data-ttu-id="69abb-132">关系</span><span class="sxs-lookup"><span data-stu-id="69abb-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="69abb-133">无</span><span class="sxs-lookup"><span data-stu-id="69abb-133">None</span></span>


## <span data-ttu-id="69abb-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69abb-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="69abb-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69abb-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->