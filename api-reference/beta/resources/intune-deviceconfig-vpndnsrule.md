---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bd40af2d8aa9a2ecb036f60e86d4056727b03a2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299707"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="56a3f-103">vpnDnsRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="56a3f-103">vpnDnsRule resource type</span></span>

<span data-ttu-id="56a3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56a3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56a3f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56a3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56a3f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56a3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a3f-107">VPN DNS 规则定义。</span><span class="sxs-lookup"><span data-stu-id="56a3f-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="56a3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="56a3f-108">Properties</span></span>
|<span data-ttu-id="56a3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="56a3f-109">Property</span></span>|<span data-ttu-id="56a3f-110">类型</span><span class="sxs-lookup"><span data-stu-id="56a3f-110">Type</span></span>|<span data-ttu-id="56a3f-111">Description</span><span class="sxs-lookup"><span data-stu-id="56a3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a3f-112">name</span><span class="sxs-lookup"><span data-stu-id="56a3f-112">name</span></span>|<span data-ttu-id="56a3f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="56a3f-113">String</span></span>|<span data-ttu-id="56a3f-114">别名.</span><span class="sxs-lookup"><span data-stu-id="56a3f-114">Name.</span></span>|
|<span data-ttu-id="56a3f-115">台</span><span class="sxs-lookup"><span data-stu-id="56a3f-115">servers</span></span>|<span data-ttu-id="56a3f-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="56a3f-116">String collection</span></span>|<span data-ttu-id="56a3f-117">台.</span><span class="sxs-lookup"><span data-stu-id="56a3f-117">Servers.</span></span>|
|<span data-ttu-id="56a3f-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="56a3f-118">proxyServerUri</span></span>|<span data-ttu-id="56a3f-119">字符串</span><span class="sxs-lookup"><span data-stu-id="56a3f-119">String</span></span>|<span data-ttu-id="56a3f-120">代理服务器 Uri。</span><span class="sxs-lookup"><span data-stu-id="56a3f-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="56a3f-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="56a3f-121">autoTrigger</span></span>|<span data-ttu-id="56a3f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a3f-122">Boolean</span></span>|<span data-ttu-id="56a3f-123">当设备连接到此域时自动连接到 VPN：默认值为 False。</span><span class="sxs-lookup"><span data-stu-id="56a3f-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="56a3f-124">保持</span><span class="sxs-lookup"><span data-stu-id="56a3f-124">persistent</span></span>|<span data-ttu-id="56a3f-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a3f-125">Boolean</span></span>|<span data-ttu-id="56a3f-126">将此规则保持为活动状态，即使未连接 VPN 也是如此：默认值为 False</span><span class="sxs-lookup"><span data-stu-id="56a3f-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="56a3f-127">关系</span><span class="sxs-lookup"><span data-stu-id="56a3f-127">Relationships</span></span>
<span data-ttu-id="56a3f-128">无</span><span class="sxs-lookup"><span data-stu-id="56a3f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56a3f-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56a3f-129">JSON Representation</span></span>
<span data-ttu-id="56a3f-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56a3f-130">Here is a JSON representation of the resource.</span></span>
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




