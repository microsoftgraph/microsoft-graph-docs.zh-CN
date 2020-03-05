---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的状态信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86986178bc7104118dfb4db83ae43f7780307fe6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447365"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="5c952-103">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c952-103">networkConnection resource type</span></span>

<span data-ttu-id="5c952-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5c952-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c952-105">包含有关与警报相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="5c952-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="5c952-106">属性</span><span class="sxs-lookup"><span data-stu-id="5c952-106">Properties</span></span>

| <span data-ttu-id="5c952-107">属性</span><span class="sxs-lookup"><span data-stu-id="5c952-107">Property</span></span>   | <span data-ttu-id="5c952-108">类型</span><span class="sxs-lookup"><span data-stu-id="5c952-108">Type</span></span>|<span data-ttu-id="5c952-109">说明</span><span class="sxs-lookup"><span data-stu-id="5c952-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c952-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="5c952-110">applicationName</span></span>|<span data-ttu-id="5c952-111">String</span><span class="sxs-lookup"><span data-stu-id="5c952-111">String</span></span>|<span data-ttu-id="5c952-112">管理网络连接的应用程序的名称（例如，Facebook、SMTP 等）。</span><span class="sxs-lookup"><span data-stu-id="5c952-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="5c952-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="5c952-113">destinationAddress</span></span>|<span data-ttu-id="5c952-114">String</span><span class="sxs-lookup"><span data-stu-id="5c952-114">String</span></span>|<span data-ttu-id="5c952-115">目标 IP 地址（的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="5c952-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="5c952-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="5c952-116">destinationDomain</span></span>|<span data-ttu-id="5c952-117">String</span><span class="sxs-lookup"><span data-stu-id="5c952-117">String</span></span>|<span data-ttu-id="5c952-118">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="5c952-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="5c952-119">（例如，"www.contoso.com"）。</span><span class="sxs-lookup"><span data-stu-id="5c952-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="5c952-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="5c952-120">destinationPort</span></span>|<span data-ttu-id="5c952-121">String</span><span class="sxs-lookup"><span data-stu-id="5c952-121">String</span></span>|<span data-ttu-id="5c952-122">目标端口（网络连接）。</span><span class="sxs-lookup"><span data-stu-id="5c952-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="5c952-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="5c952-123">destinationUrl</span></span>|<span data-ttu-id="5c952-124">String</span><span class="sxs-lookup"><span data-stu-id="5c952-124">String</span></span>|<span data-ttu-id="5c952-125">网络连接 URL/URI 字符串-不包括参数。</span><span class="sxs-lookup"><span data-stu-id="5c952-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="5c952-126">（例如，"www.contoso.com/products/default.html"）</span><span class="sxs-lookup"><span data-stu-id="5c952-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="5c952-127">direction</span><span class="sxs-lookup"><span data-stu-id="5c952-127">direction</span></span>|<span data-ttu-id="5c952-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="5c952-128">connectionDirection</span></span>|<span data-ttu-id="5c952-129">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="5c952-129">Network connection direction.</span></span> <span data-ttu-id="5c952-130">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="5c952-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="5c952-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="5c952-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="5c952-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c952-132">DateTimeOffset</span></span>|<span data-ttu-id="5c952-133">注册目标域的日期。</span><span class="sxs-lookup"><span data-stu-id="5c952-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="5c952-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5c952-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c952-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5c952-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5c952-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="5c952-136">localDnsName</span></span>|<span data-ttu-id="5c952-137">String</span><span class="sxs-lookup"><span data-stu-id="5c952-137">String</span></span>|<span data-ttu-id="5c952-138">在主机的本地 DNS 缓存中显示的本地 DNS 名称解析（例如，在 "主机" 文件被篡改的情况下）。</span><span class="sxs-lookup"><span data-stu-id="5c952-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="5c952-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="5c952-139">natDestinationAddress</span></span>|<span data-ttu-id="5c952-140">String</span><span class="sxs-lookup"><span data-stu-id="5c952-140">String</span></span>|<span data-ttu-id="5c952-141">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="5c952-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="5c952-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="5c952-142">natDestinationPort</span></span>|<span data-ttu-id="5c952-143">String</span><span class="sxs-lookup"><span data-stu-id="5c952-143">String</span></span>|<span data-ttu-id="5c952-144">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="5c952-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="5c952-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="5c952-145">natSourceAddress</span></span>|<span data-ttu-id="5c952-146">String</span><span class="sxs-lookup"><span data-stu-id="5c952-146">String</span></span>|<span data-ttu-id="5c952-147">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="5c952-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="5c952-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="5c952-148">natSourcePort</span></span>|<span data-ttu-id="5c952-149">String</span><span class="sxs-lookup"><span data-stu-id="5c952-149">String</span></span>|<span data-ttu-id="5c952-150">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="5c952-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="5c952-151">协议</span><span class="sxs-lookup"><span data-stu-id="5c952-151">protocol</span></span>|[<span data-ttu-id="5c952-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="5c952-152">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="5c952-153">网络协议。</span><span class="sxs-lookup"><span data-stu-id="5c952-153">Network protocol.</span></span> <span data-ttu-id="5c952-154">可能的值为`unknown`： `ip`、 `icmp`、 `igmp` `ggp` `ipv4` `tcp` `spx` `spxII`、、、、、、、、、、、、、、、、、、、、。 `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx`</span><span class="sxs-lookup"><span data-stu-id="5c952-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="5c952-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="5c952-155">riskScore</span></span>|<span data-ttu-id="5c952-156">String</span><span class="sxs-lookup"><span data-stu-id="5c952-156">String</span></span>|<span data-ttu-id="5c952-157">提供程序生成/计算网络连接的风险分数。</span><span class="sxs-lookup"><span data-stu-id="5c952-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="5c952-158">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="5c952-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="5c952-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="5c952-159">sourceAddress</span></span>|<span data-ttu-id="5c952-160">String</span><span class="sxs-lookup"><span data-stu-id="5c952-160">String</span></span>|<span data-ttu-id="5c952-161">源（即，网络连接的来源）的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="5c952-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="5c952-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="5c952-162">sourcePort</span></span>|<span data-ttu-id="5c952-163">String</span><span class="sxs-lookup"><span data-stu-id="5c952-163">String</span></span>|<span data-ttu-id="5c952-164">源（即源） IP 端口（的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="5c952-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="5c952-165">status</span><span class="sxs-lookup"><span data-stu-id="5c952-165">status</span></span>|<span data-ttu-id="5c952-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="5c952-166">connectionStatus</span></span>|<span data-ttu-id="5c952-167">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="5c952-167">Network connection status.</span></span> <span data-ttu-id="5c952-168">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="5c952-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="5c952-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="5c952-169">urlParameters</span></span>|<span data-ttu-id="5c952-170">String</span><span class="sxs-lookup"><span data-stu-id="5c952-170">String</span></span>|<span data-ttu-id="5c952-171">目标 URL 的参数（后缀）。</span><span class="sxs-lookup"><span data-stu-id="5c952-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c952-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c952-172">JSON representation</span></span>

<span data-ttu-id="5c952-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c952-173">The following is a JSON representation of the resource.</span></span>

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
