---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b4842444bc248e51e1967fcbef4a863ed50498c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867674"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="bbb9b-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="bbb9b-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="bbb9b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbb9b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbb9b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbb9b-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="bbb9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="bbb9b-108">Properties</span></span>
|<span data-ttu-id="bbb9b-109">属性</span><span class="sxs-lookup"><span data-stu-id="bbb9b-109">Property</span></span>|<span data-ttu-id="bbb9b-110">类型</span><span class="sxs-lookup"><span data-stu-id="bbb9b-110">Type</span></span>|<span data-ttu-id="bbb9b-111">Description</span><span class="sxs-lookup"><span data-stu-id="bbb9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb9b-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="bbb9b-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="bbb9b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="bbb9b-113">String</span></span>|<span data-ttu-id="bbb9b-114">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="bbb9b-115">address</span><span class="sxs-lookup"><span data-stu-id="bbb9b-115">address</span></span>|<span data-ttu-id="bbb9b-116">String</span><span class="sxs-lookup"><span data-stu-id="bbb9b-116">String</span></span>|<span data-ttu-id="bbb9b-117">地址。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-117">Address.</span></span>|
|<span data-ttu-id="bbb9b-118">port</span><span class="sxs-lookup"><span data-stu-id="bbb9b-118">port</span></span>|<span data-ttu-id="bbb9b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="bbb9b-119">Int32</span></span>|<span data-ttu-id="bbb9b-120">端口。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-120">Port.</span></span> <span data-ttu-id="bbb9b-121">有效的值 0 到 65535</span><span class="sxs-lookup"><span data-stu-id="bbb9b-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbb9b-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="bbb9b-122">Relationships</span></span>
<span data-ttu-id="bbb9b-123">无</span><span class="sxs-lookup"><span data-stu-id="bbb9b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bbb9b-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbb9b-124">JSON Representation</span></span>
<span data-ttu-id="bbb9b-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbb9b-125">Here is a JSON representation of the resource.</span></span>
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





