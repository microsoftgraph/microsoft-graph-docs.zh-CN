<span data-ttu-id="21d8c-p104">唯一的 SKU 显示名称。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber；例如：“AAD_Premium”。只读</span><span class="sxs-lookup"><span data-stu-id="21d8c-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span>| 唯一的 SKU 显示名称。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber；例如：“AAD_Premium”。只读 |

## <span data-ttu-id="21d8c-132">关系</span><span class="sxs-lookup"><span data-stu-id="21d8c-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="21d8c-133">无</span><span class="sxs-lookup"><span data-stu-id="21d8c-133">None</span></span>

## <span data-ttu-id="21d8c-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21d8c-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="21d8c-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21d8c-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->