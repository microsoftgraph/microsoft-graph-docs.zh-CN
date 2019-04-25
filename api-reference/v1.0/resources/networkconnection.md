---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的状态信息。
localization_priority: Normal
ms.openlocfilehash: 78ddcfd19d68b8dcd64c74a5beed6d1430f0ca38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580273"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="bb0aa-103">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb0aa-103">networkConnection resource type</span></span>

<span data-ttu-id="bb0aa-104">包含有关与警报相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="bb0aa-105">属性</span><span class="sxs-lookup"><span data-stu-id="bb0aa-105">Properties</span></span>

| <span data-ttu-id="bb0aa-106">属性</span><span class="sxs-lookup"><span data-stu-id="bb0aa-106">Property</span></span>   | <span data-ttu-id="bb0aa-107">类型</span><span class="sxs-lookup"><span data-stu-id="bb0aa-107">Type</span></span>|<span data-ttu-id="bb0aa-108">说明</span><span class="sxs-lookup"><span data-stu-id="bb0aa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb0aa-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="bb0aa-109">applicationName</span></span>|<span data-ttu-id="bb0aa-110">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-110">String</span></span>|<span data-ttu-id="bb0aa-111">管理网络连接的应用程序的名称 (例如, Facebook、SMTP 等)。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="bb0aa-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="bb0aa-112">destinationAddress</span></span>|<span data-ttu-id="bb0aa-113">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-113">String</span></span>|<span data-ttu-id="bb0aa-114">目标 IP 地址 (的网络连接)。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="bb0aa-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="bb0aa-115">destinationDomain</span></span>|<span data-ttu-id="bb0aa-116">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-116">String</span></span>|<span data-ttu-id="bb0aa-117">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="bb0aa-118">(例如, "www.contoso.com")。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="bb0aa-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="bb0aa-119">destinationPort</span></span>|<span data-ttu-id="bb0aa-120">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-120">String</span></span>|<span data-ttu-id="bb0aa-121">目标端口 (网络连接)。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="bb0aa-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="bb0aa-122">destinationUrl</span></span>|<span data-ttu-id="bb0aa-123">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-123">String</span></span>|<span data-ttu-id="bb0aa-124">网络连接 URL/URI 字符串-不包括参数。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="bb0aa-125">(例如, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="bb0aa-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="bb0aa-126">direction</span><span class="sxs-lookup"><span data-stu-id="bb0aa-126">direction</span></span>|<span data-ttu-id="bb0aa-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="bb0aa-127">connectionDirection</span></span>|<span data-ttu-id="bb0aa-128">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-128">Network connection direction.</span></span> <span data-ttu-id="bb0aa-129">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="bb0aa-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="bb0aa-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="bb0aa-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb0aa-131">DateTimeOffset</span></span>|<span data-ttu-id="bb0aa-132">注册目标域的日期。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="bb0aa-133">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bb0aa-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bb0aa-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bb0aa-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="bb0aa-135">localDnsName</span></span>|<span data-ttu-id="bb0aa-136">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-136">String</span></span>|<span data-ttu-id="bb0aa-137">在主机的本地 dns 缓存中显示的本地 dns 名称解析 (例如, 在 "主机" 文件被篡改的情况下)。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="bb0aa-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="bb0aa-138">natDestinationAddress</span></span>|<span data-ttu-id="bb0aa-139">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-139">String</span></span>|<span data-ttu-id="bb0aa-140">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="bb0aa-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="bb0aa-141">natDestinationPort</span></span>|<span data-ttu-id="bb0aa-142">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-142">String</span></span>|<span data-ttu-id="bb0aa-143">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="bb0aa-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="bb0aa-144">natSourceAddress</span></span>|<span data-ttu-id="bb0aa-145">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-145">String</span></span>|<span data-ttu-id="bb0aa-146">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="bb0aa-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="bb0aa-147">natSourcePort</span></span>|<span data-ttu-id="bb0aa-148">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-148">String</span></span>|<span data-ttu-id="bb0aa-149">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="bb0aa-150">协议</span><span class="sxs-lookup"><span data-stu-id="bb0aa-150">protocol</span></span>|[<span data-ttu-id="bb0aa-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="bb0aa-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="bb0aa-152">网络协议。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-152">Network protocol.</span></span> <span data-ttu-id="bb0aa-153">可能的值为`unknown`: `ip`、 `icmp`、 `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader`、、、、、、、、、、、、、、、、 `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="bb0aa-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="bb0aa-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="bb0aa-154">riskScore</span></span>|<span data-ttu-id="bb0aa-155">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-155">String</span></span>|<span data-ttu-id="bb0aa-156">提供程序生成/计算网络连接的风险分数。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="bb0aa-157">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="bb0aa-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="bb0aa-158">sourceAddress</span></span>|<span data-ttu-id="bb0aa-159">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-159">String</span></span>|<span data-ttu-id="bb0aa-160">源 (即, 网络连接的来源) 的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="bb0aa-161">sourcePort</span><span class="sxs-lookup"><span data-stu-id="bb0aa-161">sourcePort</span></span>|<span data-ttu-id="bb0aa-162">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-162">String</span></span>|<span data-ttu-id="bb0aa-163">源 (即源) IP 端口 (的网络连接)。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="bb0aa-164">状态</span><span class="sxs-lookup"><span data-stu-id="bb0aa-164">status</span></span>|<span data-ttu-id="bb0aa-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="bb0aa-165">connectionStatus</span></span>|<span data-ttu-id="bb0aa-166">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-166">Network connection status.</span></span> <span data-ttu-id="bb0aa-167">可取值为：`unknown`、`attempted`、`succeeded`、`blocked` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="bb0aa-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="bb0aa-168">urlParameters</span></span>|<span data-ttu-id="bb0aa-169">String</span><span class="sxs-lookup"><span data-stu-id="bb0aa-169">String</span></span>|<span data-ttu-id="bb0aa-170">目标 URL 的参数 (后缀)。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb0aa-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb0aa-171">JSON representation</span></span>

<span data-ttu-id="bb0aa-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb0aa-172">The following is a JSON representation of the resource.</span></span>

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
