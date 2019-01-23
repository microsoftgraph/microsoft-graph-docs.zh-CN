---
title: vpnOnDemandRule 资源类型
description: VPN 点播规则定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421457"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="2d0f7-103">vpnOnDemandRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d0f7-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="2d0f7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2d0f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d0f7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d0f7-107">VPN 点播规则定义。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2d0f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d0f7-108">Properties</span></span>
|<span data-ttu-id="2d0f7-109">属性</span><span class="sxs-lookup"><span data-stu-id="2d0f7-109">Property</span></span>|<span data-ttu-id="2d0f7-110">类型</span><span class="sxs-lookup"><span data-stu-id="2d0f7-110">Type</span></span>|<span data-ttu-id="2d0f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="2d0f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d0f7-112">ssid</span><span class="sxs-lookup"><span data-stu-id="2d0f7-112">ssids</span></span>|<span data-ttu-id="2d0f7-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="2d0f7-113">String collection</span></span>|<span data-ttu-id="2d0f7-114">网络服务设置标识符 (Ssid)。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="2d0f7-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="2d0f7-115">dnsSearchDomains</span></span>|<span data-ttu-id="2d0f7-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="2d0f7-116">String collection</span></span>|<span data-ttu-id="2d0f7-117">DNS 搜索域。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="2d0f7-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="2d0f7-118">probeUrl</span></span>|<span data-ttu-id="2d0f7-119">String</span><span class="sxs-lookup"><span data-stu-id="2d0f7-119">String</span></span>|<span data-ttu-id="2d0f7-120">调查 URL。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-120">A URL to probe.</span></span> <span data-ttu-id="2d0f7-121">如果此 URL 是成功不使用重定向中提取 （返回 200 HTTP 状态代码），此规则匹配。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="2d0f7-122">action</span><span class="sxs-lookup"><span data-stu-id="2d0f7-122">action</span></span>|[<span data-ttu-id="2d0f7-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="2d0f7-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="2d0f7-124">操作。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-124">Action.</span></span> <span data-ttu-id="2d0f7-125">可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="2d0f7-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="2d0f7-126">domainAction</span></span>|[<span data-ttu-id="2d0f7-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="2d0f7-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="2d0f7-128">域操作 （仅当操作是计算连接时才适用）。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="2d0f7-129">可取值为：`connectIfNeeded`、`neverConnect`。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="2d0f7-130">域</span><span class="sxs-lookup"><span data-stu-id="2d0f7-130">domains</span></span>|<span data-ttu-id="2d0f7-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="2d0f7-131">String collection</span></span>|<span data-ttu-id="2d0f7-132">域 （仅当操作是计算连接时才适用）。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="2d0f7-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="2d0f7-133">probeRequiredUrl</span></span>|<span data-ttu-id="2d0f7-134">String</span><span class="sxs-lookup"><span data-stu-id="2d0f7-134">String</span></span>|<span data-ttu-id="2d0f7-135">探测器所需的 Url （仅操作评估连接并 DomainAction 是连接，必要时才适用）。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d0f7-136">关系</span><span class="sxs-lookup"><span data-stu-id="2d0f7-136">Relationships</span></span>
<span data-ttu-id="2d0f7-137">无</span><span class="sxs-lookup"><span data-stu-id="2d0f7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d0f7-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d0f7-138">JSON Representation</span></span>
<span data-ttu-id="2d0f7-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d0f7-139">Here is a JSON representation of the resource.</span></span>
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




