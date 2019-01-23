---
title: windowsNetworkIsolationPolicy 资源类型
description: Windows 网络隔离策略
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7ab7addffa4ff3f9b84ced60c30fe8707c695b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403754"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="9ee87-103">windowsNetworkIsolationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ee87-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="9ee87-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9ee87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ee87-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ee87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ee87-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ee87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ee87-107">Windows 网络隔离策略</span><span class="sxs-lookup"><span data-stu-id="9ee87-107">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="9ee87-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ee87-108">Properties</span></span>
|<span data-ttu-id="9ee87-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ee87-109">Property</span></span>|<span data-ttu-id="9ee87-110">类型</span><span class="sxs-lookup"><span data-stu-id="9ee87-110">Type</span></span>|<span data-ttu-id="9ee87-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ee87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee87-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="9ee87-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="9ee87-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ee87-113">String collection</span></span>|<span data-ttu-id="9ee87-114">这是构成企业边界的域列表。</span><span class="sxs-lookup"><span data-stu-id="9ee87-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="9ee87-115">将被视为企业数据和保护数据从一个发送到的设备这些域。</span><span class="sxs-lookup"><span data-stu-id="9ee87-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="9ee87-116">这些位置将被视为企业数据到共享的安全目标。</span><span class="sxs-lookup"><span data-stu-id="9ee87-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="9ee87-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="9ee87-117">enterpriseCloudResources</span></span>|<span data-ttu-id="9ee87-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ee87-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="9ee87-119">包含需要保护在云中承载的企业资源域的列表。</span><span class="sxs-lookup"><span data-stu-id="9ee87-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="9ee87-120">与这些资源的连接被视为企业数据。</span><span class="sxs-lookup"><span data-stu-id="9ee87-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="9ee87-121">如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。</span><span class="sxs-lookup"><span data-stu-id="9ee87-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="9ee87-122">此外必须使用 EnterpriseInternalProxyServers 策略配置代理服务器使用实现此目的。</span><span class="sxs-lookup"><span data-stu-id="9ee87-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="9ee87-123">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9ee87-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9ee87-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="9ee87-124">enterpriseIPRanges</span></span>|<span data-ttu-id="9ee87-125">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ee87-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="9ee87-126">设置可定义企业网络中计算机的企业 IP 范围。</span><span class="sxs-lookup"><span data-stu-id="9ee87-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="9ee87-127">来自这些计算机的数据将被视为企业的一部分并受保护。</span><span class="sxs-lookup"><span data-stu-id="9ee87-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="9ee87-128">这些位置将被视为企业数据到共享的安全目标。</span><span class="sxs-lookup"><span data-stu-id="9ee87-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="9ee87-129">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9ee87-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9ee87-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="9ee87-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="9ee87-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ee87-131">String collection</span></span>|<span data-ttu-id="9ee87-132">这是逗号分隔的内部代理服务器列表。</span><span class="sxs-lookup"><span data-stu-id="9ee87-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="9ee87-133">例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。</span><span class="sxs-lookup"><span data-stu-id="9ee87-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="9ee87-134">这些代理已由管理员配置为连接到 Internet 上的特定资源。</span><span class="sxs-lookup"><span data-stu-id="9ee87-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="9ee87-135">它们被视为企业版网络位置。</span><span class="sxs-lookup"><span data-stu-id="9ee87-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="9ee87-136">代理是仅利用中配置 EnterpriseCloudResources 策略以强制转换为通过这些代理的匹配的云资源通信。</span><span class="sxs-lookup"><span data-stu-id="9ee87-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="9ee87-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9ee87-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="9ee87-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ee87-138">Boolean</span></span>|<span data-ttu-id="9ee87-139">用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ee87-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="9ee87-140">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="9ee87-140">Default is false.</span></span>|
|<span data-ttu-id="9ee87-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="9ee87-141">enterpriseProxyServers</span></span>|<span data-ttu-id="9ee87-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ee87-142">String collection</span></span>|<span data-ttu-id="9ee87-143">这是代理服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="9ee87-143">This is a list of proxy servers.</span></span> <span data-ttu-id="9ee87-144">不在此列表的任何服务器被视为非企业。</span><span class="sxs-lookup"><span data-stu-id="9ee87-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="9ee87-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="9ee87-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="9ee87-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ee87-146">Boolean</span></span>|<span data-ttu-id="9ee87-147">用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ee87-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="9ee87-148">默认值为 false</span><span class="sxs-lookup"><span data-stu-id="9ee87-148">Default is false</span></span>|
|<span data-ttu-id="9ee87-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="9ee87-149">neutralDomainResources</span></span>|<span data-ttu-id="9ee87-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ee87-150">String collection</span></span>|<span data-ttu-id="9ee87-151">可用于工作或个人资源的域名的列表。</span><span class="sxs-lookup"><span data-stu-id="9ee87-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ee87-152">关系</span><span class="sxs-lookup"><span data-stu-id="9ee87-152">Relationships</span></span>
<span data-ttu-id="9ee87-153">无</span><span class="sxs-lookup"><span data-stu-id="9ee87-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ee87-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ee87-154">JSON Representation</span></span>
<span data-ttu-id="9ee87-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ee87-155">Here is a JSON representation of the resource.</span></span>
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




