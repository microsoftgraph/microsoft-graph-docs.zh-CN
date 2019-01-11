---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: a20520a729076c7e63079c6dfc803659ace45b9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880057"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="1046f-104">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="1046f-104">networkConnection resource type</span></span>

 > <span data-ttu-id="1046f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1046f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1046f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1046f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1046f-107">包含有关与通知相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="1046f-107">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="1046f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1046f-108">Properties</span></span>

| <span data-ttu-id="1046f-109">属性</span><span class="sxs-lookup"><span data-stu-id="1046f-109">Property</span></span>   | <span data-ttu-id="1046f-110">类型</span><span class="sxs-lookup"><span data-stu-id="1046f-110">Type</span></span>|<span data-ttu-id="1046f-111">Description</span><span class="sxs-lookup"><span data-stu-id="1046f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1046f-112">applicationName</span><span class="sxs-lookup"><span data-stu-id="1046f-112">applicationName</span></span>|<span data-ttu-id="1046f-113">String</span><span class="sxs-lookup"><span data-stu-id="1046f-113">String</span></span>|<span data-ttu-id="1046f-114">管理网络连接 （例如，Facebook、 SMTP 等） 的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="1046f-114">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="1046f-115">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="1046f-115">destinationAddress</span></span>|<span data-ttu-id="1046f-116">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-116">String</span></span>|<span data-ttu-id="1046f-117">目标 IP 地址 （的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="1046f-117">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="1046f-118">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="1046f-118">destinationDomain</span></span>|<span data-ttu-id="1046f-119">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-119">String</span></span>|<span data-ttu-id="1046f-120">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="1046f-120">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="1046f-121">(例如 www.contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="1046f-121">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="1046f-122">destinationPort</span><span class="sxs-lookup"><span data-stu-id="1046f-122">destinationPort</span></span>|<span data-ttu-id="1046f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-123">String</span></span>|<span data-ttu-id="1046f-124">目标端口 （的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="1046f-124">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="1046f-125">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="1046f-125">destinationUrl</span></span>|<span data-ttu-id="1046f-126">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-126">String</span></span>|<span data-ttu-id="1046f-127">网络连接 URL/URI 字符串-排除参数。</span><span class="sxs-lookup"><span data-stu-id="1046f-127">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="1046f-128">(例如 www.contoso.com/products/default.html)</span><span class="sxs-lookup"><span data-stu-id="1046f-128">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="1046f-129">方向</span><span class="sxs-lookup"><span data-stu-id="1046f-129">direction</span></span>|<span data-ttu-id="1046f-130">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="1046f-130">connectionDirection</span></span>|<span data-ttu-id="1046f-131">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="1046f-131">Network connection direction.</span></span> <span data-ttu-id="1046f-132">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="1046f-132">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="1046f-133">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="1046f-133">domainRegisteredDateTime</span></span>|<span data-ttu-id="1046f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1046f-134">DateTimeOffset</span></span>|<span data-ttu-id="1046f-135">目标域注册时的日期。</span><span class="sxs-lookup"><span data-stu-id="1046f-135">Date when the destination domain was registered.</span></span> <span data-ttu-id="1046f-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1046f-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1046f-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1046f-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1046f-138">localDnsName</span><span class="sxs-lookup"><span data-stu-id="1046f-138">localDnsName</span></span>|<span data-ttu-id="1046f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-139">String</span></span>|<span data-ttu-id="1046f-140">在本地 DNS 名称解析 （例如，在情况下的主机文件已被篡改） 出现在主机的本地 DNS 缓存中。</span><span class="sxs-lookup"><span data-stu-id="1046f-140">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="1046f-141">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="1046f-141">natDestinationAddress</span></span>|<span data-ttu-id="1046f-142">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-142">String</span></span>|<span data-ttu-id="1046f-143">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="1046f-143">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="1046f-144">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="1046f-144">natDestinationPort</span></span>|<span data-ttu-id="1046f-145">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-145">String</span></span>|<span data-ttu-id="1046f-146">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="1046f-146">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="1046f-147">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="1046f-147">natSourceAddress</span></span>|<span data-ttu-id="1046f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-148">String</span></span>|<span data-ttu-id="1046f-149">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="1046f-149">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="1046f-150">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="1046f-150">natSourcePort</span></span>|<span data-ttu-id="1046f-151">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-151">String</span></span>|<span data-ttu-id="1046f-152">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="1046f-152">Network Address Translation source port.</span></span>|
|<span data-ttu-id="1046f-153">protocol</span><span class="sxs-lookup"><span data-stu-id="1046f-153">protocol</span></span>|[<span data-ttu-id="1046f-154">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="1046f-154">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="1046f-155">网络协议。</span><span class="sxs-lookup"><span data-stu-id="1046f-155">Network protocol.</span></span> <span data-ttu-id="1046f-156">可能的值为： `unknown`， `ip`， `icmp`， `igmp`， `ggp`， `ipv4`， `tcp`， `pup`， `udp`， `idp`， `ipv6`， `ipv6RoutingHeader`， `ipv6FragmentHeader`， `ipSecEncapsulatingSecurityPayload`， `ipSecAuthenticationHeader`， `icmpV6`， `ipv6NoNextHeader`， `ipv6DestinationOptions`， `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="1046f-156">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="1046f-157">riskScore</span><span class="sxs-lookup"><span data-stu-id="1046f-157">riskScore</span></span>|<span data-ttu-id="1046f-158">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-158">String</span></span>|<span data-ttu-id="1046f-159">提供程序生成/计算风险的网络连接的分数。</span><span class="sxs-lookup"><span data-stu-id="1046f-159">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="1046f-160">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="1046f-160">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="1046f-161">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="1046f-161">sourceAddress</span></span>|<span data-ttu-id="1046f-162">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-162">String</span></span>|<span data-ttu-id="1046f-163">源 （即原点） IP 地址 （的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="1046f-163">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="1046f-164">sourcePort</span><span class="sxs-lookup"><span data-stu-id="1046f-164">sourcePort</span></span>|<span data-ttu-id="1046f-165">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-165">String</span></span>|<span data-ttu-id="1046f-166">源 （即原点） IP （网络连接端口）。</span><span class="sxs-lookup"><span data-stu-id="1046f-166">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="1046f-167">status</span><span class="sxs-lookup"><span data-stu-id="1046f-167">status</span></span>|<span data-ttu-id="1046f-168">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="1046f-168">connectionStatus</span></span>|<span data-ttu-id="1046f-169">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="1046f-169">Network connection status.</span></span> <span data-ttu-id="1046f-170">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="1046f-170">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="1046f-171">urlParameters</span><span class="sxs-lookup"><span data-stu-id="1046f-171">urlParameters</span></span>|<span data-ttu-id="1046f-172">字符串</span><span class="sxs-lookup"><span data-stu-id="1046f-172">String</span></span>|<span data-ttu-id="1046f-173">目标 URL 参数 （后缀）。</span><span class="sxs-lookup"><span data-stu-id="1046f-173">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1046f-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1046f-174">JSON representation</span></span>

<span data-ttu-id="1046f-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1046f-175">The following is a JSON representation of the resource.</span></span>

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
