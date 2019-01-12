---
title: vpnOnDemandRule 资源类型
description: VPN 点播规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43908a55ff43c533d02ace629a80b96dc09c10ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955413"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="52bee-103">vpnOnDemandRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="52bee-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="52bee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="52bee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52bee-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="52bee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52bee-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="52bee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52bee-107">VPN 点播规则定义。</span><span class="sxs-lookup"><span data-stu-id="52bee-107">VPN On-Demand Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="52bee-108">属性</span><span class="sxs-lookup"><span data-stu-id="52bee-108">Properties</span></span>
|<span data-ttu-id="52bee-109">属性</span><span class="sxs-lookup"><span data-stu-id="52bee-109">Property</span></span>|<span data-ttu-id="52bee-110">类型</span><span class="sxs-lookup"><span data-stu-id="52bee-110">Type</span></span>|<span data-ttu-id="52bee-111">说明</span><span class="sxs-lookup"><span data-stu-id="52bee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52bee-112">ssid</span><span class="sxs-lookup"><span data-stu-id="52bee-112">ssids</span></span>|<span data-ttu-id="52bee-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="52bee-113">String collection</span></span>|<span data-ttu-id="52bee-114">网络服务设置标识符 (Ssid)。</span><span class="sxs-lookup"><span data-stu-id="52bee-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="52bee-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="52bee-115">dnsSearchDomains</span></span>|<span data-ttu-id="52bee-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="52bee-116">String collection</span></span>|<span data-ttu-id="52bee-117">DNS 搜索域。</span><span class="sxs-lookup"><span data-stu-id="52bee-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="52bee-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="52bee-118">probeUrl</span></span>|<span data-ttu-id="52bee-119">字符串</span><span class="sxs-lookup"><span data-stu-id="52bee-119">String</span></span>|<span data-ttu-id="52bee-120">调查 URL。</span><span class="sxs-lookup"><span data-stu-id="52bee-120">A URL to probe.</span></span> <span data-ttu-id="52bee-121">如果此 URL 是成功不使用重定向中提取 （返回 200 HTTP 状态代码），此规则匹配。</span><span class="sxs-lookup"><span data-stu-id="52bee-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="52bee-122">action</span><span class="sxs-lookup"><span data-stu-id="52bee-122">action</span></span>|[<span data-ttu-id="52bee-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="52bee-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="52bee-124">操作。</span><span class="sxs-lookup"><span data-stu-id="52bee-124">Action.</span></span> <span data-ttu-id="52bee-125">可取值为：`connect`、`evaluateConnection`、`ignore`、`disconnect`。</span><span class="sxs-lookup"><span data-stu-id="52bee-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="52bee-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="52bee-126">domainAction</span></span>|[<span data-ttu-id="52bee-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="52bee-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="52bee-128">域操作 （仅当操作是计算连接时才适用）。</span><span class="sxs-lookup"><span data-stu-id="52bee-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="52bee-129">可取值为：`connectIfNeeded`、`neverConnect`。</span><span class="sxs-lookup"><span data-stu-id="52bee-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="52bee-130">域</span><span class="sxs-lookup"><span data-stu-id="52bee-130">domains</span></span>|<span data-ttu-id="52bee-131">String 集合</span><span class="sxs-lookup"><span data-stu-id="52bee-131">String collection</span></span>|<span data-ttu-id="52bee-132">域 （仅当操作是计算连接时才适用）。</span><span class="sxs-lookup"><span data-stu-id="52bee-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="52bee-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="52bee-133">probeRequiredUrl</span></span>|<span data-ttu-id="52bee-134">字符串</span><span class="sxs-lookup"><span data-stu-id="52bee-134">String</span></span>|<span data-ttu-id="52bee-135">探测器所需的 Url （仅操作评估连接并 DomainAction 是连接，必要时才适用）。</span><span class="sxs-lookup"><span data-stu-id="52bee-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="52bee-136">Relationships</span><span class="sxs-lookup"><span data-stu-id="52bee-136">Relationships</span></span>
<span data-ttu-id="52bee-137">无</span><span class="sxs-lookup"><span data-stu-id="52bee-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52bee-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52bee-138">JSON Representation</span></span>
<span data-ttu-id="52bee-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52bee-139">Here is a JSON representation of the resource.</span></span>
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





