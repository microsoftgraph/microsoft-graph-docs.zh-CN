---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56b9177c19ec089a3c93bd388084ae20d7865ace
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944206"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="f23dc-103">windows10VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="f23dc-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="f23dc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f23dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f23dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f23dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23dc-106">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="f23dc-106">VPN Proxy Server.</span></span>


<span data-ttu-id="f23dc-107">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f23dc-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f23dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="f23dc-108">Properties</span></span>
|<span data-ttu-id="f23dc-109">属性</span><span class="sxs-lookup"><span data-stu-id="f23dc-109">Property</span></span>|<span data-ttu-id="f23dc-110">类型</span><span class="sxs-lookup"><span data-stu-id="f23dc-110">Type</span></span>|<span data-ttu-id="f23dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="f23dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23dc-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="f23dc-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="f23dc-113">String</span><span class="sxs-lookup"><span data-stu-id="f23dc-113">String</span></span>|<span data-ttu-id="f23dc-114">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="f23dc-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="f23dc-115">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f23dc-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="f23dc-116">address</span><span class="sxs-lookup"><span data-stu-id="f23dc-116">address</span></span>|<span data-ttu-id="f23dc-117">String</span><span class="sxs-lookup"><span data-stu-id="f23dc-117">String</span></span>|<span data-ttu-id="f23dc-118">处理.</span><span class="sxs-lookup"><span data-stu-id="f23dc-118">Address.</span></span> <span data-ttu-id="f23dc-119">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="f23dc-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="f23dc-120">端口</span><span class="sxs-lookup"><span data-stu-id="f23dc-120">port</span></span>|<span data-ttu-id="f23dc-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f23dc-121">Int32</span></span>|<span data-ttu-id="f23dc-122">端口.</span><span class="sxs-lookup"><span data-stu-id="f23dc-122">Port.</span></span> <span data-ttu-id="f23dc-123">从[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="f23dc-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="f23dc-124">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="f23dc-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="f23dc-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f23dc-125">Boolean</span></span>|<span data-ttu-id="f23dc-126">对本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="f23dc-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f23dc-127">关系</span><span class="sxs-lookup"><span data-stu-id="f23dc-127">Relationships</span></span>
<span data-ttu-id="f23dc-128">无</span><span class="sxs-lookup"><span data-stu-id="f23dc-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f23dc-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f23dc-129">JSON Representation</span></span>
<span data-ttu-id="f23dc-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f23dc-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```




