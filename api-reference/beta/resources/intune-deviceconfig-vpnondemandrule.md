---
title: vpnOnDemandRule 资源类型
description: VPN 按需规则定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 648214bac549b13605211aa47d5e12201db02bab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299609"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="07d23-103">vpnOnDemandRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="07d23-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="07d23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07d23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07d23-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07d23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07d23-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07d23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d23-107">VPN 按需规则定义。</span><span class="sxs-lookup"><span data-stu-id="07d23-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="07d23-108">属性</span><span class="sxs-lookup"><span data-stu-id="07d23-108">Properties</span></span>
|<span data-ttu-id="07d23-109">属性</span><span class="sxs-lookup"><span data-stu-id="07d23-109">Property</span></span>|<span data-ttu-id="07d23-110">类型</span><span class="sxs-lookup"><span data-stu-id="07d23-110">Type</span></span>|<span data-ttu-id="07d23-111">Description</span><span class="sxs-lookup"><span data-stu-id="07d23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d23-112">ssid</span><span class="sxs-lookup"><span data-stu-id="07d23-112">ssids</span></span>|<span data-ttu-id="07d23-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="07d23-113">String collection</span></span>|<span data-ttu-id="07d23-114">网络服务 (Ssid) 设置标识符。</span><span class="sxs-lookup"><span data-stu-id="07d23-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="07d23-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="07d23-115">dnsSearchDomains</span></span>|<span data-ttu-id="07d23-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="07d23-116">String collection</span></span>|<span data-ttu-id="07d23-117">DNS 搜索域。</span><span class="sxs-lookup"><span data-stu-id="07d23-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="07d23-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="07d23-118">probeUrl</span></span>|<span data-ttu-id="07d23-119">字符串</span><span class="sxs-lookup"><span data-stu-id="07d23-119">String</span></span>|<span data-ttu-id="07d23-120">要探测的 URL。</span><span class="sxs-lookup"><span data-stu-id="07d23-120">A URL to probe.</span></span> <span data-ttu-id="07d23-121">如果此 URL 已成功获取 (返回 200 HTTP 状态代码) 而不进行重定向，则此规则匹配。</span><span class="sxs-lookup"><span data-stu-id="07d23-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="07d23-122">action</span><span class="sxs-lookup"><span data-stu-id="07d23-122">action</span></span>|[<span data-ttu-id="07d23-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="07d23-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="07d23-124">退货.</span><span class="sxs-lookup"><span data-stu-id="07d23-124">Action.</span></span> <span data-ttu-id="07d23-125">可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。</span><span class="sxs-lookup"><span data-stu-id="07d23-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="07d23-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="07d23-126">domainAction</span></span>|[<span data-ttu-id="07d23-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="07d23-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="07d23-128">域操作 (仅当操作评估连接) 时才适用。</span><span class="sxs-lookup"><span data-stu-id="07d23-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="07d23-129">可取值为：`connectIfNeeded`、`neverConnect`。</span><span class="sxs-lookup"><span data-stu-id="07d23-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="07d23-130">域</span><span class="sxs-lookup"><span data-stu-id="07d23-130">domains</span></span>|<span data-ttu-id="07d23-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="07d23-131">String collection</span></span>|<span data-ttu-id="07d23-132">域 (仅当操作评估连接) 时才适用。</span><span class="sxs-lookup"><span data-stu-id="07d23-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="07d23-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="07d23-133">probeRequiredUrl</span></span>|<span data-ttu-id="07d23-134">字符串</span><span class="sxs-lookup"><span data-stu-id="07d23-134">String</span></span>|<span data-ttu-id="07d23-135">探测器必需 Url (仅在操作评估连接时适用，如果需要，DomainAction 将进行连接）) 。</span><span class="sxs-lookup"><span data-stu-id="07d23-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="07d23-136">关系</span><span class="sxs-lookup"><span data-stu-id="07d23-136">Relationships</span></span>
<span data-ttu-id="07d23-137">无</span><span class="sxs-lookup"><span data-stu-id="07d23-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07d23-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07d23-138">JSON Representation</span></span>
<span data-ttu-id="07d23-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07d23-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```




