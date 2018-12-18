---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: tfitzmac
ms.openlocfilehash: 64d755c4f21b47e928c64348a2f1d6dad1f7206a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322020"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="7fa86-103">vpnRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fa86-103">vpnRoute resource type</span></span>

> <span data-ttu-id="7fa86-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7fa86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fa86-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7fa86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fa86-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7fa86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fa86-107">VPN 路由定义。</span><span class="sxs-lookup"><span data-stu-id="7fa86-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="7fa86-108">属性</span><span class="sxs-lookup"><span data-stu-id="7fa86-108">Properties</span></span>
|<span data-ttu-id="7fa86-109">属性</span><span class="sxs-lookup"><span data-stu-id="7fa86-109">Property</span></span>|<span data-ttu-id="7fa86-110">类型</span><span class="sxs-lookup"><span data-stu-id="7fa86-110">Type</span></span>|<span data-ttu-id="7fa86-111">说明</span><span class="sxs-lookup"><span data-stu-id="7fa86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fa86-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="7fa86-112">destinationPrefix</span></span>|<span data-ttu-id="7fa86-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7fa86-113">String</span></span>|<span data-ttu-id="7fa86-114">目标前缀 （IPv4/v6 地址）。</span><span class="sxs-lookup"><span data-stu-id="7fa86-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="7fa86-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="7fa86-115">prefixSize</span></span>|<span data-ttu-id="7fa86-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7fa86-116">Int32</span></span>|<span data-ttu-id="7fa86-117">前缀大小。</span><span class="sxs-lookup"><span data-stu-id="7fa86-117">Prefix size.</span></span> <span data-ttu-id="7fa86-118">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="7fa86-118">(1-32).</span></span> <span data-ttu-id="7fa86-119">有效的值 1 到 32</span><span class="sxs-lookup"><span data-stu-id="7fa86-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fa86-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="7fa86-120">Relationships</span></span>
<span data-ttu-id="7fa86-121">无</span><span class="sxs-lookup"><span data-stu-id="7fa86-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7fa86-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fa86-122">JSON Representation</span></span>
<span data-ttu-id="7fa86-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fa86-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```





