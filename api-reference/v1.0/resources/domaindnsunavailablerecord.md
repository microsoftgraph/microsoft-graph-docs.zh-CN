<span data-ttu-id="90875-p102">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="90875-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>
不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。

## <span data-ttu-id="90875-109">属性</span><span class="sxs-lookup"><span data-stu-id="90875-109">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="90875-110">属性</span><span class="sxs-lookup"><span data-stu-id="90875-110">Property</span></span>     | <span data-ttu-id="90875-111">类型</span><span class="sxs-lookup"><span data-stu-id="90875-111">Type</span></span>   |<span data-ttu-id="90875-112">说明</span><span class="sxs-lookup"><span data-stu-id="90875-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90875-113">说明</span><span class="sxs-lookup"><span data-stu-id="90875-113">description</span></span>|<span data-ttu-id="90875-114">String</span><span class="sxs-lookup"><span data-stu-id="90875-114">String</span></span>|<span data-ttu-id="90875-115">提供返回 **DomainDnsUnavailableRecord** 实体的原因。</span><span class="sxs-lookup"><span data-stu-id="90875-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <span data-ttu-id="90875-116">关系</span><span class="sxs-lookup"><span data-stu-id="90875-116">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="90875-117">无</span><span class="sxs-lookup"><span data-stu-id="90875-117">None</span></span>

## <span data-ttu-id="90875-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90875-118">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="90875-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90875-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->