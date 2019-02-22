---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8a452cdde7c4c360107a67396d8f5ce49d6eb1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145274"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="c8e81-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8e81-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="c8e81-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8e81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8e81-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8e81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8e81-106">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c8e81-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="c8e81-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8e81-107">Properties</span></span>
|<span data-ttu-id="c8e81-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8e81-108">Property</span></span>|<span data-ttu-id="c8e81-109">类型</span><span class="sxs-lookup"><span data-stu-id="c8e81-109">Type</span></span>|<span data-ttu-id="c8e81-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8e81-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8e81-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="c8e81-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="c8e81-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c8e81-112">String</span></span>|<span data-ttu-id="c8e81-113">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="c8e81-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="c8e81-114">address</span><span class="sxs-lookup"><span data-stu-id="c8e81-114">address</span></span>|<span data-ttu-id="c8e81-115">String</span><span class="sxs-lookup"><span data-stu-id="c8e81-115">String</span></span>|<span data-ttu-id="c8e81-116">处理.</span><span class="sxs-lookup"><span data-stu-id="c8e81-116">Address.</span></span>|
|<span data-ttu-id="c8e81-117">port</span><span class="sxs-lookup"><span data-stu-id="c8e81-117">port</span></span>|<span data-ttu-id="c8e81-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c8e81-118">Int32</span></span>|<span data-ttu-id="c8e81-119">端口.</span><span class="sxs-lookup"><span data-stu-id="c8e81-119">Port.</span></span> <span data-ttu-id="c8e81-120">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="c8e81-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8e81-121">关系</span><span class="sxs-lookup"><span data-stu-id="c8e81-121">Relationships</span></span>
<span data-ttu-id="c8e81-122">无</span><span class="sxs-lookup"><span data-stu-id="c8e81-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8e81-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8e81-123">JSON Representation</span></span>
<span data-ttu-id="c8e81-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8e81-124">Here is a JSON representation of the resource.</span></span>
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




