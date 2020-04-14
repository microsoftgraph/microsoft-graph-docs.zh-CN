---
title: vpnOnDemandRule 资源类型
description: VPN 按需规则定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd5724e4c2c1cfb5ca185dd8420011853812305a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412145"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="9b4fb-103">vpnOnDemandRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b4fb-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="9b4fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b4fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b4fb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b4fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b4fb-107">VPN 按需规则定义。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9b4fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b4fb-108">Properties</span></span>
|<span data-ttu-id="9b4fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b4fb-109">Property</span></span>|<span data-ttu-id="9b4fb-110">类型</span><span class="sxs-lookup"><span data-stu-id="9b4fb-110">Type</span></span>|<span data-ttu-id="9b4fb-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b4fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4fb-112">ssid</span><span class="sxs-lookup"><span data-stu-id="9b4fb-112">ssids</span></span>|<span data-ttu-id="9b4fb-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="9b4fb-113">String collection</span></span>|<span data-ttu-id="9b4fb-114">网络服务集标识符（Ssid）。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="9b4fb-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="9b4fb-115">dnsSearchDomains</span></span>|<span data-ttu-id="9b4fb-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="9b4fb-116">String collection</span></span>|<span data-ttu-id="9b4fb-117">DNS 搜索域。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="9b4fb-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="9b4fb-118">probeUrl</span></span>|<span data-ttu-id="9b4fb-119">String</span><span class="sxs-lookup"><span data-stu-id="9b4fb-119">String</span></span>|<span data-ttu-id="9b4fb-120">要探测的 URL。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-120">A URL to probe.</span></span> <span data-ttu-id="9b4fb-121">如果此 URL 已成功获取（返回 200 HTTP 状态代码）而不进行重定向，则此规则匹配。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="9b4fb-122">action</span><span class="sxs-lookup"><span data-stu-id="9b4fb-122">action</span></span>|[<span data-ttu-id="9b4fb-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="9b4fb-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="9b4fb-124">退货.</span><span class="sxs-lookup"><span data-stu-id="9b4fb-124">Action.</span></span> <span data-ttu-id="9b4fb-125">可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="9b4fb-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="9b4fb-126">domainAction</span></span>|[<span data-ttu-id="9b4fb-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="9b4fb-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="9b4fb-128">域操作（仅适用于操作评估连接时）。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="9b4fb-129">可取值为：`connectIfNeeded`、`neverConnect`。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="9b4fb-130">域</span><span class="sxs-lookup"><span data-stu-id="9b4fb-130">domains</span></span>|<span data-ttu-id="9b4fb-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="9b4fb-131">String collection</span></span>|<span data-ttu-id="9b4fb-132">域（仅当操作为 "评估连接时" 时适用）。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="9b4fb-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="9b4fb-133">probeRequiredUrl</span></span>|<span data-ttu-id="9b4fb-134">String</span><span class="sxs-lookup"><span data-stu-id="9b4fb-134">String</span></span>|<span data-ttu-id="9b4fb-135">探测器必需 Url （仅在操作评估连接时适用，如果需要，DomainAction 将进行连接）。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b4fb-136">关系</span><span class="sxs-lookup"><span data-stu-id="9b4fb-136">Relationships</span></span>
<span data-ttu-id="9b4fb-137">无</span><span class="sxs-lookup"><span data-stu-id="9b4fb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b4fb-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b4fb-138">JSON Representation</span></span>
<span data-ttu-id="9b4fb-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b4fb-139">Here is a JSON representation of the resource.</span></span>
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



