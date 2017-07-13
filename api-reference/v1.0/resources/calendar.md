<span data-ttu-id="40223-p111">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="40223-p111">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>| 为日历定义的单值扩展属性的集合。只读。可为 Null。|

## <span data-ttu-id="40223-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40223-206">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="40223-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40223-207">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
