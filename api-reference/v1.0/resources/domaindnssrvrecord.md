<span data-ttu-id="a4828-p105">配置 DNS 主机上的 SRV 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="a4828-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span>| 配置 DNS 主机上的 SRV 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null |
|<span data-ttu-id="a4828-149">weight</span><span class="sxs-lookup"><span data-stu-id="a4828-149">weight</span></span>|<span data-ttu-id="a4828-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a4828-150">Int32</span></span>| <span data-ttu-id="a4828-151">配置 DNS 主机上的 SRV 记录的*权重*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="a4828-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <span data-ttu-id="a4828-152">关系</span><span class="sxs-lookup"><span data-stu-id="a4828-152">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="a4828-153">无</span><span class="sxs-lookup"><span data-stu-id="a4828-153">None</span></span>


## <span data-ttu-id="a4828-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4828-154">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="a4828-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4828-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->