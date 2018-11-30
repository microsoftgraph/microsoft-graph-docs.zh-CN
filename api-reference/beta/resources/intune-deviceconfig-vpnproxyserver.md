---
title: vpnProxyServer 资源类型
description: VPN 代理服务器。
ms.openlocfilehash: 31e711475bf0f797eead80ca3fe2f3c9af8ba27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042836"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="3670b-103">vpnProxyServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="3670b-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="3670b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3670b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3670b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3670b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3670b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3670b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3670b-107">VPN 代理服务器。</span><span class="sxs-lookup"><span data-stu-id="3670b-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="3670b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3670b-108">Properties</span></span>
|<span data-ttu-id="3670b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3670b-109">Property</span></span>|<span data-ttu-id="3670b-110">类型</span><span class="sxs-lookup"><span data-stu-id="3670b-110">Type</span></span>|<span data-ttu-id="3670b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3670b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3670b-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="3670b-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="3670b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3670b-113">String</span></span>|<span data-ttu-id="3670b-114">代理服务器的自动配置脚本的 url。</span><span class="sxs-lookup"><span data-stu-id="3670b-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="3670b-115">address</span><span class="sxs-lookup"><span data-stu-id="3670b-115">address</span></span>|<span data-ttu-id="3670b-116">String</span><span class="sxs-lookup"><span data-stu-id="3670b-116">String</span></span>|<span data-ttu-id="3670b-117">地址。</span><span class="sxs-lookup"><span data-stu-id="3670b-117">Address.</span></span>|
|<span data-ttu-id="3670b-118">port</span><span class="sxs-lookup"><span data-stu-id="3670b-118">port</span></span>|<span data-ttu-id="3670b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="3670b-119">Int32</span></span>|<span data-ttu-id="3670b-120">端口。</span><span class="sxs-lookup"><span data-stu-id="3670b-120">Port.</span></span> <span data-ttu-id="3670b-121">有效的值 0 到 65535</span><span class="sxs-lookup"><span data-stu-id="3670b-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="3670b-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="3670b-122">Relationships</span></span>
<span data-ttu-id="3670b-123">无</span><span class="sxs-lookup"><span data-stu-id="3670b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3670b-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3670b-124">JSON Representation</span></span>
<span data-ttu-id="3670b-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3670b-125">Here is a JSON representation of the resource.</span></span>
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





