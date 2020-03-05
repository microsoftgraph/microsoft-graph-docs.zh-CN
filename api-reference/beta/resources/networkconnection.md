---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c587d9d6e11354a136948bbbf37565e42e0bb678
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522580"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="ab1c8-104">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab1c8-104">networkConnection resource type</span></span>

<span data-ttu-id="ab1c8-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ab1c8-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1c8-106">包含有关与警报相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-106">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="ab1c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="ab1c8-107">Properties</span></span>

| <span data-ttu-id="ab1c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab1c8-108">Property</span></span>   | <span data-ttu-id="ab1c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="ab1c8-109">Type</span></span>|<span data-ttu-id="ab1c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab1c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab1c8-111">applicationName</span><span class="sxs-lookup"><span data-stu-id="ab1c8-111">applicationName</span></span>|<span data-ttu-id="ab1c8-112">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-112">String</span></span>|<span data-ttu-id="ab1c8-113">管理网络连接的应用程序的名称（例如，Facebook、SMTP 等）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-113">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="ab1c8-114">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="ab1c8-114">destinationAddress</span></span>|<span data-ttu-id="ab1c8-115">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-115">String</span></span>|<span data-ttu-id="ab1c8-116">目标 IP 地址（的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-116">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="ab1c8-117">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="ab1c8-117">destinationDomain</span></span>|<span data-ttu-id="ab1c8-118">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-118">String</span></span>|<span data-ttu-id="ab1c8-119">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-119">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="ab1c8-120">（例如，"www.contoso.com"）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-120">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="ab1c8-121">destinationPort</span><span class="sxs-lookup"><span data-stu-id="ab1c8-121">destinationPort</span></span>|<span data-ttu-id="ab1c8-122">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-122">String</span></span>|<span data-ttu-id="ab1c8-123">目标端口（网络连接）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-123">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="ab1c8-124">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="ab1c8-124">destinationUrl</span></span>|<span data-ttu-id="ab1c8-125">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-125">String</span></span>|<span data-ttu-id="ab1c8-126">网络连接 URL/URI 字符串-不包括参数。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-126">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="ab1c8-127">（例如，"www.contoso.com/products/default.html"）</span><span class="sxs-lookup"><span data-stu-id="ab1c8-127">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="ab1c8-128">direction</span><span class="sxs-lookup"><span data-stu-id="ab1c8-128">direction</span></span>|<span data-ttu-id="ab1c8-129">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="ab1c8-129">connectionDirection</span></span>|<span data-ttu-id="ab1c8-130">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-130">Network connection direction.</span></span> <span data-ttu-id="ab1c8-131">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-131">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="ab1c8-132">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="ab1c8-132">domainRegisteredDateTime</span></span>|<span data-ttu-id="ab1c8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab1c8-133">DateTimeOffset</span></span>|<span data-ttu-id="ab1c8-134">注册目标域的日期。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-134">Date when the destination domain was registered.</span></span> <span data-ttu-id="ab1c8-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab1c8-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ab1c8-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ab1c8-137">localDnsName</span><span class="sxs-lookup"><span data-stu-id="ab1c8-137">localDnsName</span></span>|<span data-ttu-id="ab1c8-138">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-138">String</span></span>|<span data-ttu-id="ab1c8-139">在主机的本地 DNS 缓存中显示的本地 DNS 名称解析（例如，在 "主机" 文件被篡改的情况下）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-139">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="ab1c8-140">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="ab1c8-140">natDestinationAddress</span></span>|<span data-ttu-id="ab1c8-141">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-141">String</span></span>|<span data-ttu-id="ab1c8-142">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-142">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="ab1c8-143">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="ab1c8-143">natDestinationPort</span></span>|<span data-ttu-id="ab1c8-144">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-144">String</span></span>|<span data-ttu-id="ab1c8-145">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-145">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="ab1c8-146">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="ab1c8-146">natSourceAddress</span></span>|<span data-ttu-id="ab1c8-147">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-147">String</span></span>|<span data-ttu-id="ab1c8-148">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-148">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="ab1c8-149">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="ab1c8-149">natSourcePort</span></span>|<span data-ttu-id="ab1c8-150">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-150">String</span></span>|<span data-ttu-id="ab1c8-151">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-151">Network Address Translation source port.</span></span>|
|<span data-ttu-id="ab1c8-152">协议</span><span class="sxs-lookup"><span data-stu-id="ab1c8-152">protocol</span></span>|<span data-ttu-id="ab1c8-153">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="ab1c8-153">securityNetworkProtocol</span></span>|<span data-ttu-id="ab1c8-154">网络协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-154">Network protocol.</span></span> <span data-ttu-id="ab1c8-155">可能的值为`unknown`： `ip`、 `icmp`、 `igmp` `ggp` `ipv4` `tcp` `spx` `spxII`、、、、、、、、、、、、、、、、、、、、。 `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx`</span><span class="sxs-lookup"><span data-stu-id="ab1c8-155">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="ab1c8-156">riskScore</span><span class="sxs-lookup"><span data-stu-id="ab1c8-156">riskScore</span></span>|<span data-ttu-id="ab1c8-157">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-157">String</span></span>|<span data-ttu-id="ab1c8-158">提供程序生成/计算网络连接的风险分数。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-158">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="ab1c8-159">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-159">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="ab1c8-160">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="ab1c8-160">sourceAddress</span></span>|<span data-ttu-id="ab1c8-161">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-161">String</span></span>|<span data-ttu-id="ab1c8-162">源（即，网络连接的来源）的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-162">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="ab1c8-163">sourcePort</span><span class="sxs-lookup"><span data-stu-id="ab1c8-163">sourcePort</span></span>|<span data-ttu-id="ab1c8-164">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-164">String</span></span>|<span data-ttu-id="ab1c8-165">源（即源） IP 端口（的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-165">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="ab1c8-166">status</span><span class="sxs-lookup"><span data-stu-id="ab1c8-166">status</span></span>|<span data-ttu-id="ab1c8-167">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="ab1c8-167">connectionStatus</span></span>|<span data-ttu-id="ab1c8-168">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-168">Network connection status.</span></span> <span data-ttu-id="ab1c8-169">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-169">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="ab1c8-170">urlParameters</span><span class="sxs-lookup"><span data-stu-id="ab1c8-170">urlParameters</span></span>|<span data-ttu-id="ab1c8-171">String</span><span class="sxs-lookup"><span data-stu-id="ab1c8-171">String</span></span>|<span data-ttu-id="ab1c8-172">目标 URL 的参数（后缀）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-172">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="ab1c8-173">securityNetworkProtocol 值</span><span class="sxs-lookup"><span data-stu-id="ab1c8-173">securityNetworkProtocol values</span></span>

