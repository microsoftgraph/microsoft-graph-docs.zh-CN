# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="18dcb-101">domainDnsUnavailableRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="18dcb-101">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="18dcb-p101">查询[域](domain.md)实体的导航属性 **serviceConfigurationRecords** 时，可能会返回一个或多个 [DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和/或 [DomainDnsTxtRecord](domaindnstxtrecord.md) 实体。这些实体指示 Microsoft Online Services 可以使用域前必须要添加到域的区域文件的 DNS 记录。无法生成这些实体时，将返回 DomainDnsUnavailableRecord 实体。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="18dcb-p101">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="18dcb-106">方法</span><span class="sxs-lookup"><span data-stu-id="18dcb-106">Methods</span></span>
<span data-ttu-id="18dcb-p102">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="18dcb-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="18dcb-109">属性</span><span class="sxs-lookup"><span data-stu-id="18dcb-109">Properties</span></span>
| <span data-ttu-id="18dcb-110">属性</span><span class="sxs-lookup"><span data-stu-id="18dcb-110">Property</span></span>     | <span data-ttu-id="18dcb-111">类型</span><span class="sxs-lookup"><span data-stu-id="18dcb-111">Type</span></span>   |<span data-ttu-id="18dcb-112">说明</span><span class="sxs-lookup"><span data-stu-id="18dcb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18dcb-113">说明</span><span class="sxs-lookup"><span data-stu-id="18dcb-113">description</span></span>|<span data-ttu-id="18dcb-114">String</span><span class="sxs-lookup"><span data-stu-id="18dcb-114">String</span></span>|<span data-ttu-id="18dcb-115">提供返回 **DomainDnsUnavailableRecord** 实体的原因。</span><span class="sxs-lookup"><span data-stu-id="18dcb-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="18dcb-116">关系</span><span class="sxs-lookup"><span data-stu-id="18dcb-116">Relationships</span></span>
<span data-ttu-id="18dcb-117">无</span><span class="sxs-lookup"><span data-stu-id="18dcb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18dcb-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18dcb-118">JSON representation</span></span>
<span data-ttu-id="18dcb-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18dcb-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
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