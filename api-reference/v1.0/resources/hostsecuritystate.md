# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="a2432-101">hostSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2432-101">hostSecurityState resource type</span></span>

<span data-ttu-id="a2432-102">包含状态信息 （包括设备、计算机等）的主机。</span><span class="sxs-lookup"><span data-stu-id="a2432-102">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="a2432-103">属性</span><span class="sxs-lookup"><span data-stu-id="a2432-103">Properties</span></span>

| <span data-ttu-id="a2432-104">属性</span><span class="sxs-lookup"><span data-stu-id="a2432-104">Property</span></span>   | <span data-ttu-id="a2432-105">类型</span><span class="sxs-lookup"><span data-stu-id="a2432-105">Type</span></span>|<span data-ttu-id="a2432-106">说明</span><span class="sxs-lookup"><span data-stu-id="a2432-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2432-107">FQDN</span><span class="sxs-lookup"><span data-stu-id="a2432-107">FQDN</span></span>|<span data-ttu-id="a2432-108">字符串</span><span class="sxs-lookup"><span data-stu-id="a2432-108">String</span></span>|<span data-ttu-id="a2432-109">承载 FQDN （完全限定域名）(例如，`machine.company.com`)。</span><span class="sxs-lookup"><span data-stu-id="a2432-109">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="a2432-110">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="a2432-110">isAzureAadJoined</span></span>|<span data-ttu-id="a2432-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="a2432-111">Boolean</span></span>|<span data-ttu-id="a2432-112">如果主机是加入到 Azure Active Directory 域服务的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="a2432-112">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="a2432-113">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="a2432-113">isAzureAadRegistered</span></span>|<span data-ttu-id="a2432-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="a2432-114">Boolean</span></span>|<span data-ttu-id="a2432-115">如果主机注册 Azure Active Directory 设备注册 （BYOD 设备-，即不完全由企业管理），则为 true。</span><span class="sxs-lookup"><span data-stu-id="a2432-115">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="a2432-116">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="a2432-116">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="a2432-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="a2432-117">Boolean</span></span>|<span data-ttu-id="a2432-118">如果主机是加入本地 Active Directory 域的域，则为 true。</span><span class="sxs-lookup"><span data-stu-id="a2432-118">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="a2432-119">netBiosName</span><span class="sxs-lookup"><span data-stu-id="a2432-119">netBiosName</span></span>|<span data-ttu-id="a2432-120">字符串</span><span class="sxs-lookup"><span data-stu-id="a2432-120">String</span></span>|<span data-ttu-id="a2432-121">不带的 DNS 域名的本地主机名称。</span><span class="sxs-lookup"><span data-stu-id="a2432-121">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="a2432-122">os</span><span class="sxs-lookup"><span data-stu-id="a2432-122">OS</span></span>|<span data-ttu-id="a2432-123">字符串</span><span class="sxs-lookup"><span data-stu-id="a2432-123">String</span></span>|<span data-ttu-id="a2432-124">主机操作系统</span><span class="sxs-lookup"><span data-stu-id="a2432-124">Host Operating System.</span></span> <span data-ttu-id="a2432-125">（例如，Windows10 MacOS、RHEL，等）。</span><span class="sxs-lookup"><span data-stu-id="a2432-125">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="a2432-126">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="a2432-126">privateIpAddress</span></span>|<span data-ttu-id="a2432-127">字符串</span><span class="sxs-lookup"><span data-stu-id="a2432-127">String</span></span>|<span data-ttu-id="a2432-128">在警报时，私有（不可路由）IPv4 或 IPv6 地址（请参阅[RFC 1918](https://tools.ietf.org/html/rfc1918)）。</span><span class="sxs-lookup"><span data-stu-id="a2432-128">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="a2432-129">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="a2432-129">publicIpAddress</span></span>|<span data-ttu-id="a2432-130">字符串</span><span class="sxs-lookup"><span data-stu-id="a2432-130">String</span></span>|<span data-ttu-id="a2432-131">在警报时，公共可路由的 IPv4 或 IPv6 地址 （请参阅 [RFC 1918](https://tools.ietf.org/html/rfc1918)）。</span><span class="sxs-lookup"><span data-stu-id="a2432-131">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="a2432-132">riskScore</span><span class="sxs-lookup"><span data-stu-id="a2432-132">riskScore</span></span>|<span data-ttu-id="a2432-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a2432-133">String</span></span>|<span data-ttu-id="a2432-134">提供程序生成/计算主机的风险评分。</span><span class="sxs-lookup"><span data-stu-id="a2432-134">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="a2432-135">建议值的范围为 0-1，相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="a2432-135">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2432-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2432-136">JSON representation</span></span>

<span data-ttu-id="a2432-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2432-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
