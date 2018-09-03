# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="eee6b-101">domainDnsRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="eee6b-101">domainDnsRecord resource type</span></span>

<span data-ttu-id="eee6b-p101">对于租户中的每个域，可能需要先将 DNS 记录添加到相应域的 DNS 区域文件，然后 Microsoft Online Services 才能使用该域。**DomainDnsRecord** 实体用于显示这些 DNS 记录。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) 和 [DomainDnsSrvRecord](domaindnssrvrecord.md) 实体的基本实体。</span><span class="sxs-lookup"><span data-stu-id="eee6b-p101">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="eee6b-105">方法</span><span class="sxs-lookup"><span data-stu-id="eee6b-105">Methods</span></span>
<span data-ttu-id="eee6b-p102">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="eee6b-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="eee6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="eee6b-108">Properties</span></span>
| <span data-ttu-id="eee6b-109">属性</span><span class="sxs-lookup"><span data-stu-id="eee6b-109">Property</span></span>     | <span data-ttu-id="eee6b-110">类型</span><span class="sxs-lookup"><span data-stu-id="eee6b-110">Type</span></span>   |<span data-ttu-id="eee6b-111">说明</span><span class="sxs-lookup"><span data-stu-id="eee6b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eee6b-112">id</span><span class="sxs-lookup"><span data-stu-id="eee6b-112">id</span></span>|<span data-ttu-id="eee6b-113">String</span><span class="sxs-lookup"><span data-stu-id="eee6b-113">String</span></span>| <span data-ttu-id="eee6b-p103">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="eee6b-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="eee6b-116">isOptional</span><span class="sxs-lookup"><span data-stu-id="eee6b-116">isOptional</span></span>|<span data-ttu-id="eee6b-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="eee6b-117">Boolean</span></span>| <span data-ttu-id="eee6b-118">如果为 false，则客户必须在 DNS 主机上配置此记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="eee6b-118">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="eee6b-119">label</span><span class="sxs-lookup"><span data-stu-id="eee6b-119">label</span></span>|<span data-ttu-id="eee6b-120">String</span><span class="sxs-lookup"><span data-stu-id="eee6b-120">String</span></span>| <span data-ttu-id="eee6b-121">配置 DNS 主机上的 DNS 记录的名称时使用的值。</span><span class="sxs-lookup"><span data-stu-id="eee6b-121">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="eee6b-122">recordType</span><span class="sxs-lookup"><span data-stu-id="eee6b-122">recordType</span></span>|<span data-ttu-id="eee6b-123">String</span><span class="sxs-lookup"><span data-stu-id="eee6b-123">String</span></span>| <span data-ttu-id="eee6b-124">指示此实体表示的 DNS 记录类型。</span><span class="sxs-lookup"><span data-stu-id="eee6b-124">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="eee6b-125">值可以是下列值之一：*CName*、*Mx*、*Srv*、*Txt*</span><span class="sxs-lookup"><span data-stu-id="eee6b-125">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="eee6b-126">Key</span><span class="sxs-lookup"><span data-stu-id="eee6b-126">Key</span></span> |
|<span data-ttu-id="eee6b-127">supportedService</span><span class="sxs-lookup"><span data-stu-id="eee6b-127">supportedService</span></span>|<span data-ttu-id="eee6b-128">String</span><span class="sxs-lookup"><span data-stu-id="eee6b-128">String</span></span>| <span data-ttu-id="eee6b-129">Microsoft Online Service 或与该 DNS 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="eee6b-129">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="eee6b-130">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="eee6b-130">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="eee6b-131">ttl</span><span class="sxs-lookup"><span data-stu-id="eee6b-131">ttl</span></span>|<span data-ttu-id="eee6b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="eee6b-132">Int32</span></span>| <span data-ttu-id="eee6b-p104">配置 DNS 主机上的 DNS 记录的生存时间 (ttl) 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="eee6b-p104">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="eee6b-135">关系</span><span class="sxs-lookup"><span data-stu-id="eee6b-135">Relationships</span></span>
<span data-ttu-id="eee6b-136">无</span><span class="sxs-lookup"><span data-stu-id="eee6b-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eee6b-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eee6b-137">JSON representation</span></span>
<span data-ttu-id="eee6b-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eee6b-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->