<span data-ttu-id="861f3-p107">配置 DNS 主机上的 CNAME 记录的生存时间 (ttl) 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="861f3-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span>| 配置 DNS 主机上的 CNAME 记录的生存时间 (ttl) 属性时使用的值。不可为 null |

## <span data-ttu-id="861f3-139">关系</span><span class="sxs-lookup"><span data-stu-id="861f3-139">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="861f3-140">无</span><span class="sxs-lookup"><span data-stu-id="861f3-140">None</span></span>


## <span data-ttu-id="861f3-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="861f3-141">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="861f3-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="861f3-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->