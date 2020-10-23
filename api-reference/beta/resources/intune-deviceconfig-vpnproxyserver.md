---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 013511c027600dd8e787959dc967d99b47c21bc8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728319"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="1c80d-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c80d-103">vpnProxyServer resource type</span></span>

<span data-ttu-id="1c80d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c80d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c80d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c80d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c80d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c80d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c80d-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="1c80d-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="1c80d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c80d-108">Properties</span></span>
|<span data-ttu-id="1c80d-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c80d-109">Property</span></span>|<span data-ttu-id="1c80d-110">类型</span><span class="sxs-lookup"><span data-stu-id="1c80d-110">Type</span></span>|<span data-ttu-id="1c80d-111">说明</span><span class="sxs-lookup"><span data-stu-id="1c80d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c80d-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="1c80d-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="1c80d-113">String</span><span class="sxs-lookup"><span data-stu-id="1c80d-113">String</span></span>|<span data-ttu-id="1c80d-114">代理的自动配置脚本 url。</span><span class="sxs-lookup"><span data-stu-id="1c80d-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="1c80d-115">address</span><span class="sxs-lookup"><span data-stu-id="1c80d-115">address</span></span>|<span data-ttu-id="1c80d-116">String</span><span class="sxs-lookup"><span data-stu-id="1c80d-116">String</span></span>|<span data-ttu-id="1c80d-117">处理.</span><span class="sxs-lookup"><span data-stu-id="1c80d-117">Address.</span></span>|
|<span data-ttu-id="1c80d-118">端口</span><span class="sxs-lookup"><span data-stu-id="1c80d-118">port</span></span>|<span data-ttu-id="1c80d-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1c80d-119">Int32</span></span>|<span data-ttu-id="1c80d-120">端口.</span><span class="sxs-lookup"><span data-stu-id="1c80d-120">Port.</span></span> <span data-ttu-id="1c80d-121">有效值为0至65535</span><span class="sxs-lookup"><span data-stu-id="1c80d-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c80d-122">关系</span><span class="sxs-lookup"><span data-stu-id="1c80d-122">Relationships</span></span>
<span data-ttu-id="1c80d-123">无</span><span class="sxs-lookup"><span data-stu-id="1c80d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c80d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c80d-124">JSON Representation</span></span>
<span data-ttu-id="1c80d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c80d-125">Here is a JSON representation of the resource.</span></span>
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





