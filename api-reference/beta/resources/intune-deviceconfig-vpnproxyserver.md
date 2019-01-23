---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 676e56771f021a79179e268280f5e3190754eef2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425671"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="07b90-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="07b90-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="07b90-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="07b90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07b90-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="07b90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07b90-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07b90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07b90-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="07b90-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="07b90-108">属性</span><span class="sxs-lookup"><span data-stu-id="07b90-108">Properties</span></span>
|<span data-ttu-id="07b90-109">属性</span><span class="sxs-lookup"><span data-stu-id="07b90-109">Property</span></span>|<span data-ttu-id="07b90-110">类型</span><span class="sxs-lookup"><span data-stu-id="07b90-110">Type</span></span>|<span data-ttu-id="07b90-111">说明</span><span class="sxs-lookup"><span data-stu-id="07b90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07b90-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="07b90-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="07b90-113">String</span><span class="sxs-lookup"><span data-stu-id="07b90-113">String</span></span>|<span data-ttu-id="07b90-114">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="07b90-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="07b90-115">address</span><span class="sxs-lookup"><span data-stu-id="07b90-115">address</span></span>|<span data-ttu-id="07b90-116">String</span><span class="sxs-lookup"><span data-stu-id="07b90-116">String</span></span>|<span data-ttu-id="07b90-117">地址。</span><span class="sxs-lookup"><span data-stu-id="07b90-117">Address.</span></span>|
|<span data-ttu-id="07b90-118">port</span><span class="sxs-lookup"><span data-stu-id="07b90-118">port</span></span>|<span data-ttu-id="07b90-119">Int32</span><span class="sxs-lookup"><span data-stu-id="07b90-119">Int32</span></span>|<span data-ttu-id="07b90-120">端口。</span><span class="sxs-lookup"><span data-stu-id="07b90-120">Port.</span></span> <span data-ttu-id="07b90-121">有效的值 0 到 65535</span><span class="sxs-lookup"><span data-stu-id="07b90-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="07b90-122">关系</span><span class="sxs-lookup"><span data-stu-id="07b90-122">Relationships</span></span>
<span data-ttu-id="07b90-123">无</span><span class="sxs-lookup"><span data-stu-id="07b90-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07b90-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07b90-124">JSON Representation</span></span>
<span data-ttu-id="07b90-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07b90-125">Here is a JSON representation of the resource.</span></span>
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




