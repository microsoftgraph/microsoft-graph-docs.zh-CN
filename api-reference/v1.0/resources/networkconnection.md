# <a name="networkconnection-resource-type"></a><span data-ttu-id="daabd-101">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="daabd-101">networkConnection resource type</span></span>

<span data-ttu-id="daabd-102">包含有关与通知相关的网络连接的有状态信息。</span><span class="sxs-lookup"><span data-stu-id="daabd-102">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="daabd-103">属性</span><span class="sxs-lookup"><span data-stu-id="daabd-103">Properties</span></span>

| <span data-ttu-id="daabd-104">属性</span><span class="sxs-lookup"><span data-stu-id="daabd-104">Property</span></span>   | <span data-ttu-id="daabd-105">类型</span><span class="sxs-lookup"><span data-stu-id="daabd-105">Type</span></span>|<span data-ttu-id="daabd-106">说明</span><span class="sxs-lookup"><span data-stu-id="daabd-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daabd-107">applicationName</span><span class="sxs-lookup"><span data-stu-id="daabd-107">applicationName</span></span>|<span data-ttu-id="daabd-108">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-108">String</span></span>|<span data-ttu-id="daabd-109">管理网络连接的应用程序的名称 （例如，Facebook、SMTP 等）。</span><span class="sxs-lookup"><span data-stu-id="daabd-109">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="daabd-110">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="daabd-110">destinationAddress</span></span>|<span data-ttu-id="daabd-111">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-111">String</span></span>|<span data-ttu-id="daabd-112">（网络连接的）目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="daabd-112">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="daabd-113">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="daabd-113">destinationDomain</span></span>|<span data-ttu-id="daabd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-114">String</span></span>|<span data-ttu-id="daabd-115">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="daabd-115">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="daabd-116">(例如“www.contoso.com”)。</span><span class="sxs-lookup"><span data-stu-id="daabd-116">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="daabd-117">destinationPort</span><span class="sxs-lookup"><span data-stu-id="daabd-117">destinationPort</span></span>|<span data-ttu-id="daabd-118">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-118">String</span></span>|<span data-ttu-id="daabd-119">（网络连接的）目标端口。</span><span class="sxs-lookup"><span data-stu-id="daabd-119">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="daabd-120">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="daabd-120">destinationUrl</span></span>|<span data-ttu-id="daabd-121">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-121">String</span></span>|<span data-ttu-id="daabd-122">网络连接 URL/URI 字符串 - 不包括参数。</span><span class="sxs-lookup"><span data-stu-id="daabd-122">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="daabd-123">(例如“www.contoso.com/products/default.html”)</span><span class="sxs-lookup"><span data-stu-id="daabd-123">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="daabd-124">direction</span><span class="sxs-lookup"><span data-stu-id="daabd-124">direction</span></span>|<span data-ttu-id="daabd-125">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="daabd-125">connectionDirection</span></span>|<span data-ttu-id="daabd-126">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="daabd-126">Network connection direction.</span></span> <span data-ttu-id="daabd-127">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="daabd-127">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="daabd-128">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="daabd-128">domainRegisteredDateTime</span></span>|<span data-ttu-id="daabd-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daabd-129">DateTimeOffset</span></span>|<span data-ttu-id="daabd-130">注册目标域时的日期。</span><span class="sxs-lookup"><span data-stu-id="daabd-130">Date when the destination domain was registered.</span></span> <span data-ttu-id="daabd-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="daabd-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="daabd-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="daabd-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="daabd-133">localDnsName</span><span class="sxs-lookup"><span data-stu-id="daabd-133">localDnsName</span></span>|<span data-ttu-id="daabd-134">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-134">String</span></span>|<span data-ttu-id="daabd-135">出现在主机本地 DNS 缓存中的本地 DNS 名称解析（例如，假使“hosts”文件被篡改）。</span><span class="sxs-lookup"><span data-stu-id="daabd-135">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="daabd-136">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="daabd-136">natDestinationAddress</span></span>|<span data-ttu-id="daabd-137">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-137">String</span></span>|<span data-ttu-id="daabd-138">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="daabd-138">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="daabd-139">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="daabd-139">natDestinationPort</span></span>|<span data-ttu-id="daabd-140">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-140">String</span></span>|<span data-ttu-id="daabd-141">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="daabd-141">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="daabd-142">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="daabd-142">natSourceAddress</span></span>|<span data-ttu-id="daabd-143">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-143">String</span></span>|<span data-ttu-id="daabd-144">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="daabd-144">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="daabd-145">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="daabd-145">natSourcePort</span></span>|<span data-ttu-id="daabd-146">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-146">String</span></span>|<span data-ttu-id="daabd-147">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="daabd-147">Network Address Translation source port.</span></span>|
|<span data-ttu-id="daabd-148">protocol</span><span class="sxs-lookup"><span data-stu-id="daabd-148">protocol</span></span>|[<span data-ttu-id="daabd-149">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="daabd-149">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="daabd-150">网络协议。</span><span class="sxs-lookup"><span data-stu-id="daabd-150">Network protocol analysis</span></span> <span data-ttu-id="daabd-151">可取值为：`unknown`、`ip`、`icmp`、`igmp`、`ggp`、`ipv4`、`tcp`、`pup`、`udp`、`idp`、`ipv6`、`ipv6RoutingHeader`、`ipv6FragmentHeader`、`ipSecEncapsulatingSecurityPayload`、`ipSecAuthenticationHeader`、`icmpV6`、`ipv6NoNextHeader`、`ipv6DestinationOptions`、`nd`、`raw`、`ipx`、`spx`、`spxII`。</span><span class="sxs-lookup"><span data-stu-id="daabd-151">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`.</span></span>|
|<span data-ttu-id="daabd-152">riskScore</span><span class="sxs-lookup"><span data-stu-id="daabd-152">riskScore</span></span>|<span data-ttu-id="daabd-153">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-153">String</span></span>|<span data-ttu-id="daabd-154">提供程序生成/计算得出的网络连接风险分数。</span><span class="sxs-lookup"><span data-stu-id="daabd-154">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="daabd-155">建议值的范围为 0-1，相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="daabd-155">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="daabd-156">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="daabd-156">sourceAddress</span></span>|<span data-ttu-id="daabd-157">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-157">String</span></span>|<span data-ttu-id="daabd-158">（网络连接的）源（即原始）IP 地址。</span><span class="sxs-lookup"><span data-stu-id="daabd-158">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="daabd-159">sourcePort</span><span class="sxs-lookup"><span data-stu-id="daabd-159">sourcePort</span></span>|<span data-ttu-id="daabd-160">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-160">String</span></span>|<span data-ttu-id="daabd-161">源（即原始）IP 端口（网络连接）。</span><span class="sxs-lookup"><span data-stu-id="daabd-161">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="daabd-162">status</span><span class="sxs-lookup"><span data-stu-id="daabd-162">status</span></span>|<span data-ttu-id="daabd-163">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="daabd-163">ConnectionStatus</span></span>|<span data-ttu-id="daabd-164">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="daabd-164">Network connection status.</span></span> <span data-ttu-id="daabd-165">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="daabd-165">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="daabd-166">urlParameters</span><span class="sxs-lookup"><span data-stu-id="daabd-166">urlParameters</span></span>|<span data-ttu-id="daabd-167">字符串</span><span class="sxs-lookup"><span data-stu-id="daabd-167">String</span></span>|<span data-ttu-id="daabd-168">目标 URL 的参数（后缀）。</span><span class="sxs-lookup"><span data-stu-id="daabd-168">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="daabd-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="daabd-169">JSON representation</span></span>

<span data-ttu-id="daabd-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daabd-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->