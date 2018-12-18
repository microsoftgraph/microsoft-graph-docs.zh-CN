---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
ms.openlocfilehash: f622d476e041fd89a639c14113e273a16aca992f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333472"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="fe976-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe976-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="fe976-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe976-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe976-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe976-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe976-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fe976-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe976-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="fe976-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="fe976-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe976-108">Properties</span></span>
|<span data-ttu-id="fe976-109">属性</span><span class="sxs-lookup"><span data-stu-id="fe976-109">Property</span></span>|<span data-ttu-id="fe976-110">类型</span><span class="sxs-lookup"><span data-stu-id="fe976-110">Type</span></span>|<span data-ttu-id="fe976-111">说明</span><span class="sxs-lookup"><span data-stu-id="fe976-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe976-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="fe976-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="fe976-113">字符串</span><span class="sxs-lookup"><span data-stu-id="fe976-113">String</span></span>|<span data-ttu-id="fe976-114">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="fe976-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="fe976-115">address</span><span class="sxs-lookup"><span data-stu-id="fe976-115">address</span></span>|<span data-ttu-id="fe976-116">String</span><span class="sxs-lookup"><span data-stu-id="fe976-116">String</span></span>|<span data-ttu-id="fe976-117">地址。</span><span class="sxs-lookup"><span data-stu-id="fe976-117">Address.</span></span>|
|<span data-ttu-id="fe976-118">port</span><span class="sxs-lookup"><span data-stu-id="fe976-118">port</span></span>|<span data-ttu-id="fe976-119">Int32</span><span class="sxs-lookup"><span data-stu-id="fe976-119">Int32</span></span>|<span data-ttu-id="fe976-120">端口。</span><span class="sxs-lookup"><span data-stu-id="fe976-120">Port.</span></span> <span data-ttu-id="fe976-121">有效的值 0 到 65535</span><span class="sxs-lookup"><span data-stu-id="fe976-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe976-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="fe976-122">Relationships</span></span>
<span data-ttu-id="fe976-123">无</span><span class="sxs-lookup"><span data-stu-id="fe976-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe976-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe976-124">JSON Representation</span></span>
<span data-ttu-id="fe976-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe976-125">Here is a JSON representation of the resource.</span></span>
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





