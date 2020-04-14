---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cf550e25c1f777e9f78fd20bdf2863e79f491b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412029"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="fd597-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd597-103">vpnProxyServer resource type</span></span>

<span data-ttu-id="fd597-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd597-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd597-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd597-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd597-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd597-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd597-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="fd597-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="fd597-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd597-108">Properties</span></span>
|<span data-ttu-id="fd597-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd597-109">Property</span></span>|<span data-ttu-id="fd597-110">类型</span><span class="sxs-lookup"><span data-stu-id="fd597-110">Type</span></span>|<span data-ttu-id="fd597-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd597-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd597-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="fd597-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="fd597-113">String</span><span class="sxs-lookup"><span data-stu-id="fd597-113">String</span></span>|<span data-ttu-id="fd597-114">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="fd597-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="fd597-115">address</span><span class="sxs-lookup"><span data-stu-id="fd597-115">address</span></span>|<span data-ttu-id="fd597-116">String</span><span class="sxs-lookup"><span data-stu-id="fd597-116">String</span></span>|<span data-ttu-id="fd597-117">处理.</span><span class="sxs-lookup"><span data-stu-id="fd597-117">Address.</span></span>|
|<span data-ttu-id="fd597-118">端口</span><span class="sxs-lookup"><span data-stu-id="fd597-118">port</span></span>|<span data-ttu-id="fd597-119">Int32</span><span class="sxs-lookup"><span data-stu-id="fd597-119">Int32</span></span>|<span data-ttu-id="fd597-120">端口.</span><span class="sxs-lookup"><span data-stu-id="fd597-120">Port.</span></span> <span data-ttu-id="fd597-121">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="fd597-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd597-122">关系</span><span class="sxs-lookup"><span data-stu-id="fd597-122">Relationships</span></span>
<span data-ttu-id="fd597-123">无</span><span class="sxs-lookup"><span data-stu-id="fd597-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd597-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd597-124">JSON Representation</span></span>
<span data-ttu-id="fd597-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd597-125">Here is a JSON representation of the resource.</span></span>
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



