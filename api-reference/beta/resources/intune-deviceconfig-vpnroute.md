---
title: vpnRoute 资源类型
description: VPN 路由定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 628e2f384b06dece13da1595a4111a2d1022a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423018"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="fe08f-103">vpnRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe08f-103">vpnRoute resource type</span></span>

> <span data-ttu-id="fe08f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fe08f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe08f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe08f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe08f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe08f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe08f-107">VPN 路由定义。</span><span class="sxs-lookup"><span data-stu-id="fe08f-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fe08f-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe08f-108">Properties</span></span>
|<span data-ttu-id="fe08f-109">属性</span><span class="sxs-lookup"><span data-stu-id="fe08f-109">Property</span></span>|<span data-ttu-id="fe08f-110">类型</span><span class="sxs-lookup"><span data-stu-id="fe08f-110">Type</span></span>|<span data-ttu-id="fe08f-111">说明</span><span class="sxs-lookup"><span data-stu-id="fe08f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe08f-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="fe08f-112">destinationPrefix</span></span>|<span data-ttu-id="fe08f-113">String</span><span class="sxs-lookup"><span data-stu-id="fe08f-113">String</span></span>|<span data-ttu-id="fe08f-114">目标前缀 （IPv4/v6 地址）。</span><span class="sxs-lookup"><span data-stu-id="fe08f-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="fe08f-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="fe08f-115">prefixSize</span></span>|<span data-ttu-id="fe08f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fe08f-116">Int32</span></span>|<span data-ttu-id="fe08f-117">前缀大小。</span><span class="sxs-lookup"><span data-stu-id="fe08f-117">Prefix size.</span></span> <span data-ttu-id="fe08f-118">(1-32)。</span><span class="sxs-lookup"><span data-stu-id="fe08f-118">(1-32).</span></span> <span data-ttu-id="fe08f-119">有效的值 1 到 32</span><span class="sxs-lookup"><span data-stu-id="fe08f-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe08f-120">关系</span><span class="sxs-lookup"><span data-stu-id="fe08f-120">Relationships</span></span>
<span data-ttu-id="fe08f-121">无</span><span class="sxs-lookup"><span data-stu-id="fe08f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe08f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe08f-122">JSON Representation</span></span>
<span data-ttu-id="fe08f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe08f-123">Here is a JSON representation of the resource.</span></span>
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




