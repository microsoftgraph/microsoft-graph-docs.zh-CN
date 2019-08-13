---
title: vpnOnDemandRule 资源类型
description: VPN 按需规则定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7b562f9f1be09c5214905e67b2a8ac604e03f20
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367664"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="3a651-103">vpnOnDemandRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a651-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="3a651-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a651-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a651-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a651-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a651-106">VPN 按需规则定义。</span><span class="sxs-lookup"><span data-stu-id="3a651-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3a651-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a651-107">Properties</span></span>
|<span data-ttu-id="3a651-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a651-108">Property</span></span>|<span data-ttu-id="3a651-109">类型</span><span class="sxs-lookup"><span data-stu-id="3a651-109">Type</span></span>|<span data-ttu-id="3a651-110">说明</span><span class="sxs-lookup"><span data-stu-id="3a651-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a651-111">ssid</span><span class="sxs-lookup"><span data-stu-id="3a651-111">ssids</span></span>|<span data-ttu-id="3a651-112">String collection</span><span class="sxs-lookup"><span data-stu-id="3a651-112">String collection</span></span>|<span data-ttu-id="3a651-113">网络服务集标识符 (Ssid)。</span><span class="sxs-lookup"><span data-stu-id="3a651-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="3a651-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="3a651-114">dnsSearchDomains</span></span>|<span data-ttu-id="3a651-115">String collection</span><span class="sxs-lookup"><span data-stu-id="3a651-115">String collection</span></span>|<span data-ttu-id="3a651-116">DNS 搜索域。</span><span class="sxs-lookup"><span data-stu-id="3a651-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="3a651-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="3a651-117">probeUrl</span></span>|<span data-ttu-id="3a651-118">String</span><span class="sxs-lookup"><span data-stu-id="3a651-118">String</span></span>|<span data-ttu-id="3a651-119">要探测的 URL。</span><span class="sxs-lookup"><span data-stu-id="3a651-119">A URL to probe.</span></span> <span data-ttu-id="3a651-120">如果此 URL 已成功获取 (返回 200 HTTP 状态代码) 而不进行重定向, 则此规则匹配。</span><span class="sxs-lookup"><span data-stu-id="3a651-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="3a651-121">action</span><span class="sxs-lookup"><span data-stu-id="3a651-121">action</span></span>|[<span data-ttu-id="3a651-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="3a651-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="3a651-123">退货.</span><span class="sxs-lookup"><span data-stu-id="3a651-123">Action.</span></span> <span data-ttu-id="3a651-124">可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。</span><span class="sxs-lookup"><span data-stu-id="3a651-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="3a651-125">domainAction</span><span class="sxs-lookup"><span data-stu-id="3a651-125">domainAction</span></span>|[<span data-ttu-id="3a651-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="3a651-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="3a651-127">域操作 (仅适用于操作评估连接时)。</span><span class="sxs-lookup"><span data-stu-id="3a651-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="3a651-128">可取值为：`connectIfNeeded`、`neverConnect`。</span><span class="sxs-lookup"><span data-stu-id="3a651-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="3a651-129">域</span><span class="sxs-lookup"><span data-stu-id="3a651-129">domains</span></span>|<span data-ttu-id="3a651-130">String collection</span><span class="sxs-lookup"><span data-stu-id="3a651-130">String collection</span></span>|<span data-ttu-id="3a651-131">域 (仅当操作为 "评估连接时" 时适用)。</span><span class="sxs-lookup"><span data-stu-id="3a651-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="3a651-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="3a651-132">probeRequiredUrl</span></span>|<span data-ttu-id="3a651-133">String</span><span class="sxs-lookup"><span data-stu-id="3a651-133">String</span></span>|<span data-ttu-id="3a651-134">探测器必需 Url (仅在操作评估连接时适用, 如果需要, DomainAction 将进行连接)。</span><span class="sxs-lookup"><span data-stu-id="3a651-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a651-135">关系</span><span class="sxs-lookup"><span data-stu-id="3a651-135">Relationships</span></span>
<span data-ttu-id="3a651-136">无</span><span class="sxs-lookup"><span data-stu-id="3a651-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a651-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a651-137">JSON Representation</span></span>
<span data-ttu-id="3a651-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a651-138">Here is a JSON representation of the resource.</span></span>
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