|<span data-ttu-id="ab1c8-174">成员</span><span class="sxs-lookup"><span data-stu-id="ab1c8-174">Member</span></span>|<span data-ttu-id="ab1c8-175">值</span><span class="sxs-lookup"><span data-stu-id="ab1c8-175">Value</span></span>|<span data-ttu-id="ab1c8-176">说明</span><span class="sxs-lookup"><span data-stu-id="ab1c8-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab1c8-177">unknown</span><span class="sxs-lookup"><span data-stu-id="ab1c8-177">unknown</span></span>|<span data-ttu-id="ab1c8-178">-1</span><span class="sxs-lookup"><span data-stu-id="ab1c8-178">-1</span></span>|<span data-ttu-id="ab1c8-179">未知协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-179">Unknown protocol.</span></span>|
|<span data-ttu-id="ab1c8-180">ip</span><span class="sxs-lookup"><span data-stu-id="ab1c8-180">ip</span></span>|<span data-ttu-id="ab1c8-181">0</span><span class="sxs-lookup"><span data-stu-id="ab1c8-181">0</span></span>|<span data-ttu-id="ab1c8-182">Internet 协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-182">Internet Protocol.</span></span>|
|<span data-ttu-id="ab1c8-183">icmp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-183">icmp</span></span>|<span data-ttu-id="ab1c8-184">1 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-184">1</span></span>| <span data-ttu-id="ab1c8-185">Internet 控制邮件协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-185">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="ab1c8-186">igmp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-186">igmp</span></span>|<span data-ttu-id="ab1c8-187">2 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-187">2</span></span>| <span data-ttu-id="ab1c8-188">Internet 组管理协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-188">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="ab1c8-189">ggp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-189">ggp</span></span>|<span data-ttu-id="ab1c8-190">3 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-190">3</span></span>| <span data-ttu-id="ab1c8-191">网关到网关协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-191">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="ab1c8-192">ipv4</span><span class="sxs-lookup"><span data-stu-id="ab1c8-192">ipv4</span></span>|<span data-ttu-id="ab1c8-193">4 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-193">4</span></span>| <span data-ttu-id="ab1c8-194">Internet 协议版本4。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-194">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="ab1c8-195">tcp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-195">tcp</span></span>|<span data-ttu-id="ab1c8-196">6 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-196">6</span></span>| <span data-ttu-id="ab1c8-197">传输控制协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-197">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="ab1c8-198">pup</span><span class="sxs-lookup"><span data-stu-id="ab1c8-198">pup</span></span>|<span data-ttu-id="ab1c8-199">12 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-199">12</span></span>| <span data-ttu-id="ab1c8-200">PARC 通用数据包协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-200">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="ab1c8-201">udp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-201">udp</span></span>|<span data-ttu-id="ab1c8-202">17 </span><span class="sxs-lookup"><span data-stu-id="ab1c8-202">17</span></span>| <span data-ttu-id="ab1c8-203">用户数据报协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-203">User Datagram Protocol.</span></span>|
|<span data-ttu-id="ab1c8-204">idp</span><span class="sxs-lookup"><span data-stu-id="ab1c8-204">idp</span></span>|<span data-ttu-id="ab1c8-205">22</span><span class="sxs-lookup"><span data-stu-id="ab1c8-205">22</span></span>| <span data-ttu-id="ab1c8-206">Internet 数据报协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-206">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="ab1c8-207">ipv4</span><span class="sxs-lookup"><span data-stu-id="ab1c8-207">ipv6</span></span>|<span data-ttu-id="ab1c8-208">41</span><span class="sxs-lookup"><span data-stu-id="ab1c8-208">41</span></span>| <span data-ttu-id="ab1c8-209">Internet 协议版本6（ipv6）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-209">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="ab1c8-210">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="ab1c8-210">ipv6RoutingHeader</span></span>|<span data-ttu-id="ab1c8-211">43</span><span class="sxs-lookup"><span data-stu-id="ab1c8-211">43</span></span>| <span data-ttu-id="ab1c8-212">ipv6 路由头。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-212">ipv6 Routing header.</span></span>|
|<span data-ttu-id="ab1c8-213">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="ab1c8-213">ipv6FragmentHeader</span></span>|<span data-ttu-id="ab1c8-214">44</span><span class="sxs-lookup"><span data-stu-id="ab1c8-214">44</span></span>| <span data-ttu-id="ab1c8-215">ipv6 分段标头。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-215">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="ab1c8-216">ipSecEncapsulatingSecurityPayload</span><span class="sxs-lookup"><span data-stu-id="ab1c8-216">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="ab1c8-217">50</span><span class="sxs-lookup"><span data-stu-id="ab1c8-217">50</span></span>| <span data-ttu-id="ab1c8-218">ipv6 封装安全有效负载标头。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-218">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="ab1c8-219">ipSecAuthenticationHeader</span><span class="sxs-lookup"><span data-stu-id="ab1c8-219">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="ab1c8-220">51</span><span class="sxs-lookup"><span data-stu-id="ab1c8-220">51</span></span>| <span data-ttu-id="ab1c8-221">ipv6 身份验证标头。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-221">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="ab1c8-222">icmpV6</span><span class="sxs-lookup"><span data-stu-id="ab1c8-222">icmpV6</span></span>|<span data-ttu-id="ab1c8-223">58</span><span class="sxs-lookup"><span data-stu-id="ab1c8-223">58</span></span>| <span data-ttu-id="ab1c8-224">Ipv6 的 Internet 控制消息协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-224">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="ab1c8-225">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="ab1c8-225">ipv6NoNextHeader</span></span>|<span data-ttu-id="ab1c8-226">59</span><span class="sxs-lookup"><span data-stu-id="ab1c8-226">59</span></span>| <span data-ttu-id="ab1c8-227">ipv6 无下一个标头。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-227">ipv6 No next header.</span></span>|
|<span data-ttu-id="ab1c8-228">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="ab1c8-228">ipv6DestinationOptions</span></span>|<span data-ttu-id="ab1c8-229">60</span><span class="sxs-lookup"><span data-stu-id="ab1c8-229">60</span></span>| <span data-ttu-id="ab1c8-230">ipv6 目标选项标头。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-230">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="ab1c8-231">点</span><span class="sxs-lookup"><span data-stu-id="ab1c8-231">nd</span></span>|<span data-ttu-id="ab1c8-232">77</span><span class="sxs-lookup"><span data-stu-id="ab1c8-232">77</span></span>| <span data-ttu-id="ab1c8-233">网络磁盘协议（非正式）。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-233">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="ab1c8-234">原始</span><span class="sxs-lookup"><span data-stu-id="ab1c8-234">raw</span></span>|<span data-ttu-id="ab1c8-235">255</span><span class="sxs-lookup"><span data-stu-id="ab1c8-235">255</span></span>| <span data-ttu-id="ab1c8-236">原始 IP 数据包协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-236">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="ab1c8-237">通讯</span><span class="sxs-lookup"><span data-stu-id="ab1c8-237">ipx</span></span>|<span data-ttu-id="ab1c8-238">1000</span><span class="sxs-lookup"><span data-stu-id="ab1c8-238">1000</span></span>| <span data-ttu-id="ab1c8-239">Internet 数据包交换协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-239">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="ab1c8-240">spx</span><span class="sxs-lookup"><span data-stu-id="ab1c8-240">spx</span></span>|<span data-ttu-id="ab1c8-241">1256</span><span class="sxs-lookup"><span data-stu-id="ab1c8-241">1256</span></span>| <span data-ttu-id="ab1c8-242">序列化的数据包交换协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-242">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="ab1c8-243">spxII</span><span class="sxs-lookup"><span data-stu-id="ab1c8-243">spxII</span></span>|<span data-ttu-id="ab1c8-244">1257</span><span class="sxs-lookup"><span data-stu-id="ab1c8-244">1257</span></span>| <span data-ttu-id="ab1c8-245">序列化数据包交换第2版协议。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-245">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab1c8-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab1c8-246">JSON representation</span></span>

<span data-ttu-id="ab1c8-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab1c8-247">The following is a JSON representation of the resource.</span></span>

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
