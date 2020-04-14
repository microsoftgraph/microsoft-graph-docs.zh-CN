---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac7b87442dc2fda2df5e342981def579457bae3d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412229"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="49cbe-103">vpnDnsRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="49cbe-103">vpnDnsRule resource type</span></span>

<span data-ttu-id="49cbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49cbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49cbe-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49cbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49cbe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49cbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49cbe-107">VPN DNS 规则定义。</span><span class="sxs-lookup"><span data-stu-id="49cbe-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="49cbe-108">属性</span><span class="sxs-lookup"><span data-stu-id="49cbe-108">Properties</span></span>
|<span data-ttu-id="49cbe-109">属性</span><span class="sxs-lookup"><span data-stu-id="49cbe-109">Property</span></span>|<span data-ttu-id="49cbe-110">类型</span><span class="sxs-lookup"><span data-stu-id="49cbe-110">Type</span></span>|<span data-ttu-id="49cbe-111">说明</span><span class="sxs-lookup"><span data-stu-id="49cbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cbe-112">name</span><span class="sxs-lookup"><span data-stu-id="49cbe-112">name</span></span>|<span data-ttu-id="49cbe-113">String</span><span class="sxs-lookup"><span data-stu-id="49cbe-113">String</span></span>|<span data-ttu-id="49cbe-114">别名.</span><span class="sxs-lookup"><span data-stu-id="49cbe-114">Name.</span></span>|
|<span data-ttu-id="49cbe-115">台</span><span class="sxs-lookup"><span data-stu-id="49cbe-115">servers</span></span>|<span data-ttu-id="49cbe-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="49cbe-116">String collection</span></span>|<span data-ttu-id="49cbe-117">台.</span><span class="sxs-lookup"><span data-stu-id="49cbe-117">Servers.</span></span>|
|<span data-ttu-id="49cbe-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="49cbe-118">proxyServerUri</span></span>|<span data-ttu-id="49cbe-119">String</span><span class="sxs-lookup"><span data-stu-id="49cbe-119">String</span></span>|<span data-ttu-id="49cbe-120">代理服务器 Uri。</span><span class="sxs-lookup"><span data-stu-id="49cbe-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="49cbe-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="49cbe-121">autoTrigger</span></span>|<span data-ttu-id="49cbe-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="49cbe-122">Boolean</span></span>|<span data-ttu-id="49cbe-123">当设备连接到此域时自动连接到 VPN：默认值为 False。</span><span class="sxs-lookup"><span data-stu-id="49cbe-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="49cbe-124">保持</span><span class="sxs-lookup"><span data-stu-id="49cbe-124">persistent</span></span>|<span data-ttu-id="49cbe-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="49cbe-125">Boolean</span></span>|<span data-ttu-id="49cbe-126">将此规则保持为活动状态，即使未连接 VPN 也是如此：默认值为 False</span><span class="sxs-lookup"><span data-stu-id="49cbe-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="49cbe-127">关系</span><span class="sxs-lookup"><span data-stu-id="49cbe-127">Relationships</span></span>
<span data-ttu-id="49cbe-128">无</span><span class="sxs-lookup"><span data-stu-id="49cbe-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49cbe-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49cbe-129">JSON Representation</span></span>
<span data-ttu-id="49cbe-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49cbe-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```



