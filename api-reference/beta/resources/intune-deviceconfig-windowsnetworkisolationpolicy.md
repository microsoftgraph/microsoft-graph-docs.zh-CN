---
title: windowsNetworkIsolationPolicy 资源类型
description: Windows 网络隔离策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 78a598dab5c1eb003b09510f925506679bc432b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293435"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="925c4-103">windowsNetworkIsolationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="925c4-103">windowsNetworkIsolationPolicy resource type</span></span>

<span data-ttu-id="925c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="925c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="925c4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="925c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="925c4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="925c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="925c4-107">Windows 网络隔离策略</span><span class="sxs-lookup"><span data-stu-id="925c4-107">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="925c4-108">属性</span><span class="sxs-lookup"><span data-stu-id="925c4-108">Properties</span></span>
|<span data-ttu-id="925c4-109">属性</span><span class="sxs-lookup"><span data-stu-id="925c4-109">Property</span></span>|<span data-ttu-id="925c4-110">类型</span><span class="sxs-lookup"><span data-stu-id="925c4-110">Type</span></span>|<span data-ttu-id="925c4-111">Description</span><span class="sxs-lookup"><span data-stu-id="925c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="925c4-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="925c4-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="925c4-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="925c4-113">String collection</span></span>|<span data-ttu-id="925c4-114">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="925c4-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="925c4-115">来自发送到设备的这些域之一的数据将被视为企业数据并受保护。</span><span class="sxs-lookup"><span data-stu-id="925c4-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="925c4-116">这些位置将被视为要共享的企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="925c4-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="925c4-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="925c4-117">enterpriseCloudResources</span></span>|<span data-ttu-id="925c4-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="925c4-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="925c4-119">包含托管在需要受保护的云中的企业资源域的列表。</span><span class="sxs-lookup"><span data-stu-id="925c4-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="925c4-120">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="925c4-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="925c4-121">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="925c4-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="925c4-122">还必须使用 EnterpriseInternalProxyServers 策略配置用于此目的的代理服务器。</span><span class="sxs-lookup"><span data-stu-id="925c4-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="925c4-123">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="925c4-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="925c4-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="925c4-124">enterpriseIPRanges</span></span>|<span data-ttu-id="925c4-125">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="925c4-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="925c4-126">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="925c4-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="925c4-127">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="925c4-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="925c4-128">这些位置将被视为要共享的企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="925c4-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="925c4-129">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="925c4-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="925c4-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="925c4-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="925c4-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="925c4-131">String collection</span></span>|<span data-ttu-id="925c4-132">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="925c4-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="925c4-133">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="925c4-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="925c4-134">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="925c4-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="925c4-135">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="925c4-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="925c4-136">仅在配置 EnterpriseCloudResources 策略以通过这些代理将流量强制到匹配的云资源时，才会利用代理。</span><span class="sxs-lookup"><span data-stu-id="925c4-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="925c4-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="925c4-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="925c4-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="925c4-138">Boolean</span></span>|<span data-ttu-id="925c4-139">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="925c4-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="925c4-140">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="925c4-140">Default is false.</span></span>|
|<span data-ttu-id="925c4-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="925c4-141">enterpriseProxyServers</span></span>|<span data-ttu-id="925c4-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="925c4-142">String collection</span></span>|<span data-ttu-id="925c4-143">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="925c4-143">This is a list of proxy servers.</span></span> <span data-ttu-id="925c4-144">任何不在此列表中的服务器都被视为非企业服务器。</span><span class="sxs-lookup"><span data-stu-id="925c4-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="925c4-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="925c4-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="925c4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="925c4-146">Boolean</span></span>|<span data-ttu-id="925c4-147">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="925c4-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="925c4-148">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="925c4-148">Default is false</span></span>|
|<span data-ttu-id="925c4-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="925c4-149">neutralDomainResources</span></span>|<span data-ttu-id="925c4-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="925c4-150">String collection</span></span>|<span data-ttu-id="925c4-151">可用于工作或个人资源的域名列表。</span><span class="sxs-lookup"><span data-stu-id="925c4-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="925c4-152">关系</span><span class="sxs-lookup"><span data-stu-id="925c4-152">Relationships</span></span>
<span data-ttu-id="925c4-153">无</span><span class="sxs-lookup"><span data-stu-id="925c4-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="925c4-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="925c4-154">JSON Representation</span></span>
<span data-ttu-id="925c4-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="925c4-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.ipRange"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```




