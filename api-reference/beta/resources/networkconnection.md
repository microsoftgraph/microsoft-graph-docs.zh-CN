---
title: networkConnection 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 6d28149854ed3157473b678db442ee3474e456c6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571917"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="59595-104">networkConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="59595-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59595-105">包含有关与通知相关的网络连接的状态信息。</span><span class="sxs-lookup"><span data-stu-id="59595-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="59595-106">属性</span><span class="sxs-lookup"><span data-stu-id="59595-106">Properties</span></span>

| <span data-ttu-id="59595-107">属性</span><span class="sxs-lookup"><span data-stu-id="59595-107">Property</span></span>   | <span data-ttu-id="59595-108">类型</span><span class="sxs-lookup"><span data-stu-id="59595-108">Type</span></span>|<span data-ttu-id="59595-109">说明</span><span class="sxs-lookup"><span data-stu-id="59595-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59595-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="59595-110">applicationName</span></span>|<span data-ttu-id="59595-111">String</span><span class="sxs-lookup"><span data-stu-id="59595-111">String</span></span>|<span data-ttu-id="59595-112">管理网络连接 （例如，Facebook、 SMTP 等） 的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="59595-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="59595-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="59595-113">destinationAddress</span></span>|<span data-ttu-id="59595-114">String</span><span class="sxs-lookup"><span data-stu-id="59595-114">String</span></span>|<span data-ttu-id="59595-115">目标 IP 地址 （的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="59595-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="59595-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="59595-116">destinationDomain</span></span>|<span data-ttu-id="59595-117">String</span><span class="sxs-lookup"><span data-stu-id="59595-117">String</span></span>|<span data-ttu-id="59595-118">目标 URL 的目标域部分。</span><span class="sxs-lookup"><span data-stu-id="59595-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="59595-119">(例如 www.contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="59595-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="59595-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="59595-120">destinationPort</span></span>|<span data-ttu-id="59595-121">String</span><span class="sxs-lookup"><span data-stu-id="59595-121">String</span></span>|<span data-ttu-id="59595-122">目标端口 （的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="59595-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="59595-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="59595-123">destinationUrl</span></span>|<span data-ttu-id="59595-124">String</span><span class="sxs-lookup"><span data-stu-id="59595-124">String</span></span>|<span data-ttu-id="59595-125">网络连接 URL/URI 字符串-排除参数。</span><span class="sxs-lookup"><span data-stu-id="59595-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="59595-126">(例如 www.contoso.com/products/default.html)</span><span class="sxs-lookup"><span data-stu-id="59595-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="59595-127">direction</span><span class="sxs-lookup"><span data-stu-id="59595-127">direction</span></span>|<span data-ttu-id="59595-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="59595-128">connectionDirection</span></span>|<span data-ttu-id="59595-129">网络连接方向。</span><span class="sxs-lookup"><span data-stu-id="59595-129">Network connection direction.</span></span> <span data-ttu-id="59595-130">可取值为：`unknown`、`inbound`、`outbound`。</span><span class="sxs-lookup"><span data-stu-id="59595-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="59595-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="59595-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="59595-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59595-132">DateTimeOffset</span></span>|<span data-ttu-id="59595-133">目标域注册时的日期。</span><span class="sxs-lookup"><span data-stu-id="59595-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="59595-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="59595-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="59595-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="59595-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="59595-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="59595-136">localDnsName</span></span>|<span data-ttu-id="59595-137">String</span><span class="sxs-lookup"><span data-stu-id="59595-137">String</span></span>|<span data-ttu-id="59595-138">在本地 DNS 名称解析 （例如，在情况下的主机文件已被篡改） 出现在主机的本地 DNS 缓存中。</span><span class="sxs-lookup"><span data-stu-id="59595-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="59595-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="59595-139">natDestinationAddress</span></span>|<span data-ttu-id="59595-140">String</span><span class="sxs-lookup"><span data-stu-id="59595-140">String</span></span>|<span data-ttu-id="59595-141">网络地址转换目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="59595-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="59595-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="59595-142">natDestinationPort</span></span>|<span data-ttu-id="59595-143">String</span><span class="sxs-lookup"><span data-stu-id="59595-143">String</span></span>|<span data-ttu-id="59595-144">网络地址转换目标端口。</span><span class="sxs-lookup"><span data-stu-id="59595-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="59595-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="59595-145">natSourceAddress</span></span>|<span data-ttu-id="59595-146">String</span><span class="sxs-lookup"><span data-stu-id="59595-146">String</span></span>|<span data-ttu-id="59595-147">网络地址转换源 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="59595-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="59595-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="59595-148">natSourcePort</span></span>|<span data-ttu-id="59595-149">String</span><span class="sxs-lookup"><span data-stu-id="59595-149">String</span></span>|<span data-ttu-id="59595-150">网络地址转换源端口。</span><span class="sxs-lookup"><span data-stu-id="59595-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="59595-151">protocol</span><span class="sxs-lookup"><span data-stu-id="59595-151">protocol</span></span>| <span data-ttu-id="59595-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="59595-152">securityNetworkProtocol</span></span> |<span data-ttu-id="59595-153">网络协议。</span><span class="sxs-lookup"><span data-stu-id="59595-153">Network protocol.</span></span> <span data-ttu-id="59595-154">可能的值为： `unknown`， `ip`， `icmp`， `igmp`， `ggp`， `ipv4`， `tcp`， `pup`， `udp`， `idp`， `ipv6`， `ipv6RoutingHeader`， `ipv6FragmentHeader`， `ipSecEncapsulatingSecurityPayload`， `ipSecAuthenticationHeader`， `icmpV6`， `ipv6NoNextHeader`， `ipv6DestinationOptions`， `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="59595-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="59595-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="59595-155">riskScore</span></span>|<span data-ttu-id="59595-156">String</span><span class="sxs-lookup"><span data-stu-id="59595-156">String</span></span>|<span data-ttu-id="59595-157">提供程序生成/计算风险的网络连接的分数。</span><span class="sxs-lookup"><span data-stu-id="59595-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="59595-158">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="59595-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="59595-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="59595-159">sourceAddress</span></span>|<span data-ttu-id="59595-160">String</span><span class="sxs-lookup"><span data-stu-id="59595-160">String</span></span>|<span data-ttu-id="59595-161">源 （即原点） IP 地址 （的网络连接）。</span><span class="sxs-lookup"><span data-stu-id="59595-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="59595-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="59595-162">sourcePort</span></span>|<span data-ttu-id="59595-163">String</span><span class="sxs-lookup"><span data-stu-id="59595-163">String</span></span>|<span data-ttu-id="59595-164">源 （即原点） IP （网络连接端口）。</span><span class="sxs-lookup"><span data-stu-id="59595-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="59595-165">status</span><span class="sxs-lookup"><span data-stu-id="59595-165">status</span></span>|<span data-ttu-id="59595-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="59595-166">connectionStatus</span></span>|<span data-ttu-id="59595-167">网络连接状态。</span><span class="sxs-lookup"><span data-stu-id="59595-167">Network connection status.</span></span> <span data-ttu-id="59595-168">可取值为：`unknown`、`attempted`、`succeeded`、`blocked`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="59595-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="59595-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="59595-169">urlParameters</span></span>|<span data-ttu-id="59595-170">String</span><span class="sxs-lookup"><span data-stu-id="59595-170">String</span></span>|<span data-ttu-id="59595-171">目标 URL 参数 （后缀）。</span><span class="sxs-lookup"><span data-stu-id="59595-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59595-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59595-172">JSON representation</span></span>

<span data-ttu-id="59595-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59595-173">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
