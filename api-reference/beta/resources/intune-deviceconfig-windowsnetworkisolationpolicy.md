---
title: windowsNetworkIsolationPolicy 资源类型
description: Windows 网络隔离策略
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f025726cfd9bcd90be102293cb2cb81db3b46778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968811"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="c4889-103">windowsNetworkIsolationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4889-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="c4889-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4889-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4889-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4889-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4889-106">Windows 网络隔离策略</span><span class="sxs-lookup"><span data-stu-id="c4889-106">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="c4889-107">属性</span><span class="sxs-lookup"><span data-stu-id="c4889-107">Properties</span></span>
|<span data-ttu-id="c4889-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4889-108">Property</span></span>|<span data-ttu-id="c4889-109">类型</span><span class="sxs-lookup"><span data-stu-id="c4889-109">Type</span></span>|<span data-ttu-id="c4889-110">说明</span><span class="sxs-lookup"><span data-stu-id="c4889-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4889-111">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="c4889-111">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="c4889-112">String collection</span><span class="sxs-lookup"><span data-stu-id="c4889-112">String collection</span></span>|<span data-ttu-id="c4889-113">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="c4889-113">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="c4889-114">来自发送到设备的这些域之一的数据将被视为企业数据并受保护。</span><span class="sxs-lookup"><span data-stu-id="c4889-114">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="c4889-115">这些位置将被视为要共享的企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="c4889-115">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="c4889-116">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="c4889-116">enterpriseCloudResources</span></span>|<span data-ttu-id="c4889-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c4889-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="c4889-118">包含托管在需要受保护的云中的企业资源域的列表。</span><span class="sxs-lookup"><span data-stu-id="c4889-118">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="c4889-119">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="c4889-119">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="c4889-120">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="c4889-120">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="c4889-121">还必须使用 EnterpriseInternalProxyServers 策略配置用于此目的的代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c4889-121">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="c4889-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c4889-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c4889-123">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="c4889-123">enterpriseIPRanges</span></span>|<span data-ttu-id="c4889-124">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c4889-124">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="c4889-125">设置定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="c4889-125">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="c4889-126">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="c4889-126">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="c4889-127">这些位置将被视为要共享的企业数据的安全目标。</span><span class="sxs-lookup"><span data-stu-id="c4889-127">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="c4889-128">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c4889-128">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c4889-129">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="c4889-129">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="c4889-130">String collection</span><span class="sxs-lookup"><span data-stu-id="c4889-130">String collection</span></span>|<span data-ttu-id="c4889-131">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="c4889-131">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="c4889-132">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="c4889-132">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="c4889-133">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="c4889-133">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="c4889-134">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="c4889-134">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="c4889-135">仅在配置 EnterpriseCloudResources 策略以通过这些代理将流量强制到匹配的云资源时, 才会利用代理。</span><span class="sxs-lookup"><span data-stu-id="c4889-135">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="c4889-136">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c4889-136">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="c4889-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4889-137">Boolean</span></span>|<span data-ttu-id="c4889-138">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c4889-138">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="c4889-139">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="c4889-139">Default is false.</span></span>|
|<span data-ttu-id="c4889-140">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="c4889-140">enterpriseProxyServers</span></span>|<span data-ttu-id="c4889-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c4889-141">String collection</span></span>|<span data-ttu-id="c4889-142">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="c4889-142">This is a list of proxy servers.</span></span> <span data-ttu-id="c4889-143">任何不在此列表中的服务器都被视为非企业服务器。</span><span class="sxs-lookup"><span data-stu-id="c4889-143">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="c4889-144">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="c4889-144">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="c4889-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4889-145">Boolean</span></span>|<span data-ttu-id="c4889-146">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c4889-146">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="c4889-147">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="c4889-147">Default is false</span></span>|
|<span data-ttu-id="c4889-148">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="c4889-148">neutralDomainResources</span></span>|<span data-ttu-id="c4889-149">String collection</span><span class="sxs-lookup"><span data-stu-id="c4889-149">String collection</span></span>|<span data-ttu-id="c4889-150">可用于工作或个人资源的域名列表。</span><span class="sxs-lookup"><span data-stu-id="c4889-150">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4889-151">关系</span><span class="sxs-lookup"><span data-stu-id="c4889-151">Relationships</span></span>
<span data-ttu-id="c4889-152">无</span><span class="sxs-lookup"><span data-stu-id="c4889-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4889-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4889-153">JSON Representation</span></span>
<span data-ttu-id="c4889-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4889-154">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
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





