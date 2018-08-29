# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="840d1-101">domainDnsSrvRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="840d1-101">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="840d1-p101">表示已添加到租户中特定域的 DNS 区域文件的 SRV 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="840d1-p101">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="840d1-104">方法</span><span class="sxs-lookup"><span data-stu-id="840d1-104">Methods</span></span>
<span data-ttu-id="840d1-p102">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="840d1-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="840d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="840d1-107">Properties</span></span>
| <span data-ttu-id="840d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="840d1-108">Property</span></span>     | <span data-ttu-id="840d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="840d1-109">Type</span></span>   |<span data-ttu-id="840d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="840d1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="840d1-111">id</span><span class="sxs-lookup"><span data-stu-id="840d1-111">id</span></span>|<span data-ttu-id="840d1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-112">String</span></span>| <span data-ttu-id="840d1-p103">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="840d1-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="840d1-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="840d1-115">isOptional</span></span>|<span data-ttu-id="840d1-116">布尔</span><span class="sxs-lookup"><span data-stu-id="840d1-116">Boolean</span></span>| <span data-ttu-id="840d1-117">如果为 false，则客户必须在 DNS 主机上配置 SRV 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="840d1-117">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="840d1-118">label</span><span class="sxs-lookup"><span data-stu-id="840d1-118">label</span></span>|<span data-ttu-id="840d1-119">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-119">String</span></span>| <span data-ttu-id="840d1-120">配置 DNS 主机上的 SRV 记录的 *name* 属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-120">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="840d1-121">nameTarget</span><span class="sxs-lookup"><span data-stu-id="840d1-121">nameTarget</span></span>|<span data-ttu-id="840d1-122">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-122">String</span></span>| <span data-ttu-id="840d1-123">配置 DNS 主机上的 SRV 记录的*目标*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-123">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="840d1-124">port</span><span class="sxs-lookup"><span data-stu-id="840d1-124">port</span></span>|<span data-ttu-id="840d1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="840d1-125">Int32</span></span>| <span data-ttu-id="840d1-126">配置 DNS 主机上的 SRV 记录的*端口*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-126">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="840d1-127">priority</span><span class="sxs-lookup"><span data-stu-id="840d1-127">priority</span></span>|<span data-ttu-id="840d1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="840d1-128">Int32</span></span>| <span data-ttu-id="840d1-129">配置 DNS 主机上的 SRV 记录的*优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-129">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="840d1-130">protocol</span><span class="sxs-lookup"><span data-stu-id="840d1-130">protocol</span></span>|<span data-ttu-id="840d1-131">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-131">String</span></span>| <span data-ttu-id="840d1-132">配置 DNS 主机上的 SRV 记录的*协议*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-132">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="840d1-133">recordType</span><span class="sxs-lookup"><span data-stu-id="840d1-133">recordType</span></span>|<span data-ttu-id="840d1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-134">String</span></span>|  <span data-ttu-id="840d1-p104">DNS 记录类型。此值始终是 *Srv*。Key</span><span class="sxs-lookup"><span data-stu-id="840d1-p104">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="840d1-138">service</span><span class="sxs-lookup"><span data-stu-id="840d1-138">service</span></span>|<span data-ttu-id="840d1-139">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-139">String</span></span>| <span data-ttu-id="840d1-140">配置 DNS 主机上的 SRV 记录的*服务*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-140">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="840d1-141">supportedService</span><span class="sxs-lookup"><span data-stu-id="840d1-141">supportedService</span></span>|<span data-ttu-id="840d1-142">字符串</span><span class="sxs-lookup"><span data-stu-id="840d1-142">String</span></span>| <span data-ttu-id="840d1-143">Microsoft Online Service 或与该 SRV 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="840d1-143">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="840d1-144">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="840d1-144">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="840d1-145">ttl</span><span class="sxs-lookup"><span data-stu-id="840d1-145">ttl</span></span>|<span data-ttu-id="840d1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="840d1-146">Int32</span></span>| <span data-ttu-id="840d1-p105">配置 DNS 主机上的 SRV 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="840d1-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="840d1-149">weight</span><span class="sxs-lookup"><span data-stu-id="840d1-149">weight</span></span>|<span data-ttu-id="840d1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="840d1-150">Int32</span></span>| <span data-ttu-id="840d1-151">配置 DNS 主机上的 SRV 记录的*权重*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="840d1-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="840d1-152">关系</span><span class="sxs-lookup"><span data-stu-id="840d1-152">Relationships</span></span>
<span data-ttu-id="840d1-153">无</span><span class="sxs-lookup"><span data-stu-id="840d1-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="840d1-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="840d1-154">JSON representation</span></span>
<span data-ttu-id="840d1-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="840d1-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
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