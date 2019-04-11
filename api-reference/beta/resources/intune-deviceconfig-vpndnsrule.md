---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db3be739e6ee1e7c5ebe2a5bd33af648488df54f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805850"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="f0940-103">vpnDnsRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0940-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="f0940-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0940-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0940-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0940-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0940-106">VPN DNS 规则定义。</span><span class="sxs-lookup"><span data-stu-id="f0940-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f0940-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0940-107">Properties</span></span>
|<span data-ttu-id="f0940-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0940-108">Property</span></span>|<span data-ttu-id="f0940-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0940-109">Type</span></span>|<span data-ttu-id="f0940-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0940-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0940-111">name</span><span class="sxs-lookup"><span data-stu-id="f0940-111">name</span></span>|<span data-ttu-id="f0940-112">String</span><span class="sxs-lookup"><span data-stu-id="f0940-112">String</span></span>|<span data-ttu-id="f0940-113">别名.</span><span class="sxs-lookup"><span data-stu-id="f0940-113">Name.</span></span>|
|<span data-ttu-id="f0940-114">台</span><span class="sxs-lookup"><span data-stu-id="f0940-114">servers</span></span>|<span data-ttu-id="f0940-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="f0940-115">String collection</span></span>|<span data-ttu-id="f0940-116">台.</span><span class="sxs-lookup"><span data-stu-id="f0940-116">Servers.</span></span>|
|<span data-ttu-id="f0940-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="f0940-117">proxyServerUri</span></span>|<span data-ttu-id="f0940-118">String</span><span class="sxs-lookup"><span data-stu-id="f0940-118">String</span></span>|<span data-ttu-id="f0940-119">代理服务器 Uri。</span><span class="sxs-lookup"><span data-stu-id="f0940-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="f0940-120">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="f0940-120">autoTrigger</span></span>|<span data-ttu-id="f0940-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="f0940-121">Boolean</span></span>|<span data-ttu-id="f0940-122">当设备连接到此域时自动连接到 VPN: 默认值为 False。</span><span class="sxs-lookup"><span data-stu-id="f0940-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="f0940-123">保持</span><span class="sxs-lookup"><span data-stu-id="f0940-123">persistent</span></span>|<span data-ttu-id="f0940-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="f0940-124">Boolean</span></span>|<span data-ttu-id="f0940-125">将此规则保持为活动状态, 即使未连接 VPN 也是如此: 默认值为 False</span><span class="sxs-lookup"><span data-stu-id="f0940-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0940-126">关系</span><span class="sxs-lookup"><span data-stu-id="f0940-126">Relationships</span></span>
<span data-ttu-id="f0940-127">无</span><span class="sxs-lookup"><span data-stu-id="f0940-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0940-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0940-128">JSON Representation</span></span>
<span data-ttu-id="f0940-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0940-129">Here is a JSON representation of the resource.</span></span>
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





