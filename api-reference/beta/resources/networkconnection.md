---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 94bf27265f591d32c01e7043d3a10468a924d78a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342196"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="47bed-104">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="47bed-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47bed-105">包含有关与警报相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="47bed-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="47bed-106">属性</span><span class="sxs-lookup"><span data-stu-id="47bed-106">Properties</span></span>

| <span data-ttu-id="47bed-107">属性</span><span class="sxs-lookup"><span data-stu-id="47bed-107">Property</span></span>   | <span data-ttu-id="47bed-108">类型</span><span class="sxs-lookup"><span data-stu-id="47bed-108">Type</span></span>|<span data-ttu-id="47bed-109">说明</span><span class="sxs-lookup"><span data-stu-id="47bed-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47bed-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="47bed-110">applicationName</span></span>|<span data-ttu-id="47bed-111">String</span><span class="sxs-lookup"><span data-stu-id="47bed-111">String</span></span>|<span data-ttu-id="47bed-112">管理网络连接的应用程序的名称 (例如, Facebook、SMTP 等)。</span><span class="sxs-lookup"><span data-stu-id="47bed-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="47bed-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="47bed-113">destinationAddress</span></span>|<span data-ttu-id="47bed-114">String</span><span class="sxs-lookup"><span data-stu-id="47bed-114">String</span></span>|<span data-ttu-id="47bed-115">目标 IP 地址 (的网络连接)。</span><span class="sxs-lookup"><span data-stu-id="47bed-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="47bed-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="47bed-116">destinationDomain</span></span>|<span data-ttu-id="47bed-117">String</span><span class="sxs-lookup"><span data-stu-id="47bed-117">String</span></span>|<span data-ttu-id="47bed-118">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="47bed-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="47bed-119">(例如, "www.contoso.com")。</span><span class="sxs-lookup"><span data-stu-id="47bed-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="47bed-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="47bed-120">destinationPort</span></span>|<span data-ttu-id="47bed-121">String</span><span class="sxs-lookup"><span data-stu-id="47bed-121">String</span></span>|<span data-ttu-id="47bed-122">目标端口 (网络连接)。</span><span class="sxs-lookup"><span data-stu-id="47bed-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="47bed-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="47bed-123">destinationUrl</span></span>|<span data-ttu-id="47bed-124">String</span><span class="sxs-lookup"><span data-stu-id="47bed-124">String</span></span>|<span data-ttu-id="47bed-125">网络连接 URL/URI 字符串-不包括参数。</span><span class="sxs-lookup"><span data-stu-id="47bed-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="47bed-126">(例如, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="47bed-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="47bed-127">direction</span><span class="sxs-lookup"><span data-stu-id="47bed-127">direction</span></span>|<span data-ttu-id="47bed-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="47bed-128">connectionDirection</span></span>|<span data-ttu-id="47bed-129">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="47bed-129">Network connection direction.</span></span> <span data-ttu-id="47bed-130">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="47bed-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="47bed-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="47bed-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="47bed-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47bed-132">DateTimeOffset</span></span>|<span data-ttu-id="47bed-133">注册目标域的日期。</span><span class="sxs-lookup"><span data-stu-id="47bed-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="47bed-134">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="47bed-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="47bed-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="47bed-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="47bed-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="47bed-136">localDnsName</span></span>|<span data-ttu-id="47bed-137">String</span><span class="sxs-lookup"><span data-stu-id="47bed-137">String</span></span>|<span data-ttu-id="47bed-138">在主机的本地 dns 缓存中显示的本地 dns 名称解析 (例如, 在 "主机" 文件被篡改的情况下)。</span><span class="sxs-lookup"><span data-stu-id="47bed-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="47bed-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="47bed-139">natDestinationAddress</span></span>|<span data-ttu-id="47bed-140">String</span><span class="sxs-lookup"><span data-stu-id="47bed-140">String</span></span>|<span data-ttu-id="47bed-141">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="47bed-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="47bed-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="47bed-142">natDestinationPort</span></span>|<span data-ttu-id="47bed-143">String</span><span class="sxs-lookup"><span data-stu-id="47bed-143">String</span></span>|<span data-ttu-id="47bed-144">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="47bed-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="47bed-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="47bed-145">natSourceAddress</span></span>|<span data-ttu-id="47bed-146">String</span><span class="sxs-lookup"><span data-stu-id="47bed-146">String</span></span>|<span data-ttu-id="47bed-147">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="47bed-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="47bed-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="47bed-148">natSourcePort</span></span>|<span data-ttu-id="47bed-149">String</span><span class="sxs-lookup"><span data-stu-id="47bed-149">String</span></span>|<span data-ttu-id="47bed-150">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="47bed-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="47bed-151">协议</span><span class="sxs-lookup"><span data-stu-id="47bed-151">protocol</span></span>|<span data-ttu-id="47bed-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="47bed-152">securityNetworkProtocol</span></span>|<span data-ttu-id="47bed-153">网络协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-153">Network protocol.</span></span> <span data-ttu-id="47bed-154">可能的值为`unknown`: `ip`、 `icmp`、 `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader`、、、、、、、、、、、、、、、、 `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="47bed-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="47bed-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="47bed-155">riskScore</span></span>|<span data-ttu-id="47bed-156">String</span><span class="sxs-lookup"><span data-stu-id="47bed-156">String</span></span>|<span data-ttu-id="47bed-157">提供程序生成/计算网络连接的风险分数。</span><span class="sxs-lookup"><span data-stu-id="47bed-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="47bed-158">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="47bed-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="47bed-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="47bed-159">sourceAddress</span></span>|<span data-ttu-id="47bed-160">String</span><span class="sxs-lookup"><span data-stu-id="47bed-160">String</span></span>|<span data-ttu-id="47bed-161">源 (即, 网络连接的来源) 的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="47bed-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="47bed-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="47bed-162">sourcePort</span></span>|<span data-ttu-id="47bed-163">String</span><span class="sxs-lookup"><span data-stu-id="47bed-163">String</span></span>|<span data-ttu-id="47bed-164">源 (即源) IP 端口 (的网络连接)。</span><span class="sxs-lookup"><span data-stu-id="47bed-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="47bed-165">status</span><span class="sxs-lookup"><span data-stu-id="47bed-165">status</span></span>|<span data-ttu-id="47bed-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="47bed-166">connectionStatus</span></span>|<span data-ttu-id="47bed-167">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="47bed-167">Network connection status.</span></span> <span data-ttu-id="47bed-168">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="47bed-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="47bed-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="47bed-169">urlParameters</span></span>|<span data-ttu-id="47bed-170">String</span><span class="sxs-lookup"><span data-stu-id="47bed-170">String</span></span>|<span data-ttu-id="47bed-171">目标 URL 的参数 (后缀)。</span><span class="sxs-lookup"><span data-stu-id="47bed-171">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="47bed-172">securityNetworkProtocol 值</span><span class="sxs-lookup"><span data-stu-id="47bed-172">securityNetworkProtocol values</span></span>

|<span data-ttu-id="47bed-173">成员</span><span class="sxs-lookup"><span data-stu-id="47bed-173">Member</span></span>|<span data-ttu-id="47bed-174">值</span><span class="sxs-lookup"><span data-stu-id="47bed-174">Value</span></span>|<span data-ttu-id="47bed-175">说明</span><span class="sxs-lookup"><span data-stu-id="47bed-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47bed-176">unknown</span><span class="sxs-lookup"><span data-stu-id="47bed-176">unknown</span></span>|<span data-ttu-id="47bed-177">-1</span><span class="sxs-lookup"><span data-stu-id="47bed-177">-1</span></span>|<span data-ttu-id="47bed-178">未知协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-178">Unknown protocol.</span></span>|
|<span data-ttu-id="47bed-179">ip</span><span class="sxs-lookup"><span data-stu-id="47bed-179">ip</span></span>|<span data-ttu-id="47bed-180">0</span><span class="sxs-lookup"><span data-stu-id="47bed-180">0</span></span>|<span data-ttu-id="47bed-181">Internet 协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-181">Internet Protocol.</span></span>|
|<span data-ttu-id="47bed-182">icmp</span><span class="sxs-lookup"><span data-stu-id="47bed-182">icmp</span></span>|<span data-ttu-id="47bed-183">1</span><span class="sxs-lookup"><span data-stu-id="47bed-183">1</span></span>| <span data-ttu-id="47bed-184">Internet 控制邮件协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-184">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="47bed-185">igmp</span><span class="sxs-lookup"><span data-stu-id="47bed-185">igmp</span></span>|<span data-ttu-id="47bed-186">双面</span><span class="sxs-lookup"><span data-stu-id="47bed-186">2</span></span>| <span data-ttu-id="47bed-187">Internet 组管理协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-187">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="47bed-188">ggp</span><span class="sxs-lookup"><span data-stu-id="47bed-188">ggp</span></span>|<span data-ttu-id="47bed-189">第三章</span><span class="sxs-lookup"><span data-stu-id="47bed-189">3</span></span>| <span data-ttu-id="47bed-190">网关到网关协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-190">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="47bed-191">ipv4</span><span class="sxs-lookup"><span data-stu-id="47bed-191">ipv4</span></span>|<span data-ttu-id="47bed-192">4</span><span class="sxs-lookup"><span data-stu-id="47bed-192">4</span></span>| <span data-ttu-id="47bed-193">Internet 协议版本4。</span><span class="sxs-lookup"><span data-stu-id="47bed-193">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="47bed-194">tcp</span><span class="sxs-lookup"><span data-stu-id="47bed-194">tcp</span></span>|<span data-ttu-id="47bed-195">型</span><span class="sxs-lookup"><span data-stu-id="47bed-195">6</span></span>| <span data-ttu-id="47bed-196">传输控制协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-196">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="47bed-197">pup</span><span class="sxs-lookup"><span data-stu-id="47bed-197">pup</span></span>|<span data-ttu-id="47bed-198">12 </span><span class="sxs-lookup"><span data-stu-id="47bed-198">12</span></span>| <span data-ttu-id="47bed-199">PARC 通用数据包协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-199">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="47bed-200">udp</span><span class="sxs-lookup"><span data-stu-id="47bed-200">udp</span></span>|<span data-ttu-id="47bed-201">×</span><span class="sxs-lookup"><span data-stu-id="47bed-201">17</span></span>| <span data-ttu-id="47bed-202">用户数据报协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-202">User Datagram Protocol.</span></span>|
|<span data-ttu-id="47bed-203">idp</span><span class="sxs-lookup"><span data-stu-id="47bed-203">idp</span></span>|<span data-ttu-id="47bed-204">22</span><span class="sxs-lookup"><span data-stu-id="47bed-204">22</span></span>| <span data-ttu-id="47bed-205">Internet 数据报协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-205">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="47bed-206">ipv4</span><span class="sxs-lookup"><span data-stu-id="47bed-206">ipv6</span></span>|<span data-ttu-id="47bed-207">41</span><span class="sxs-lookup"><span data-stu-id="47bed-207">41</span></span>| <span data-ttu-id="47bed-208">Internet 协议版本 6 (ipv6)。</span><span class="sxs-lookup"><span data-stu-id="47bed-208">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="47bed-209">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="47bed-209">ipv6RoutingHeader</span></span>|<span data-ttu-id="47bed-210">43</span><span class="sxs-lookup"><span data-stu-id="47bed-210">43</span></span>| <span data-ttu-id="47bed-211">ipv6 路由头。</span><span class="sxs-lookup"><span data-stu-id="47bed-211">ipv6 Routing header.</span></span>|
|<span data-ttu-id="47bed-212">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="47bed-212">ipv6FragmentHeader</span></span>|<span data-ttu-id="47bed-213">44</span><span class="sxs-lookup"><span data-stu-id="47bed-213">44</span></span>| <span data-ttu-id="47bed-214">ipv6 分段标头。</span><span class="sxs-lookup"><span data-stu-id="47bed-214">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="47bed-215">ipSecEncapsulatingSecurityPayload</span><span class="sxs-lookup"><span data-stu-id="47bed-215">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="47bed-216">50</span><span class="sxs-lookup"><span data-stu-id="47bed-216">50</span></span>| <span data-ttu-id="47bed-217">ipv6 封装安全有效负载标头。</span><span class="sxs-lookup"><span data-stu-id="47bed-217">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="47bed-218">ipSecAuthenticationHeader</span><span class="sxs-lookup"><span data-stu-id="47bed-218">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="47bed-219">51</span><span class="sxs-lookup"><span data-stu-id="47bed-219">51</span></span>| <span data-ttu-id="47bed-220">ipv6 身份验证标头。</span><span class="sxs-lookup"><span data-stu-id="47bed-220">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="47bed-221">icmpV6</span><span class="sxs-lookup"><span data-stu-id="47bed-221">icmpV6</span></span>|<span data-ttu-id="47bed-222">58</span><span class="sxs-lookup"><span data-stu-id="47bed-222">58</span></span>| <span data-ttu-id="47bed-223">ipv6 的 Internet 控制消息协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-223">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="47bed-224">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="47bed-224">ipv6NoNextHeader</span></span>|<span data-ttu-id="47bed-225">59</span><span class="sxs-lookup"><span data-stu-id="47bed-225">59</span></span>| <span data-ttu-id="47bed-226">ipv6 无下一个标头。</span><span class="sxs-lookup"><span data-stu-id="47bed-226">ipv6 No next header.</span></span>|
|<span data-ttu-id="47bed-227">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="47bed-227">ipv6DestinationOptions</span></span>|<span data-ttu-id="47bed-228">60</span><span class="sxs-lookup"><span data-stu-id="47bed-228">60</span></span>| <span data-ttu-id="47bed-229">ipv6 目标选项标头。</span><span class="sxs-lookup"><span data-stu-id="47bed-229">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="47bed-230">点</span><span class="sxs-lookup"><span data-stu-id="47bed-230">nd</span></span>|<span data-ttu-id="47bed-231">77</span><span class="sxs-lookup"><span data-stu-id="47bed-231">77</span></span>| <span data-ttu-id="47bed-232">网络磁盘协议 (非正式)。</span><span class="sxs-lookup"><span data-stu-id="47bed-232">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="47bed-233">原始</span><span class="sxs-lookup"><span data-stu-id="47bed-233">raw</span></span>|<span data-ttu-id="47bed-234">255</span><span class="sxs-lookup"><span data-stu-id="47bed-234">255</span></span>| <span data-ttu-id="47bed-235">原始 IP 数据包协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-235">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="47bed-236">通讯</span><span class="sxs-lookup"><span data-stu-id="47bed-236">ipx</span></span>|<span data-ttu-id="47bed-237">1000</span><span class="sxs-lookup"><span data-stu-id="47bed-237">1000</span></span>| <span data-ttu-id="47bed-238">Internet 数据包交换协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-238">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="47bed-239">spx</span><span class="sxs-lookup"><span data-stu-id="47bed-239">spx</span></span>|<span data-ttu-id="47bed-240">1256</span><span class="sxs-lookup"><span data-stu-id="47bed-240">1256</span></span>| <span data-ttu-id="47bed-241">序列化的数据包交换协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-241">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="47bed-242">spxII</span><span class="sxs-lookup"><span data-stu-id="47bed-242">spxII</span></span>|<span data-ttu-id="47bed-243">1257</span><span class="sxs-lookup"><span data-stu-id="47bed-243">1257</span></span>| <span data-ttu-id="47bed-244">序列化数据包交换第2版协议。</span><span class="sxs-lookup"><span data-stu-id="47bed-244">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47bed-245">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47bed-245">JSON representation</span></span>

<span data-ttu-id="47bed-246">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47bed-246">The following is a JSON representation of the resource.</span></span>

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
