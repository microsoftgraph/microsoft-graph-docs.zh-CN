# <a name="filtercriteria-resource-type"></a><span data-ttu-id="d5a79-101">FilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5a79-101">FilterCriteria resource type</span></span>

<span data-ttu-id="d5a79-102">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="d5a79-102">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5a79-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5a79-103">JSON representation</span></span>

<span data-ttu-id="d5a79-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5a79-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "icon": {"@odata.type": "microsoft.graph.workbookIcon"},
  "values": {"@odata.type": "microsoft.graph.Json"}
}

```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'color' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion1' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion2' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'dynamicCriteria' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'filterOn' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'icon' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'values' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table."
  ]
} -->