---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的状态信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 25750b5484558c53ab03d3001bc2b8bafa307524
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035992"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="589cb-103">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="589cb-103">networkConnection resource type</span></span>

<span data-ttu-id="589cb-104">包含有关与警报相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="589cb-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="589cb-105">属性</span><span class="sxs-lookup"><span data-stu-id="589cb-105">Properties</span></span>

| <span data-ttu-id="589cb-106">属性</span><span class="sxs-lookup"><span data-stu-id="589cb-106">Property</span></span>   | <span data-ttu-id="589cb-107">类型</span><span class="sxs-lookup"><span data-stu-id="589cb-107">Type</span></span>|<span data-ttu-id="589cb-108">说明</span><span class="sxs-lookup"><span data-stu-id="589cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="589cb-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="589cb-109">applicationName</span></span>|<span data-ttu-id="589cb-110">String</span><span class="sxs-lookup"><span data-stu-id="589cb-110">String</span></span>|<span data-ttu-id="589cb-111">管理网络连接的应用程序的名称 (例如, Facebook、SMTP 等)。</span><span class="sxs-lookup"><span data-stu-id="589cb-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="589cb-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="589cb-112">destinationAddress</span></span>|<span data-ttu-id="589cb-113">String</span><span class="sxs-lookup"><span data-stu-id="589cb-113">String</span></span>|<span data-ttu-id="589cb-114">目标 IP 地址 (的网络连接)。</span><span class="sxs-lookup"><span data-stu-id="589cb-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="589cb-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="589cb-115">destinationDomain</span></span>|<span data-ttu-id="589cb-116">String</span><span class="sxs-lookup"><span data-stu-id="589cb-116">String</span></span>|<span data-ttu-id="589cb-117">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="589cb-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="589cb-118">(例如, "www.contoso.com")。</span><span class="sxs-lookup"><span data-stu-id="589cb-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="589cb-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="589cb-119">destinationPort</span></span>|<span data-ttu-id="589cb-120">String</span><span class="sxs-lookup"><span data-stu-id="589cb-120">String</span></span>|<span data-ttu-id="589cb-121">目标端口 (网络连接)。</span><span class="sxs-lookup"><span data-stu-id="589cb-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="589cb-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="589cb-122">destinationUrl</span></span>|<span data-ttu-id="589cb-123">String</span><span class="sxs-lookup"><span data-stu-id="589cb-123">String</span></span>|<span data-ttu-id="589cb-124">网络连接 URL/URI 字符串-不包括参数。</span><span class="sxs-lookup"><span data-stu-id="589cb-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="589cb-125">(例如, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="589cb-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="589cb-126">direction</span><span class="sxs-lookup"><span data-stu-id="589cb-126">direction</span></span>|<span data-ttu-id="589cb-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="589cb-127">connectionDirection</span></span>|<span data-ttu-id="589cb-128">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="589cb-128">Network connection direction.</span></span> <span data-ttu-id="589cb-129">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="589cb-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="589cb-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="589cb-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="589cb-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="589cb-131">DateTimeOffset</span></span>|<span data-ttu-id="589cb-132">注册目标域的日期。</span><span class="sxs-lookup"><span data-stu-id="589cb-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="589cb-133">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="589cb-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="589cb-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="589cb-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="589cb-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="589cb-135">localDnsName</span></span>|<span data-ttu-id="589cb-136">String</span><span class="sxs-lookup"><span data-stu-id="589cb-136">String</span></span>|<span data-ttu-id="589cb-137">在主机的本地 DNS 缓存中显示的本地 DNS 名称解析 (例如, 在 "主机" 文件被篡改的情况下)。</span><span class="sxs-lookup"><span data-stu-id="589cb-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="589cb-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="589cb-138">natDestinationAddress</span></span>|<span data-ttu-id="589cb-139">String</span><span class="sxs-lookup"><span data-stu-id="589cb-139">String</span></span>|<span data-ttu-id="589cb-140">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="589cb-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="589cb-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="589cb-141">natDestinationPort</span></span>|<span data-ttu-id="589cb-142">String</span><span class="sxs-lookup"><span data-stu-id="589cb-142">String</span></span>|<span data-ttu-id="589cb-143">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="589cb-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="589cb-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="589cb-144">natSourceAddress</span></span>|<span data-ttu-id="589cb-145">String</span><span class="sxs-lookup"><span data-stu-id="589cb-145">String</span></span>|<span data-ttu-id="589cb-146">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="589cb-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="589cb-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="589cb-147">natSourcePort</span></span>|<span data-ttu-id="589cb-148">String</span><span class="sxs-lookup"><span data-stu-id="589cb-148">String</span></span>|<span data-ttu-id="589cb-149">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="589cb-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="589cb-150">协议</span><span class="sxs-lookup"><span data-stu-id="589cb-150">protocol</span></span>|[<span data-ttu-id="589cb-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="589cb-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="589cb-152">网络协议。</span><span class="sxs-lookup"><span data-stu-id="589cb-152">Network protocol.</span></span> <span data-ttu-id="589cb-153">可能的值为`unknown`: `ip`、 `icmp`、 `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader`、、、、、、、、、、、、、、、、 `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="589cb-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="589cb-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="589cb-154">riskScore</span></span>|<span data-ttu-id="589cb-155">String</span><span class="sxs-lookup"><span data-stu-id="589cb-155">String</span></span>|<span data-ttu-id="589cb-156">提供程序生成/计算网络连接的风险分数。</span><span class="sxs-lookup"><span data-stu-id="589cb-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="589cb-157">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="589cb-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="589cb-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="589cb-158">sourceAddress</span></span>|<span data-ttu-id="589cb-159">String</span><span class="sxs-lookup"><span data-stu-id="589cb-159">String</span></span>|<span data-ttu-id="589cb-160">源 (即, 网络连接的来源) 的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="589cb-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="589cb-161">sourcePort</span><span class="sxs-lookup"><span data-stu-id="589cb-161">sourcePort</span></span>|<span data-ttu-id="589cb-162">String</span><span class="sxs-lookup"><span data-stu-id="589cb-162">String</span></span>|<span data-ttu-id="589cb-163">源 (即源) IP 端口 (的网络连接)。</span><span class="sxs-lookup"><span data-stu-id="589cb-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="589cb-164">status</span><span class="sxs-lookup"><span data-stu-id="589cb-164">status</span></span>|<span data-ttu-id="589cb-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="589cb-165">connectionStatus</span></span>|<span data-ttu-id="589cb-166">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="589cb-166">Network connection status.</span></span> <span data-ttu-id="589cb-167">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="589cb-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="589cb-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="589cb-168">urlParameters</span></span>|<span data-ttu-id="589cb-169">String</span><span class="sxs-lookup"><span data-stu-id="589cb-169">String</span></span>|<span data-ttu-id="589cb-170">目标 URL 的参数 (后缀)。</span><span class="sxs-lookup"><span data-stu-id="589cb-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="589cb-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="589cb-171">JSON representation</span></span>

<span data-ttu-id="589cb-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="589cb-172">The following is a JSON representation of the resource.</span></span>

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
