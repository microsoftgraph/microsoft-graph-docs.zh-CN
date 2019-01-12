---
title: windows81VpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d276ee7ac84bfe86c197025c05bf1a119b85e06c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917958"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="be7aa-103">windows81VpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="be7aa-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="be7aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="be7aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be7aa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be7aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be7aa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="be7aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be7aa-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="be7aa-107">VPN Proxy Server.</span></span>

<span data-ttu-id="be7aa-108">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="be7aa-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="be7aa-109">属性</span><span class="sxs-lookup"><span data-stu-id="be7aa-109">Properties</span></span>
|<span data-ttu-id="be7aa-110">属性</span><span class="sxs-lookup"><span data-stu-id="be7aa-110">Property</span></span>|<span data-ttu-id="be7aa-111">类型</span><span class="sxs-lookup"><span data-stu-id="be7aa-111">Type</span></span>|<span data-ttu-id="be7aa-112">说明</span><span class="sxs-lookup"><span data-stu-id="be7aa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be7aa-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="be7aa-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="be7aa-114">字符串</span><span class="sxs-lookup"><span data-stu-id="be7aa-114">String</span></span>|<span data-ttu-id="be7aa-115">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="be7aa-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="be7aa-116">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="be7aa-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="be7aa-117">address</span><span class="sxs-lookup"><span data-stu-id="be7aa-117">address</span></span>|<span data-ttu-id="be7aa-118">String</span><span class="sxs-lookup"><span data-stu-id="be7aa-118">String</span></span>|<span data-ttu-id="be7aa-119">地址。</span><span class="sxs-lookup"><span data-stu-id="be7aa-119">Address.</span></span> <span data-ttu-id="be7aa-120">继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="be7aa-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="be7aa-121">port</span><span class="sxs-lookup"><span data-stu-id="be7aa-121">port</span></span>|<span data-ttu-id="be7aa-122">Int32</span><span class="sxs-lookup"><span data-stu-id="be7aa-122">Int32</span></span>|<span data-ttu-id="be7aa-123">端口。</span><span class="sxs-lookup"><span data-stu-id="be7aa-123">Port.</span></span> <span data-ttu-id="be7aa-124">有效值 0 到 65535 继承自[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="be7aa-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="be7aa-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="be7aa-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="be7aa-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="be7aa-126">Boolean</span></span>|<span data-ttu-id="be7aa-127">自动检测代理设置。</span><span class="sxs-lookup"><span data-stu-id="be7aa-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="be7aa-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="be7aa-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="be7aa-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="be7aa-129">Boolean</span></span>|<span data-ttu-id="be7aa-130">对于本地地址绕过代理服务器。</span><span class="sxs-lookup"><span data-stu-id="be7aa-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be7aa-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="be7aa-131">Relationships</span></span>
<span data-ttu-id="be7aa-132">无</span><span class="sxs-lookup"><span data-stu-id="be7aa-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be7aa-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be7aa-133">JSON Representation</span></span>
<span data-ttu-id="be7aa-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be7aa-134">Here is a JSON representation of the resource.</span></span>
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





