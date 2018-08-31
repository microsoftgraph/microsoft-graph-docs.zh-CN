# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="1a5c1-101">domainDnsCnameRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a5c1-101">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="1a5c1-p101">表示已添加到租户中特定域的 DNS 区域文件的 CNAME 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p101">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="1a5c1-104">方法</span><span class="sxs-lookup"><span data-stu-id="1a5c1-104">Methods</span></span>
<span data-ttu-id="1a5c1-p102">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="1a5c1-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a5c1-107">Properties</span></span>
| <span data-ttu-id="1a5c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a5c1-108">Property</span></span>     | <span data-ttu-id="1a5c1-109">类型</span><span class="sxs-lookup"><span data-stu-id="1a5c1-109">Type</span></span>   |<span data-ttu-id="1a5c1-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a5c1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a5c1-111">canonicalName</span><span class="sxs-lookup"><span data-stu-id="1a5c1-111">canonicalName</span></span>|<span data-ttu-id="1a5c1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1a5c1-112">String</span></span>| <span data-ttu-id="1a5c1-p103">CNAME 记录的规范名称。用于配置 DNS 主机上的 CNAME 记录。</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p103">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="1a5c1-115">ID</span><span class="sxs-lookup"><span data-stu-id="1a5c1-115">id</span></span>|<span data-ttu-id="1a5c1-116">字符串</span><span class="sxs-lookup"><span data-stu-id="1a5c1-116">String</span></span>| <span data-ttu-id="1a5c1-p104">分配给该实体的唯一标识符。不可为 NULL，只读</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p104">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="1a5c1-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="1a5c1-119">isOptional</span></span>|<span data-ttu-id="1a5c1-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="1a5c1-120">Boolean</span></span>| <span data-ttu-id="1a5c1-p105">如果为 false，则客户必须在 DNS 主机上配置 CNAME 记录才能使 Microsoft Online Services 在域中正常运行。不可为 null</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p105">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="1a5c1-123">标签</span><span class="sxs-lookup"><span data-stu-id="1a5c1-123">label</span></span>|<span data-ttu-id="1a5c1-124">字符串</span><span class="sxs-lookup"><span data-stu-id="1a5c1-124">String</span></span>| <span data-ttu-id="1a5c1-125">配置 DNS 主机上的 CNAME 记录的*别名/主机/名称*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="1a5c1-125">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="1a5c1-126">recordType</span><span class="sxs-lookup"><span data-stu-id="1a5c1-126">recordType</span></span>|<span data-ttu-id="1a5c1-127">字符串</span><span class="sxs-lookup"><span data-stu-id="1a5c1-127">String</span></span>| <span data-ttu-id="1a5c1-p106">DNS 记录类型。此值始终是 *CName*。键</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p106">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="1a5c1-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="1a5c1-131">supportedService</span></span>|<span data-ttu-id="1a5c1-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1a5c1-132">String</span></span>| <span data-ttu-id="1a5c1-133">Microsoft Online Service 或与该 CNAME 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="1a5c1-133">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="1a5c1-134">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="1a5c1-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="1a5c1-135">ttl</span><span class="sxs-lookup"><span data-stu-id="1a5c1-135">ttl</span></span>|<span data-ttu-id="1a5c1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1a5c1-136">Int32</span></span>| <span data-ttu-id="1a5c1-p107">配置 DNS 主机上的 CNAME 记录的生存时间 (ttl) 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="1a5c1-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="1a5c1-139">关系</span><span class="sxs-lookup"><span data-stu-id="1a5c1-139">Relationships</span></span>
<span data-ttu-id="1a5c1-140">无</span><span class="sxs-lookup"><span data-stu-id="1a5c1-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a5c1-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a5c1-141">JSON representation</span></span>
<span data-ttu-id="1a5c1-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a5c1-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
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