---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 212bafa99a51e269716978cafa4fcf274dd76579
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572022"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="efb2a-103">windows10VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="efb2a-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="efb2a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efb2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efb2a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efb2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb2a-106">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="efb2a-106">VPN Proxy Server.</span></span>


<span data-ttu-id="efb2a-107">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="efb2a-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efb2a-108">属性</span><span class="sxs-lookup"><span data-stu-id="efb2a-108">Properties</span></span>
|<span data-ttu-id="efb2a-109">属性</span><span class="sxs-lookup"><span data-stu-id="efb2a-109">Property</span></span>|<span data-ttu-id="efb2a-110">类型</span><span class="sxs-lookup"><span data-stu-id="efb2a-110">Type</span></span>|<span data-ttu-id="efb2a-111">说明</span><span class="sxs-lookup"><span data-stu-id="efb2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb2a-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="efb2a-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="efb2a-113">String</span><span class="sxs-lookup"><span data-stu-id="efb2a-113">String</span></span>|<span data-ttu-id="efb2a-114">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="efb2a-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="efb2a-115">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="efb2a-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="efb2a-116">address</span><span class="sxs-lookup"><span data-stu-id="efb2a-116">address</span></span>|<span data-ttu-id="efb2a-117">String</span><span class="sxs-lookup"><span data-stu-id="efb2a-117">String</span></span>|<span data-ttu-id="efb2a-118">处理.</span><span class="sxs-lookup"><span data-stu-id="efb2a-118">Address.</span></span> <span data-ttu-id="efb2a-119">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="efb2a-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="efb2a-120">端口</span><span class="sxs-lookup"><span data-stu-id="efb2a-120">port</span></span>|<span data-ttu-id="efb2a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="efb2a-121">Int32</span></span>|<span data-ttu-id="efb2a-122">端口.</span><span class="sxs-lookup"><span data-stu-id="efb2a-122">Port.</span></span> <span data-ttu-id="efb2a-123">从[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="efb2a-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="efb2a-124">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="efb2a-124">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="efb2a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="efb2a-125">Boolean</span></span>|<span data-ttu-id="efb2a-126">对本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="efb2a-126">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efb2a-127">关系</span><span class="sxs-lookup"><span data-stu-id="efb2a-127">Relationships</span></span>
<span data-ttu-id="efb2a-128">无</span><span class="sxs-lookup"><span data-stu-id="efb2a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efb2a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efb2a-129">JSON Representation</span></span>
<span data-ttu-id="efb2a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efb2a-130">Here is a JSON representation of the resource.</span></span>
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





