---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb4f94ee9cb1eabb76c5e0aead33ae323b05a8b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734257"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="5e13f-103">windows81VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e13f-103">windows81VpnProxyServer resource type</span></span>

<span data-ttu-id="5e13f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e13f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e13f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e13f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e13f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e13f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e13f-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="5e13f-107">VPN Proxy Server.</span></span>


<span data-ttu-id="5e13f-108">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5e13f-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e13f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e13f-109">Properties</span></span>
|<span data-ttu-id="5e13f-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e13f-110">Property</span></span>|<span data-ttu-id="5e13f-111">类型</span><span class="sxs-lookup"><span data-stu-id="5e13f-111">Type</span></span>|<span data-ttu-id="5e13f-112">说明</span><span class="sxs-lookup"><span data-stu-id="5e13f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e13f-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="5e13f-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="5e13f-114">String</span><span class="sxs-lookup"><span data-stu-id="5e13f-114">String</span></span>|<span data-ttu-id="5e13f-115">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="5e13f-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="5e13f-116">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5e13f-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="5e13f-117">address</span><span class="sxs-lookup"><span data-stu-id="5e13f-117">address</span></span>|<span data-ttu-id="5e13f-118">String</span><span class="sxs-lookup"><span data-stu-id="5e13f-118">String</span></span>|<span data-ttu-id="5e13f-119">处理.</span><span class="sxs-lookup"><span data-stu-id="5e13f-119">Address.</span></span> <span data-ttu-id="5e13f-120">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="5e13f-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="5e13f-121">端口</span><span class="sxs-lookup"><span data-stu-id="5e13f-121">port</span></span>|<span data-ttu-id="5e13f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5e13f-122">Int32</span></span>|<span data-ttu-id="5e13f-123">端口.</span><span class="sxs-lookup"><span data-stu-id="5e13f-123">Port.</span></span> <span data-ttu-id="5e13f-124">从[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="5e13f-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="5e13f-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="5e13f-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="5e13f-126">布尔</span><span class="sxs-lookup"><span data-stu-id="5e13f-126">Boolean</span></span>|<span data-ttu-id="5e13f-127">自动检测代理设置。</span><span class="sxs-lookup"><span data-stu-id="5e13f-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="5e13f-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="5e13f-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="5e13f-129">布尔</span><span class="sxs-lookup"><span data-stu-id="5e13f-129">Boolean</span></span>|<span data-ttu-id="5e13f-130">对本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="5e13f-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e13f-131">关系</span><span class="sxs-lookup"><span data-stu-id="5e13f-131">Relationships</span></span>
<span data-ttu-id="5e13f-132">无</span><span class="sxs-lookup"><span data-stu-id="5e13f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e13f-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e13f-133">JSON Representation</span></span>
<span data-ttu-id="5e13f-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e13f-134">Here is a JSON representation of the resource.</span></span>
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





