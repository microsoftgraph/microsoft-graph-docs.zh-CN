---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c711f02dc0b4f7e44ff1bd54669ed9befb73e42a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807642"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="58a13-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="58a13-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="58a13-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58a13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a13-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58a13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a13-106">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="58a13-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="58a13-107">属性</span><span class="sxs-lookup"><span data-stu-id="58a13-107">Properties</span></span>
|<span data-ttu-id="58a13-108">属性</span><span class="sxs-lookup"><span data-stu-id="58a13-108">Property</span></span>|<span data-ttu-id="58a13-109">类型</span><span class="sxs-lookup"><span data-stu-id="58a13-109">Type</span></span>|<span data-ttu-id="58a13-110">说明</span><span class="sxs-lookup"><span data-stu-id="58a13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a13-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="58a13-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="58a13-112">String</span><span class="sxs-lookup"><span data-stu-id="58a13-112">String</span></span>|<span data-ttu-id="58a13-113">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="58a13-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="58a13-114">address</span><span class="sxs-lookup"><span data-stu-id="58a13-114">address</span></span>|<span data-ttu-id="58a13-115">String</span><span class="sxs-lookup"><span data-stu-id="58a13-115">String</span></span>|<span data-ttu-id="58a13-116">处理.</span><span class="sxs-lookup"><span data-stu-id="58a13-116">Address.</span></span>|
|<span data-ttu-id="58a13-117">端口</span><span class="sxs-lookup"><span data-stu-id="58a13-117">port</span></span>|<span data-ttu-id="58a13-118">Int32</span><span class="sxs-lookup"><span data-stu-id="58a13-118">Int32</span></span>|<span data-ttu-id="58a13-119">端口.</span><span class="sxs-lookup"><span data-stu-id="58a13-119">Port.</span></span> <span data-ttu-id="58a13-120">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="58a13-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="58a13-121">关系</span><span class="sxs-lookup"><span data-stu-id="58a13-121">Relationships</span></span>
<span data-ttu-id="58a13-122">无</span><span class="sxs-lookup"><span data-stu-id="58a13-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58a13-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58a13-123">JSON Representation</span></span>
<span data-ttu-id="58a13-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58a13-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





