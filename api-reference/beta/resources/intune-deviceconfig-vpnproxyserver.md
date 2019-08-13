---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: faa9a1bd74a9535cccca8d387a5a8a23de6db3b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367615"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="62196-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="62196-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="62196-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62196-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62196-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62196-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62196-106">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="62196-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="62196-107">属性</span><span class="sxs-lookup"><span data-stu-id="62196-107">Properties</span></span>
|<span data-ttu-id="62196-108">属性</span><span class="sxs-lookup"><span data-stu-id="62196-108">Property</span></span>|<span data-ttu-id="62196-109">类型</span><span class="sxs-lookup"><span data-stu-id="62196-109">Type</span></span>|<span data-ttu-id="62196-110">说明</span><span class="sxs-lookup"><span data-stu-id="62196-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62196-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="62196-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="62196-112">String</span><span class="sxs-lookup"><span data-stu-id="62196-112">String</span></span>|<span data-ttu-id="62196-113">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="62196-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="62196-114">address</span><span class="sxs-lookup"><span data-stu-id="62196-114">address</span></span>|<span data-ttu-id="62196-115">String</span><span class="sxs-lookup"><span data-stu-id="62196-115">String</span></span>|<span data-ttu-id="62196-116">处理.</span><span class="sxs-lookup"><span data-stu-id="62196-116">Address.</span></span>|
|<span data-ttu-id="62196-117">端口</span><span class="sxs-lookup"><span data-stu-id="62196-117">port</span></span>|<span data-ttu-id="62196-118">Int32</span><span class="sxs-lookup"><span data-stu-id="62196-118">Int32</span></span>|<span data-ttu-id="62196-119">端口.</span><span class="sxs-lookup"><span data-stu-id="62196-119">Port.</span></span> <span data-ttu-id="62196-120">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="62196-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="62196-121">关系</span><span class="sxs-lookup"><span data-stu-id="62196-121">Relationships</span></span>
<span data-ttu-id="62196-122">无</span><span class="sxs-lookup"><span data-stu-id="62196-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62196-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62196-123">JSON Representation</span></span>
<span data-ttu-id="62196-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62196-124">Here is a JSON representation of the resource.</span></span>
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



