---
title: vpnOnDemandRule 资源类型
description: VPN 按需规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161584"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="e130e-103">vpnOnDemandRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="e130e-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="e130e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e130e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e130e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e130e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e130e-106">VPN 按需规则定义。</span><span class="sxs-lookup"><span data-stu-id="e130e-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e130e-107">属性</span><span class="sxs-lookup"><span data-stu-id="e130e-107">Properties</span></span>
|<span data-ttu-id="e130e-108">属性</span><span class="sxs-lookup"><span data-stu-id="e130e-108">Property</span></span>|<span data-ttu-id="e130e-109">类型</span><span class="sxs-lookup"><span data-stu-id="e130e-109">Type</span></span>|<span data-ttu-id="e130e-110">说明</span><span class="sxs-lookup"><span data-stu-id="e130e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e130e-111">ssid</span><span class="sxs-lookup"><span data-stu-id="e130e-111">ssids</span></span>|<span data-ttu-id="e130e-112">String collection</span><span class="sxs-lookup"><span data-stu-id="e130e-112">String collection</span></span>|<span data-ttu-id="e130e-113">网络服务集标识符 (ssid)。</span><span class="sxs-lookup"><span data-stu-id="e130e-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="e130e-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="e130e-114">dnsSearchDomains</span></span>|<span data-ttu-id="e130e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="e130e-115">String collection</span></span>|<span data-ttu-id="e130e-116">DNS 搜索域。</span><span class="sxs-lookup"><span data-stu-id="e130e-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="e130e-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="e130e-117">probeUrl</span></span>|<span data-ttu-id="e130e-118">String</span><span class="sxs-lookup"><span data-stu-id="e130e-118">String</span></span>|<span data-ttu-id="e130e-119">要探测的 URL。</span><span class="sxs-lookup"><span data-stu-id="e130e-119">A URL to probe.</span></span> <span data-ttu-id="e130e-120">如果此 URL 已成功获取 (返回 200 HTTP 状态代码) 而不进行重定向, 则此规则匹配。</span><span class="sxs-lookup"><span data-stu-id="e130e-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="e130e-121">action</span><span class="sxs-lookup"><span data-stu-id="e130e-121">action</span></span>|[<span data-ttu-id="e130e-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="e130e-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="e130e-123">退货.</span><span class="sxs-lookup"><span data-stu-id="e130e-123">Action.</span></span> <span data-ttu-id="e130e-124">可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。</span><span class="sxs-lookup"><span data-stu-id="e130e-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="e130e-125">domainAction</span><span class="sxs-lookup"><span data-stu-id="e130e-125">domainAction</span></span>|[<span data-ttu-id="e130e-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="e130e-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="e130e-127">域操作 (仅适用于操作评估连接时)。</span><span class="sxs-lookup"><span data-stu-id="e130e-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="e130e-128">可取值为：`connectIfNeeded`、`neverConnect`。</span><span class="sxs-lookup"><span data-stu-id="e130e-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="e130e-129">域</span><span class="sxs-lookup"><span data-stu-id="e130e-129">domains</span></span>|<span data-ttu-id="e130e-130">String collection</span><span class="sxs-lookup"><span data-stu-id="e130e-130">String collection</span></span>|<span data-ttu-id="e130e-131">域 (仅当操作为 "评估连接时" 时适用)。</span><span class="sxs-lookup"><span data-stu-id="e130e-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="e130e-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="e130e-132">probeRequiredUrl</span></span>|<span data-ttu-id="e130e-133">String</span><span class="sxs-lookup"><span data-stu-id="e130e-133">String</span></span>|<span data-ttu-id="e130e-134">探测器必需 Url (仅在操作评估连接时适用, 如果需要, DomainAction 将进行连接)。</span><span class="sxs-lookup"><span data-stu-id="e130e-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e130e-135">关系</span><span class="sxs-lookup"><span data-stu-id="e130e-135">Relationships</span></span>
<span data-ttu-id="e130e-136">无</span><span class="sxs-lookup"><span data-stu-id="e130e-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e130e-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e130e-137">JSON Representation</span></span>
<span data-ttu-id="e130e-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e130e-138">Here is a JSON representation of the resource.</span></span>
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




