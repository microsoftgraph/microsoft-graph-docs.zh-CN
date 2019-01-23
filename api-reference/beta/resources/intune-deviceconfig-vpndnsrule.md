---
title: vpnDnsRule 资源类型
description: VPN DNS 规则定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425580"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="c6827-103">vpnDnsRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6827-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="c6827-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c6827-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c6827-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6827-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6827-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6827-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6827-107">VPN DNS 规则定义。</span><span class="sxs-lookup"><span data-stu-id="c6827-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c6827-108">属性</span><span class="sxs-lookup"><span data-stu-id="c6827-108">Properties</span></span>
|<span data-ttu-id="c6827-109">属性</span><span class="sxs-lookup"><span data-stu-id="c6827-109">Property</span></span>|<span data-ttu-id="c6827-110">类型</span><span class="sxs-lookup"><span data-stu-id="c6827-110">Type</span></span>|<span data-ttu-id="c6827-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6827-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6827-112">name</span><span class="sxs-lookup"><span data-stu-id="c6827-112">name</span></span>|<span data-ttu-id="c6827-113">String</span><span class="sxs-lookup"><span data-stu-id="c6827-113">String</span></span>|<span data-ttu-id="c6827-114">名称。</span><span class="sxs-lookup"><span data-stu-id="c6827-114">Name.</span></span>|
|<span data-ttu-id="c6827-115">服务器</span><span class="sxs-lookup"><span data-stu-id="c6827-115">servers</span></span>|<span data-ttu-id="c6827-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="c6827-116">String collection</span></span>|<span data-ttu-id="c6827-117">服务器。</span><span class="sxs-lookup"><span data-stu-id="c6827-117">Servers.</span></span>|
|<span data-ttu-id="c6827-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="c6827-118">proxyServerUri</span></span>|<span data-ttu-id="c6827-119">String</span><span class="sxs-lookup"><span data-stu-id="c6827-119">String</span></span>|<span data-ttu-id="c6827-120">代理服务器 Uri。</span><span class="sxs-lookup"><span data-stu-id="c6827-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="c6827-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="c6827-121">autoTrigger</span></span>|<span data-ttu-id="c6827-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6827-122">Boolean</span></span>|<span data-ttu-id="c6827-123">当设备连接到此域时，自动连接到 VPN： 默认值为 False。</span><span class="sxs-lookup"><span data-stu-id="c6827-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="c6827-124">persistent</span><span class="sxs-lookup"><span data-stu-id="c6827-124">persistent</span></span>|<span data-ttu-id="c6827-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6827-125">Boolean</span></span>|<span data-ttu-id="c6827-126">保持此规则处于活动状态，即使没有连接 VPN: False 默认</span><span class="sxs-lookup"><span data-stu-id="c6827-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6827-127">关系</span><span class="sxs-lookup"><span data-stu-id="c6827-127">Relationships</span></span>
<span data-ttu-id="c6827-128">无</span><span class="sxs-lookup"><span data-stu-id="c6827-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6827-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6827-129">JSON Representation</span></span>
<span data-ttu-id="c6827-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6827-130">Here is a JSON representation of the resource.</span></span>
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




