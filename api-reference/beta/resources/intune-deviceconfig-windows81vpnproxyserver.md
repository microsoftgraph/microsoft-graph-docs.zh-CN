---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 345856eb5032026cd92c33cad07a620e3659f473
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786563"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="03e6f-103">windows81VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="03e6f-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="03e6f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03e6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03e6f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03e6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e6f-106">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="03e6f-106">VPN Proxy Server.</span></span>


<span data-ttu-id="03e6f-107">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="03e6f-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03e6f-108">属性</span><span class="sxs-lookup"><span data-stu-id="03e6f-108">Properties</span></span>
|<span data-ttu-id="03e6f-109">属性</span><span class="sxs-lookup"><span data-stu-id="03e6f-109">Property</span></span>|<span data-ttu-id="03e6f-110">类型</span><span class="sxs-lookup"><span data-stu-id="03e6f-110">Type</span></span>|<span data-ttu-id="03e6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="03e6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e6f-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="03e6f-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="03e6f-113">String</span><span class="sxs-lookup"><span data-stu-id="03e6f-113">String</span></span>|<span data-ttu-id="03e6f-114">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="03e6f-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="03e6f-115">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="03e6f-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="03e6f-116">address</span><span class="sxs-lookup"><span data-stu-id="03e6f-116">address</span></span>|<span data-ttu-id="03e6f-117">String</span><span class="sxs-lookup"><span data-stu-id="03e6f-117">String</span></span>|<span data-ttu-id="03e6f-118">处理.</span><span class="sxs-lookup"><span data-stu-id="03e6f-118">Address.</span></span> <span data-ttu-id="03e6f-119">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="03e6f-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="03e6f-120">端口</span><span class="sxs-lookup"><span data-stu-id="03e6f-120">port</span></span>|<span data-ttu-id="03e6f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="03e6f-121">Int32</span></span>|<span data-ttu-id="03e6f-122">端口.</span><span class="sxs-lookup"><span data-stu-id="03e6f-122">Port.</span></span> <span data-ttu-id="03e6f-123">从[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="03e6f-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="03e6f-124">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="03e6f-124">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="03e6f-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="03e6f-125">Boolean</span></span>|<span data-ttu-id="03e6f-126">自动检测代理设置。</span><span class="sxs-lookup"><span data-stu-id="03e6f-126">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="03e6f-127">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="03e6f-127">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="03e6f-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="03e6f-128">Boolean</span></span>|<span data-ttu-id="03e6f-129">对本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="03e6f-129">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03e6f-130">关系</span><span class="sxs-lookup"><span data-stu-id="03e6f-130">Relationships</span></span>
<span data-ttu-id="03e6f-131">无</span><span class="sxs-lookup"><span data-stu-id="03e6f-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03e6f-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03e6f-132">JSON Representation</span></span>
<span data-ttu-id="03e6f-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03e6f-133">Here is a JSON representation of the resource.</span></span>
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



