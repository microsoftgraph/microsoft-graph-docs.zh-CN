---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0226b443922b3adb03a186397f2a569e9dccbad0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084560"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="3e2de-103">windows81VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e2de-103">windows81VpnProxyServer resource type</span></span>

<span data-ttu-id="3e2de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e2de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e2de-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e2de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e2de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e2de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e2de-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="3e2de-107">VPN Proxy Server.</span></span>


<span data-ttu-id="3e2de-108">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="3e2de-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e2de-109">属性</span><span class="sxs-lookup"><span data-stu-id="3e2de-109">Properties</span></span>
|<span data-ttu-id="3e2de-110">属性</span><span class="sxs-lookup"><span data-stu-id="3e2de-110">Property</span></span>|<span data-ttu-id="3e2de-111">类型</span><span class="sxs-lookup"><span data-stu-id="3e2de-111">Type</span></span>|<span data-ttu-id="3e2de-112">说明</span><span class="sxs-lookup"><span data-stu-id="3e2de-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e2de-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="3e2de-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="3e2de-114">字符串</span><span class="sxs-lookup"><span data-stu-id="3e2de-114">String</span></span>|<span data-ttu-id="3e2de-115">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="3e2de-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="3e2de-116">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="3e2de-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3e2de-117">address</span><span class="sxs-lookup"><span data-stu-id="3e2de-117">address</span></span>|<span data-ttu-id="3e2de-118">String</span><span class="sxs-lookup"><span data-stu-id="3e2de-118">String</span></span>|<span data-ttu-id="3e2de-119">处理.</span><span class="sxs-lookup"><span data-stu-id="3e2de-119">Address.</span></span> <span data-ttu-id="3e2de-120">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="3e2de-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3e2de-121">端口</span><span class="sxs-lookup"><span data-stu-id="3e2de-121">port</span></span>|<span data-ttu-id="3e2de-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3e2de-122">Int32</span></span>|<span data-ttu-id="3e2de-123">端口.</span><span class="sxs-lookup"><span data-stu-id="3e2de-123">Port.</span></span> <span data-ttu-id="3e2de-124">从[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="3e2de-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3e2de-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="3e2de-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="3e2de-126">布尔</span><span class="sxs-lookup"><span data-stu-id="3e2de-126">Boolean</span></span>|<span data-ttu-id="3e2de-127">自动检测代理设置。</span><span class="sxs-lookup"><span data-stu-id="3e2de-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="3e2de-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="3e2de-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="3e2de-129">布尔</span><span class="sxs-lookup"><span data-stu-id="3e2de-129">Boolean</span></span>|<span data-ttu-id="3e2de-130">对本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="3e2de-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e2de-131">关系</span><span class="sxs-lookup"><span data-stu-id="3e2de-131">Relationships</span></span>
<span data-ttu-id="3e2de-132">无</span><span class="sxs-lookup"><span data-stu-id="3e2de-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e2de-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e2de-133">JSON Representation</span></span>
<span data-ttu-id="3e2de-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e2de-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```






