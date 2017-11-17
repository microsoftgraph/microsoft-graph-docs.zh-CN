<span data-ttu-id="3cecb-p102">模板的的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="3cecb-p102">Unique identifier for the subscription. Read-only.</span></span>| 模板的的唯一标识符。只读。|
|<span data-ttu-id="3cecb-131">values</span><span class="sxs-lookup"><span data-stu-id="3cecb-131">values</span></span>|<span data-ttu-id="3cecb-132">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3cecb-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="3cecb-133">setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。</span><span class="sxs-lookup"><span data-stu-id="3cecb-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3cecb-134">关系</span><span class="sxs-lookup"><span data-stu-id="3cecb-134">Relationships</span></span>

<span data-ttu-id="3cecb-135">无。</span><span class="sxs-lookup"><span data-stu-id="3cecb-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3cecb-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cecb-136">JSON representation</span></span>

<span data-ttu-id="3cecb-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cecb-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->