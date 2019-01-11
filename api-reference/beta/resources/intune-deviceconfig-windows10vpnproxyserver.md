---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 231740bbeaa6757456fa684eb71a5b59ebd4adc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872175"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="64b73-103">windows10VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="64b73-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="64b73-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="64b73-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64b73-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="64b73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64b73-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="64b73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64b73-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="64b73-107">VPN Proxy Server.</span></span>

<span data-ttu-id="64b73-108">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="64b73-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64b73-109">属性</span><span class="sxs-lookup"><span data-stu-id="64b73-109">Properties</span></span>
|<span data-ttu-id="64b73-110">属性</span><span class="sxs-lookup"><span data-stu-id="64b73-110">Property</span></span>|<span data-ttu-id="64b73-111">类型</span><span class="sxs-lookup"><span data-stu-id="64b73-111">Type</span></span>|<span data-ttu-id="64b73-112">Description</span><span class="sxs-lookup"><span data-stu-id="64b73-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64b73-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="64b73-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="64b73-114">字符串</span><span class="sxs-lookup"><span data-stu-id="64b73-114">String</span></span>|<span data-ttu-id="64b73-115">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="64b73-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="64b73-116">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="64b73-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="64b73-117">address</span><span class="sxs-lookup"><span data-stu-id="64b73-117">address</span></span>|<span data-ttu-id="64b73-118">String</span><span class="sxs-lookup"><span data-stu-id="64b73-118">String</span></span>|<span data-ttu-id="64b73-119">地址。</span><span class="sxs-lookup"><span data-stu-id="64b73-119">Address.</span></span> <span data-ttu-id="64b73-120">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="64b73-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="64b73-121">port</span><span class="sxs-lookup"><span data-stu-id="64b73-121">port</span></span>|<span data-ttu-id="64b73-122">Int32</span><span class="sxs-lookup"><span data-stu-id="64b73-122">Int32</span></span>|<span data-ttu-id="64b73-123">端口。</span><span class="sxs-lookup"><span data-stu-id="64b73-123">Port.</span></span> <span data-ttu-id="64b73-124">有效值 0 到 65535 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="64b73-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="64b73-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="64b73-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="64b73-126">布尔</span><span class="sxs-lookup"><span data-stu-id="64b73-126">Boolean</span></span>|<span data-ttu-id="64b73-127">对于本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="64b73-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64b73-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="64b73-128">Relationships</span></span>
<span data-ttu-id="64b73-129">无</span><span class="sxs-lookup"><span data-stu-id="64b73-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64b73-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64b73-130">JSON Representation</span></span>
<span data-ttu-id="64b73-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64b73-131">Here is a JSON representation of the resource.</span></span>
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





