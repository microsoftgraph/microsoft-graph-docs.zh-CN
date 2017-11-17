<span data-ttu-id="908bf-p103">该示例将从任务的代理人列表中删除 ID 为 ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 的用户，并更改用户 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的代理人顺序。如果尚未将任务分配给 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的用户，则使用此值更新分配会将此任务分配给该用户。</span><span class="sxs-lookup"><span data-stu-id="908bf-p103">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
该示例将从任务的代理人列表中删除 ID 为 ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 的用户，并更改用户 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的代理人顺序。如果尚未将任务分配给 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的用户，则使用此值更新分配会将此任务分配给该用户。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->