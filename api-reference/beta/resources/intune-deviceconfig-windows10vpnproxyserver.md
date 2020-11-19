---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 684fe0ec823ca43d2a7784555678beddb43dbff1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279393"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="eaaa6-103">windows10VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="eaaa6-103">windows10VpnProxyServer resource type</span></span>

<span data-ttu-id="eaaa6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaaa6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaaa6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eaaa6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaaa6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eaaa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaaa6-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="eaaa6-107">VPN Proxy Server.</span></span>


<span data-ttu-id="eaaa6-108">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa6-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eaaa6-109">属性</span><span class="sxs-lookup"><span data-stu-id="eaaa6-109">Properties</span></span>
|<span data-ttu-id="eaaa6-110">属性</span><span class="sxs-lookup"><span data-stu-id="eaaa6-110">Property</span></span>|<span data-ttu-id="eaaa6-111">类型</span><span class="sxs-lookup"><span data-stu-id="eaaa6-111">Type</span></span>|<span data-ttu-id="eaaa6-112">说明</span><span class="sxs-lookup"><span data-stu-id="eaaa6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaaa6-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="eaaa6-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="eaaa6-114">字符串</span><span class="sxs-lookup"><span data-stu-id="eaaa6-114">String</span></span>|<span data-ttu-id="eaaa6-115">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="eaaa6-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="eaaa6-116">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa6-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="eaaa6-117">address</span><span class="sxs-lookup"><span data-stu-id="eaaa6-117">address</span></span>|<span data-ttu-id="eaaa6-118">String</span><span class="sxs-lookup"><span data-stu-id="eaaa6-118">String</span></span>|<span data-ttu-id="eaaa6-119">处理.</span><span class="sxs-lookup"><span data-stu-id="eaaa6-119">Address.</span></span> <span data-ttu-id="eaaa6-120">继承自 [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="eaaa6-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="eaaa6-121">端口</span><span class="sxs-lookup"><span data-stu-id="eaaa6-121">port</span></span>|<span data-ttu-id="eaaa6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="eaaa6-122">Int32</span></span>|<span data-ttu-id="eaaa6-123">端口.</span><span class="sxs-lookup"><span data-stu-id="eaaa6-123">Port.</span></span> <span data-ttu-id="eaaa6-124">从[VpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)继承的有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="eaaa6-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="eaaa6-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="eaaa6-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="eaaa6-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaaa6-126">Boolean</span></span>|<span data-ttu-id="eaaa6-127">对本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="eaaa6-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaaa6-128">关系</span><span class="sxs-lookup"><span data-stu-id="eaaa6-128">Relationships</span></span>
<span data-ttu-id="eaaa6-129">无</span><span class="sxs-lookup"><span data-stu-id="eaaa6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eaaa6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eaaa6-130">JSON Representation</span></span>
<span data-ttu-id="eaaa6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaaa6-131">Here is a JSON representation of the resource.</span></span>
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




