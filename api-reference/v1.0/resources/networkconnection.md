---
title: networkConnection 资源类型
description: 包含有关与警报相关的网络连接的有状态信息。
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5671726ead3da811c109a9a2afe01c49b665e513
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719008"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="93fa0-103">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="93fa0-103">networkConnection resource type</span></span>

<span data-ttu-id="93fa0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93fa0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93fa0-105">包含有关与警报相关的网络连接的有状态信息。</span><span class="sxs-lookup"><span data-stu-id="93fa0-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="93fa0-106">属性</span><span class="sxs-lookup"><span data-stu-id="93fa0-106">Properties</span></span>

| <span data-ttu-id="93fa0-107">属性</span><span class="sxs-lookup"><span data-stu-id="93fa0-107">Property</span></span>   | <span data-ttu-id="93fa0-108">类型</span><span class="sxs-lookup"><span data-stu-id="93fa0-108">Type</span></span>|<span data-ttu-id="93fa0-109">说明</span><span class="sxs-lookup"><span data-stu-id="93fa0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93fa0-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="93fa0-110">applicationName</span></span>|<span data-ttu-id="93fa0-111">String</span><span class="sxs-lookup"><span data-stu-id="93fa0-111">String</span></span>|<span data-ttu-id="93fa0-112">管理网络连接应用程序的名称 (例如 Facebook 或 SMTP) 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-112">Name of the application managing the network connection (for example, Facebook or SMTP).</span></span>|
|<span data-ttu-id="93fa0-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="93fa0-113">destinationAddress</span></span>|<span data-ttu-id="93fa0-114">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-114">String</span></span>|<span data-ttu-id="93fa0-115">网络连接 (的目标 IP 地址) 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="93fa0-116">destinationLocation</span><span class="sxs-lookup"><span data-stu-id="93fa0-116">destinationLocation</span></span>|<span data-ttu-id="93fa0-117">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-117">String</span></span>|<span data-ttu-id="93fa0-118">位置 (IP 地址映射) 网络连接目标关联的位置。</span><span class="sxs-lookup"><span data-stu-id="93fa0-118">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="93fa0-119">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="93fa0-119">destinationDomain</span></span>|<span data-ttu-id="93fa0-120">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-120">String</span></span>|<span data-ttu-id="93fa0-121">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="93fa0-121">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="93fa0-122"> (例如"www.contoso.com") 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-122">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="93fa0-123">destinationPort</span><span class="sxs-lookup"><span data-stu-id="93fa0-123">destinationPort</span></span>|<span data-ttu-id="93fa0-124">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-124">String</span></span>|<span data-ttu-id="93fa0-125">网络连接 (的目标端口) 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-125">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="93fa0-126">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="93fa0-126">destinationUrl</span></span>|<span data-ttu-id="93fa0-127">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-127">String</span></span>|<span data-ttu-id="93fa0-128">网络连接 URL/URI 字符串 - 不包括参数。</span><span class="sxs-lookup"><span data-stu-id="93fa0-128">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="93fa0-129"> (例如"www.contoso.com/products/default.html') </span><span class="sxs-lookup"><span data-stu-id="93fa0-129">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="93fa0-130">direction</span><span class="sxs-lookup"><span data-stu-id="93fa0-130">direction</span></span>|<span data-ttu-id="93fa0-131">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="93fa0-131">connectionDirection</span></span>|<span data-ttu-id="93fa0-132">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="93fa0-132">Network connection direction.</span></span> <span data-ttu-id="93fa0-133">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="93fa0-133">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="93fa0-134">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="93fa0-134">domainRegisteredDateTime</span></span>|<span data-ttu-id="93fa0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93fa0-135">DateTimeOffset</span></span>|<span data-ttu-id="93fa0-136">目标域的注册日期。</span><span class="sxs-lookup"><span data-stu-id="93fa0-136">Date when the destination domain was registered.</span></span> <span data-ttu-id="93fa0-137">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="93fa0-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93fa0-138">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="93fa0-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="93fa0-139">localDnsName</span><span class="sxs-lookup"><span data-stu-id="93fa0-139">localDnsName</span></span>|<span data-ttu-id="93fa0-140">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-140">String</span></span>|<span data-ttu-id="93fa0-141">显示在主机本地 DNS 缓存中的本地 DNS 名称解析 (例如，如果"主机"文件被篡改) 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-141">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="93fa0-142">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="93fa0-142">natDestinationAddress</span></span>|<span data-ttu-id="93fa0-143">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-143">String</span></span>|<span data-ttu-id="93fa0-144">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="93fa0-144">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="93fa0-145">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="93fa0-145">natDestinationPort</span></span>|<span data-ttu-id="93fa0-146">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-146">String</span></span>|<span data-ttu-id="93fa0-147">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="93fa0-147">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="93fa0-148">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="93fa0-148">natSourceAddress</span></span>|<span data-ttu-id="93fa0-149">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-149">String</span></span>|<span data-ttu-id="93fa0-150">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="93fa0-150">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="93fa0-151">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="93fa0-151">natSourcePort</span></span>|<span data-ttu-id="93fa0-152">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-152">String</span></span>|<span data-ttu-id="93fa0-153">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="93fa0-153">Network Address Translation source port.</span></span>|
|<span data-ttu-id="93fa0-154">协议</span><span class="sxs-lookup"><span data-stu-id="93fa0-154">protocol</span></span>|[<span data-ttu-id="93fa0-155">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="93fa0-155">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="93fa0-156">网络协议。</span><span class="sxs-lookup"><span data-stu-id="93fa0-156">Network protocol.</span></span> <span data-ttu-id="93fa0-157">可能的值是 `unknown` `ip` `icmp` ：、、、、、、、、、、 `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-157">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="93fa0-158">riskScore</span><span class="sxs-lookup"><span data-stu-id="93fa0-158">riskScore</span></span>|<span data-ttu-id="93fa0-159">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-159">String</span></span>|<span data-ttu-id="93fa0-160">提供商生成/计算网络连接的风险评分。</span><span class="sxs-lookup"><span data-stu-id="93fa0-160">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="93fa0-161">建议的值范围为 0-1，等于百分比。</span><span class="sxs-lookup"><span data-stu-id="93fa0-161">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="93fa0-162">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="93fa0-162">sourceAddress</span></span>|<span data-ttu-id="93fa0-163">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-163">String</span></span>|<span data-ttu-id="93fa0-164">源 (，即) 网络连接 (源 IP 地址) 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-164">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="93fa0-165">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="93fa0-165">sourceLocation</span></span>|<span data-ttu-id="93fa0-166">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-166">String</span></span>|<span data-ttu-id="93fa0-167">位置 (IP 地址映射) 网络连接源关联的 IP 地址映射。</span><span class="sxs-lookup"><span data-stu-id="93fa0-167">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="93fa0-168">sourcePort</span><span class="sxs-lookup"><span data-stu-id="93fa0-168">sourcePort</span></span>|<span data-ttu-id="93fa0-169">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-169">String</span></span>|<span data-ttu-id="93fa0-170">源 (，即) 网络 (源 IP 端口) 。</span><span class="sxs-lookup"><span data-stu-id="93fa0-170">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="93fa0-171">状态</span><span class="sxs-lookup"><span data-stu-id="93fa0-171">status</span></span>|<span data-ttu-id="93fa0-172">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="93fa0-172">connectionStatus</span></span>|<span data-ttu-id="93fa0-173">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="93fa0-173">Network connection status.</span></span> <span data-ttu-id="93fa0-174">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="93fa0-174">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="93fa0-175">urlParameters</span><span class="sxs-lookup"><span data-stu-id="93fa0-175">urlParameters</span></span>|<span data-ttu-id="93fa0-176">字符串</span><span class="sxs-lookup"><span data-stu-id="93fa0-176">String</span></span>|<span data-ttu-id="93fa0-177">参数 (URL) 后缀。</span><span class="sxs-lookup"><span data-stu-id="93fa0-177">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93fa0-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93fa0-178">JSON representation</span></span>

<span data-ttu-id="93fa0-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93fa0-179">The following is a JSON representation of the resource.</span></span>

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
  "destinationLocation": "String",
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
  "sourceLocation": "String",
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

