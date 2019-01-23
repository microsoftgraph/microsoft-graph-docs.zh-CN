---
title: windows10VpnProxyServer 资源类型
description: VPN 代理服务器。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407121"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="c2eb2-103">windows10VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2eb2-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="c2eb2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2eb2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2eb2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2eb2-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-107">VPN Proxy Server.</span></span>


<span data-ttu-id="c2eb2-108">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2eb2-109">属性</span><span class="sxs-lookup"><span data-stu-id="c2eb2-109">Properties</span></span>
|<span data-ttu-id="c2eb2-110">属性</span><span class="sxs-lookup"><span data-stu-id="c2eb2-110">Property</span></span>|<span data-ttu-id="c2eb2-111">类型</span><span class="sxs-lookup"><span data-stu-id="c2eb2-111">Type</span></span>|<span data-ttu-id="c2eb2-112">说明</span><span class="sxs-lookup"><span data-stu-id="c2eb2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2eb2-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="c2eb2-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="c2eb2-114">String</span><span class="sxs-lookup"><span data-stu-id="c2eb2-114">String</span></span>|<span data-ttu-id="c2eb2-115">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="c2eb2-116">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c2eb2-117">address</span><span class="sxs-lookup"><span data-stu-id="c2eb2-117">address</span></span>|<span data-ttu-id="c2eb2-118">String</span><span class="sxs-lookup"><span data-stu-id="c2eb2-118">String</span></span>|<span data-ttu-id="c2eb2-119">地址。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-119">Address.</span></span> <span data-ttu-id="c2eb2-120">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c2eb2-121">port</span><span class="sxs-lookup"><span data-stu-id="c2eb2-121">port</span></span>|<span data-ttu-id="c2eb2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c2eb2-122">Int32</span></span>|<span data-ttu-id="c2eb2-123">端口。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-123">Port.</span></span> <span data-ttu-id="c2eb2-124">有效值 0 到 65535 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c2eb2-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c2eb2-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="c2eb2-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="c2eb2-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2eb2-126">Boolean</span></span>|<span data-ttu-id="c2eb2-127">对于本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2eb2-128">关系</span><span class="sxs-lookup"><span data-stu-id="c2eb2-128">Relationships</span></span>
<span data-ttu-id="c2eb2-129">无</span><span class="sxs-lookup"><span data-stu-id="c2eb2-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2eb2-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2eb2-130">JSON Representation</span></span>
<span data-ttu-id="c2eb2-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2eb2-131">Here is a JSON representation of the resource.</span></span>
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




