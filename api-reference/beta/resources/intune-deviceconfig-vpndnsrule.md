---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 983b30b1f724c3c8f76e967179c6fcdb1ff1fecb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367727"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="8a6cd-103">vpnDnsRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a6cd-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="8a6cd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a6cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a6cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a6cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a6cd-106">VPN DNS 规则定义。</span><span class="sxs-lookup"><span data-stu-id="8a6cd-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8a6cd-107">属性</span><span class="sxs-lookup"><span data-stu-id="8a6cd-107">Properties</span></span>
|<span data-ttu-id="8a6cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a6cd-108">Property</span></span>|<span data-ttu-id="8a6cd-109">类型</span><span class="sxs-lookup"><span data-stu-id="8a6cd-109">Type</span></span>|<span data-ttu-id="8a6cd-110">说明</span><span class="sxs-lookup"><span data-stu-id="8a6cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6cd-111">name</span><span class="sxs-lookup"><span data-stu-id="8a6cd-111">name</span></span>|<span data-ttu-id="8a6cd-112">String</span><span class="sxs-lookup"><span data-stu-id="8a6cd-112">String</span></span>|<span data-ttu-id="8a6cd-113">别名.</span><span class="sxs-lookup"><span data-stu-id="8a6cd-113">Name.</span></span>|
|<span data-ttu-id="8a6cd-114">台</span><span class="sxs-lookup"><span data-stu-id="8a6cd-114">servers</span></span>|<span data-ttu-id="8a6cd-115">String collection</span><span class="sxs-lookup"><span data-stu-id="8a6cd-115">String collection</span></span>|<span data-ttu-id="8a6cd-116">台.</span><span class="sxs-lookup"><span data-stu-id="8a6cd-116">Servers.</span></span>|
|<span data-ttu-id="8a6cd-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="8a6cd-117">proxyServerUri</span></span>|<span data-ttu-id="8a6cd-118">String</span><span class="sxs-lookup"><span data-stu-id="8a6cd-118">String</span></span>|<span data-ttu-id="8a6cd-119">代理服务器 Uri。</span><span class="sxs-lookup"><span data-stu-id="8a6cd-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="8a6cd-120">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="8a6cd-120">autoTrigger</span></span>|<span data-ttu-id="8a6cd-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a6cd-121">Boolean</span></span>|<span data-ttu-id="8a6cd-122">当设备连接到此域时自动连接到 VPN: 默认值为 False。</span><span class="sxs-lookup"><span data-stu-id="8a6cd-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="8a6cd-123">保持</span><span class="sxs-lookup"><span data-stu-id="8a6cd-123">persistent</span></span>|<span data-ttu-id="8a6cd-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a6cd-124">Boolean</span></span>|<span data-ttu-id="8a6cd-125">将此规则保持为活动状态, 即使未连接 VPN 也是如此: 默认值为 False</span><span class="sxs-lookup"><span data-stu-id="8a6cd-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a6cd-126">关系</span><span class="sxs-lookup"><span data-stu-id="8a6cd-126">Relationships</span></span>
<span data-ttu-id="8a6cd-127">无</span><span class="sxs-lookup"><span data-stu-id="8a6cd-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a6cd-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a6cd-128">JSON Representation</span></span>
<span data-ttu-id="8a6cd-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a6cd-129">Here is a JSON representation of the resource.</span></span>
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



