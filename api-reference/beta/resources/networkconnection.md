---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9d25d78d51a39d3240d0d7566b7037f55e379fe1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811110"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="3c7c5-104">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c7c5-104">networkConnection resource type</span></span>

<span data-ttu-id="3c7c5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c7c5-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c7c5-106">包含有关与警报相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-106">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="3c7c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="3c7c5-107">Properties</span></span>

| <span data-ttu-id="3c7c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c7c5-108">Property</span></span>   | <span data-ttu-id="3c7c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="3c7c5-109">Type</span></span>|<span data-ttu-id="3c7c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="3c7c5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c7c5-111">applicationName</span><span class="sxs-lookup"><span data-stu-id="3c7c5-111">applicationName</span></span>|<span data-ttu-id="3c7c5-112">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-112">String</span></span>|<span data-ttu-id="3c7c5-113">管理网络连接的应用程序的名称 (例如，Facebook、SMTP 等 ) 。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-113">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="3c7c5-114">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="3c7c5-114">destinationAddress</span></span>|<span data-ttu-id="3c7c5-115">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-115">String</span></span>|<span data-ttu-id="3c7c5-116">网络连接) 的目标 IP 地址 (。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-116">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="3c7c5-117">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="3c7c5-117">destinationDomain</span></span>|<span data-ttu-id="3c7c5-118">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-118">String</span></span>|<span data-ttu-id="3c7c5-119">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-119">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="3c7c5-120"> (例如 "www.contoso.com" ) 。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-120">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="3c7c5-121">destinationLocation</span><span class="sxs-lookup"><span data-stu-id="3c7c5-121">destinationLocation</span></span>|<span data-ttu-id="3c7c5-122">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-122">String</span></span>|<span data-ttu-id="3c7c5-123">通过 IP 地址映射)  (与网络连接的目标相关联的位置。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-123">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="3c7c5-124">destinationPort</span><span class="sxs-lookup"><span data-stu-id="3c7c5-124">destinationPort</span></span>|<span data-ttu-id="3c7c5-125">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-125">String</span></span>|<span data-ttu-id="3c7c5-126">网络连接) 的目标端口 (。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-126">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="3c7c5-127">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="3c7c5-127">destinationUrl</span></span>|<span data-ttu-id="3c7c5-128">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-128">String</span></span>|<span data-ttu-id="3c7c5-129">网络连接 URL/URI 字符串-不包括参数。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-129">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="3c7c5-130"> (例如 "www.contoso.com/products/default.html" ) </span><span class="sxs-lookup"><span data-stu-id="3c7c5-130">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="3c7c5-131">direction</span><span class="sxs-lookup"><span data-stu-id="3c7c5-131">direction</span></span>|<span data-ttu-id="3c7c5-132">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="3c7c5-132">connectionDirection</span></span>|<span data-ttu-id="3c7c5-133">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-133">Network connection direction.</span></span> <span data-ttu-id="3c7c5-134">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-134">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="3c7c5-135">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="3c7c5-135">domainRegisteredDateTime</span></span>|<span data-ttu-id="3c7c5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c7c5-136">DateTimeOffset</span></span>|<span data-ttu-id="3c7c5-137">注册目标域的日期。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-137">Date when the destination domain was registered.</span></span> <span data-ttu-id="3c7c5-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c7c5-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3c7c5-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3c7c5-140">localDnsName</span><span class="sxs-lookup"><span data-stu-id="3c7c5-140">localDnsName</span></span>|<span data-ttu-id="3c7c5-141">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-141">String</span></span>|<span data-ttu-id="3c7c5-142">在主机的本地 DNS 缓存中显示的本地 DNS 名称解析 (例如，如果 "hosts" 文件被篡改) 。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-142">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="3c7c5-143">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="3c7c5-143">natDestinationAddress</span></span>|<span data-ttu-id="3c7c5-144">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-144">String</span></span>|<span data-ttu-id="3c7c5-145">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-145">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="3c7c5-146">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="3c7c5-146">natDestinationPort</span></span>|<span data-ttu-id="3c7c5-147">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-147">String</span></span>|<span data-ttu-id="3c7c5-148">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-148">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="3c7c5-149">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="3c7c5-149">natSourceAddress</span></span>|<span data-ttu-id="3c7c5-150">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-150">String</span></span>|<span data-ttu-id="3c7c5-151">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-151">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="3c7c5-152">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="3c7c5-152">natSourcePort</span></span>|<span data-ttu-id="3c7c5-153">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-153">String</span></span>|<span data-ttu-id="3c7c5-154">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-154">Network Address Translation source port.</span></span>|
|<span data-ttu-id="3c7c5-155">协议</span><span class="sxs-lookup"><span data-stu-id="3c7c5-155">protocol</span></span>|<span data-ttu-id="3c7c5-156">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="3c7c5-156">securityNetworkProtocol</span></span>|<span data-ttu-id="3c7c5-157">网络协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-157">Network protocol.</span></span> <span data-ttu-id="3c7c5-158">可能的值为：、、、、、、、、、、、、、、、、、、、、、、 `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` 。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-158">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="3c7c5-159">riskScore</span><span class="sxs-lookup"><span data-stu-id="3c7c5-159">riskScore</span></span>|<span data-ttu-id="3c7c5-160">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-160">String</span></span>|<span data-ttu-id="3c7c5-161">提供程序生成/计算网络连接的风险分数。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-161">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="3c7c5-162">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-162">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="3c7c5-163">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="3c7c5-163">sourceAddress</span></span>|<span data-ttu-id="3c7c5-164">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-164">String</span></span>|<span data-ttu-id="3c7c5-165">源 (（即网络连接) 的来源) IP 地址） (。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-165">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="3c7c5-166">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="3c7c5-166">sourceLocation</span></span>|<span data-ttu-id="3c7c5-167">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-167">String</span></span>|<span data-ttu-id="3c7c5-168">与网络连接的源相关联的 IP 地址映射)  (位置。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-168">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="3c7c5-169">sourcePort</span><span class="sxs-lookup"><span data-stu-id="3c7c5-169">sourcePort</span></span>|<span data-ttu-id="3c7c5-170">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-170">String</span></span>|<span data-ttu-id="3c7c5-171">源 (（即网络连接) 的 IP 端口 (）的来源) 。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-171">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="3c7c5-172">status</span><span class="sxs-lookup"><span data-stu-id="3c7c5-172">status</span></span>|<span data-ttu-id="3c7c5-173">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="3c7c5-173">connectionStatus</span></span>|<span data-ttu-id="3c7c5-174">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-174">Network connection status.</span></span> <span data-ttu-id="3c7c5-175">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-175">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="3c7c5-176">urlParameters</span><span class="sxs-lookup"><span data-stu-id="3c7c5-176">urlParameters</span></span>|<span data-ttu-id="3c7c5-177">String</span><span class="sxs-lookup"><span data-stu-id="3c7c5-177">String</span></span>|<span data-ttu-id="3c7c5-178">参数 (后缀) 的目标 URL。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-178">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="3c7c5-179">securityNetworkProtocol 值</span><span class="sxs-lookup"><span data-stu-id="3c7c5-179">securityNetworkProtocol values</span></span>

|<span data-ttu-id="3c7c5-180">成员</span><span class="sxs-lookup"><span data-stu-id="3c7c5-180">Member</span></span>|<span data-ttu-id="3c7c5-181">值</span><span class="sxs-lookup"><span data-stu-id="3c7c5-181">Value</span></span>|<span data-ttu-id="3c7c5-182">说明</span><span class="sxs-lookup"><span data-stu-id="3c7c5-182">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c7c5-183">unknown</span><span class="sxs-lookup"><span data-stu-id="3c7c5-183">unknown</span></span>|<span data-ttu-id="3c7c5-184">-1</span><span class="sxs-lookup"><span data-stu-id="3c7c5-184">-1</span></span>|<span data-ttu-id="3c7c5-185">未知协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-185">Unknown protocol.</span></span>|
|<span data-ttu-id="3c7c5-186">ip</span><span class="sxs-lookup"><span data-stu-id="3c7c5-186">ip</span></span>|<span data-ttu-id="3c7c5-187">0</span><span class="sxs-lookup"><span data-stu-id="3c7c5-187">0</span></span>|<span data-ttu-id="3c7c5-188">Internet 协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-188">Internet Protocol.</span></span>|
|<span data-ttu-id="3c7c5-189">icmp</span><span class="sxs-lookup"><span data-stu-id="3c7c5-189">icmp</span></span>|<span data-ttu-id="3c7c5-190">1</span><span class="sxs-lookup"><span data-stu-id="3c7c5-190">1</span></span>| <span data-ttu-id="3c7c5-191">Internet 控制邮件协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-191">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="3c7c5-192">igmp</span><span class="sxs-lookup"><span data-stu-id="3c7c5-192">igmp</span></span>|<span data-ttu-id="3c7c5-193">双面</span><span class="sxs-lookup"><span data-stu-id="3c7c5-193">2</span></span>| <span data-ttu-id="3c7c5-194">Internet 组管理协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-194">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="3c7c5-195">ggp</span><span class="sxs-lookup"><span data-stu-id="3c7c5-195">ggp</span></span>|<span data-ttu-id="3c7c5-196">第三章</span><span class="sxs-lookup"><span data-stu-id="3c7c5-196">3</span></span>| <span data-ttu-id="3c7c5-197">网关到网关协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-197">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="3c7c5-198">ipv4</span><span class="sxs-lookup"><span data-stu-id="3c7c5-198">ipv4</span></span>|<span data-ttu-id="3c7c5-199">4 </span><span class="sxs-lookup"><span data-stu-id="3c7c5-199">4</span></span>| <span data-ttu-id="3c7c5-200">Internet 协议版本4。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-200">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="3c7c5-201">tcp</span><span class="sxs-lookup"><span data-stu-id="3c7c5-201">tcp</span></span>|<span data-ttu-id="3c7c5-202">6 </span><span class="sxs-lookup"><span data-stu-id="3c7c5-202">6</span></span>| <span data-ttu-id="3c7c5-203">传输控制协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-203">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="3c7c5-204">pup</span><span class="sxs-lookup"><span data-stu-id="3c7c5-204">pup</span></span>|<span data-ttu-id="3c7c5-205">12 </span><span class="sxs-lookup"><span data-stu-id="3c7c5-205">12</span></span>| <span data-ttu-id="3c7c5-206">PARC 通用数据包协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-206">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="3c7c5-207">udp</span><span class="sxs-lookup"><span data-stu-id="3c7c5-207">udp</span></span>|<span data-ttu-id="3c7c5-208">17 </span><span class="sxs-lookup"><span data-stu-id="3c7c5-208">17</span></span>| <span data-ttu-id="3c7c5-209">用户数据报协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-209">User Datagram Protocol.</span></span>|
|<span data-ttu-id="3c7c5-210">idp</span><span class="sxs-lookup"><span data-stu-id="3c7c5-210">idp</span></span>|<span data-ttu-id="3c7c5-211">22</span><span class="sxs-lookup"><span data-stu-id="3c7c5-211">22</span></span>| <span data-ttu-id="3c7c5-212">Internet 数据报协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-212">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="3c7c5-213">ipv4</span><span class="sxs-lookup"><span data-stu-id="3c7c5-213">ipv6</span></span>|<span data-ttu-id="3c7c5-214">41</span><span class="sxs-lookup"><span data-stu-id="3c7c5-214">41</span></span>| <span data-ttu-id="3c7c5-215">Internet 协议版本 6 (ipv6) 。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-215">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="3c7c5-216">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="3c7c5-216">ipv6RoutingHeader</span></span>|<span data-ttu-id="3c7c5-217">43</span><span class="sxs-lookup"><span data-stu-id="3c7c5-217">43</span></span>| <span data-ttu-id="3c7c5-218">ipv6 路由头。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-218">ipv6 Routing header.</span></span>|
|<span data-ttu-id="3c7c5-219">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="3c7c5-219">ipv6FragmentHeader</span></span>|<span data-ttu-id="3c7c5-220">44</span><span class="sxs-lookup"><span data-stu-id="3c7c5-220">44</span></span>| <span data-ttu-id="3c7c5-221">ipv6 分段标头。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-221">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="3c7c5-222">ipSecEncapsulatingSecurityPayload</span><span class="sxs-lookup"><span data-stu-id="3c7c5-222">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="3c7c5-223">50</span><span class="sxs-lookup"><span data-stu-id="3c7c5-223">50</span></span>| <span data-ttu-id="3c7c5-224">ipv6 封装安全有效负载标头。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-224">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="3c7c5-225">ipSecAuthenticationHeader</span><span class="sxs-lookup"><span data-stu-id="3c7c5-225">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="3c7c5-226">51</span><span class="sxs-lookup"><span data-stu-id="3c7c5-226">51</span></span>| <span data-ttu-id="3c7c5-227">ipv6 身份验证标头。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-227">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="3c7c5-228">icmpV6</span><span class="sxs-lookup"><span data-stu-id="3c7c5-228">icmpV6</span></span>|<span data-ttu-id="3c7c5-229">58</span><span class="sxs-lookup"><span data-stu-id="3c7c5-229">58</span></span>| <span data-ttu-id="3c7c5-230">Ipv6 的 Internet 控制消息协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-230">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="3c7c5-231">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="3c7c5-231">ipv6NoNextHeader</span></span>|<span data-ttu-id="3c7c5-232">59</span><span class="sxs-lookup"><span data-stu-id="3c7c5-232">59</span></span>| <span data-ttu-id="3c7c5-233">ipv6 无下一个标头。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-233">ipv6 No next header.</span></span>|
|<span data-ttu-id="3c7c5-234">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="3c7c5-234">ipv6DestinationOptions</span></span>|<span data-ttu-id="3c7c5-235">60</span><span class="sxs-lookup"><span data-stu-id="3c7c5-235">60</span></span>| <span data-ttu-id="3c7c5-236">ipv6 目标选项标头。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-236">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="3c7c5-237">点</span><span class="sxs-lookup"><span data-stu-id="3c7c5-237">nd</span></span>|<span data-ttu-id="3c7c5-238">77</span><span class="sxs-lookup"><span data-stu-id="3c7c5-238">77</span></span>| <span data-ttu-id="3c7c5-239"> (非正式) 的网络磁盘协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-239">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="3c7c5-240">原始</span><span class="sxs-lookup"><span data-stu-id="3c7c5-240">raw</span></span>|<span data-ttu-id="3c7c5-241">255</span><span class="sxs-lookup"><span data-stu-id="3c7c5-241">255</span></span>| <span data-ttu-id="3c7c5-242">原始 IP 数据包协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-242">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="3c7c5-243">通讯</span><span class="sxs-lookup"><span data-stu-id="3c7c5-243">ipx</span></span>|<span data-ttu-id="3c7c5-244">1000</span><span class="sxs-lookup"><span data-stu-id="3c7c5-244">1000</span></span>| <span data-ttu-id="3c7c5-245">Internet 数据包交换协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-245">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="3c7c5-246">spx</span><span class="sxs-lookup"><span data-stu-id="3c7c5-246">spx</span></span>|<span data-ttu-id="3c7c5-247">1256</span><span class="sxs-lookup"><span data-stu-id="3c7c5-247">1256</span></span>| <span data-ttu-id="3c7c5-248">序列化的数据包交换协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-248">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="3c7c5-249">spxII</span><span class="sxs-lookup"><span data-stu-id="3c7c5-249">spxII</span></span>|<span data-ttu-id="3c7c5-250">1257</span><span class="sxs-lookup"><span data-stu-id="3c7c5-250">1257</span></span>| <span data-ttu-id="3c7c5-251">序列化数据包交换第2版协议。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-251">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c7c5-252">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c7c5-252">JSON representation</span></span>

<span data-ttu-id="3c7c5-253">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c7c5-253">The following is a JSON representation of the resource.</span></span>

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
  "destinationLocation": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "string",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourceLocation": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
