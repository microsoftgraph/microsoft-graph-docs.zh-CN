# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="616eb-101">domainDnsMxRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="616eb-101">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="616eb-p101">表示已添加到租户中特定域的 DNS 区域文件的 MX 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。</span><span class="sxs-lookup"><span data-stu-id="616eb-p101">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="616eb-104">方法</span><span class="sxs-lookup"><span data-stu-id="616eb-104">Methods</span></span>
<span data-ttu-id="616eb-p102">不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。</span><span class="sxs-lookup"><span data-stu-id="616eb-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="616eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="616eb-107">Properties</span></span>
| <span data-ttu-id="616eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="616eb-108">Property</span></span>     | <span data-ttu-id="616eb-109">类型</span><span class="sxs-lookup"><span data-stu-id="616eb-109">Type</span></span>   |<span data-ttu-id="616eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="616eb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="616eb-111">id</span><span class="sxs-lookup"><span data-stu-id="616eb-111">id</span></span>|<span data-ttu-id="616eb-112">字符串</span><span class="sxs-lookup"><span data-stu-id="616eb-112">String</span></span>| <span data-ttu-id="616eb-p103">分配给此实体的唯一标识符。不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="616eb-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="616eb-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="616eb-115">isOptional</span></span>|<span data-ttu-id="616eb-116">布尔</span><span class="sxs-lookup"><span data-stu-id="616eb-116">Boolean</span></span>| <span data-ttu-id="616eb-117">如果为 false，则客户必须在 DNS 主机上配置 MX 记录才能使 Microsoft Online Services 在域中正常运行。</span><span class="sxs-lookup"><span data-stu-id="616eb-117">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="616eb-118">label</span><span class="sxs-lookup"><span data-stu-id="616eb-118">label</span></span>|<span data-ttu-id="616eb-119">字符串</span><span class="sxs-lookup"><span data-stu-id="616eb-119">String</span></span>| <span data-ttu-id="616eb-120">配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="616eb-120">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="616eb-121">mailExchange</span><span class="sxs-lookup"><span data-stu-id="616eb-121">mailExchange</span></span>|<span data-ttu-id="616eb-122">字符串</span><span class="sxs-lookup"><span data-stu-id="616eb-122">String</span></span>| <span data-ttu-id="616eb-123">配置 DNS 主机上的 MX 记录的*答复/目标/值*时使用的值。</span><span class="sxs-lookup"><span data-stu-id="616eb-123">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="616eb-124">preference</span><span class="sxs-lookup"><span data-stu-id="616eb-124">preference</span></span>|<span data-ttu-id="616eb-125">Int32</span><span class="sxs-lookup"><span data-stu-id="616eb-125">Int32</span></span>| <span data-ttu-id="616eb-126">配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。</span><span class="sxs-lookup"><span data-stu-id="616eb-126">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="616eb-127">recordType</span><span class="sxs-lookup"><span data-stu-id="616eb-127">recordType</span></span>|<span data-ttu-id="616eb-128">字符串</span><span class="sxs-lookup"><span data-stu-id="616eb-128">String</span></span>| <span data-ttu-id="616eb-p104">DNS 记录类型。此值始终是 *Mx*。Key</span><span class="sxs-lookup"><span data-stu-id="616eb-p104">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="616eb-132">supportedService</span><span class="sxs-lookup"><span data-stu-id="616eb-132">supportedService</span></span>|<span data-ttu-id="616eb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="616eb-133">String</span></span>| <span data-ttu-id="616eb-134">Microsoft Online Service 或与该 Mx 记录存在依赖关系的功能。</span><span class="sxs-lookup"><span data-stu-id="616eb-134">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="616eb-135">可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="616eb-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="616eb-136">ttl</span><span class="sxs-lookup"><span data-stu-id="616eb-136">ttl</span></span>|<span data-ttu-id="616eb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="616eb-137">Int32</span></span>| <span data-ttu-id="616eb-p105">配置 DNS 主机上的 MX 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null</span><span class="sxs-lookup"><span data-stu-id="616eb-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="616eb-140">关系</span><span class="sxs-lookup"><span data-stu-id="616eb-140">Relationships</span></span>
<span data-ttu-id="616eb-141">无</span><span class="sxs-lookup"><span data-stu-id="616eb-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="616eb-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="616eb-142">JSON representation</span></span>
<span data-ttu-id="616eb-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="616eb-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->