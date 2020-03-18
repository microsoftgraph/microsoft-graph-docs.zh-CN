---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e0d5b07aa04d7e47459923b1b33d3d32008dcc1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787325"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="056ee-103">vpnRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="056ee-103">vpnRoute resource type</span></span>

> <span data-ttu-id="056ee-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="056ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="056ee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="056ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="056ee-106">VPN 路由定义。</span><span class="sxs-lookup"><span data-stu-id="056ee-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="056ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="056ee-107">Properties</span></span>
|<span data-ttu-id="056ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="056ee-108">Property</span></span>|<span data-ttu-id="056ee-109">类型</span><span class="sxs-lookup"><span data-stu-id="056ee-109">Type</span></span>|<span data-ttu-id="056ee-110">说明</span><span class="sxs-lookup"><span data-stu-id="056ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="056ee-111">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="056ee-111">destinationPrefix</span></span>|<span data-ttu-id="056ee-112">String</span><span class="sxs-lookup"><span data-stu-id="056ee-112">String</span></span>|<span data-ttu-id="056ee-113">目标前缀（IPv4/v6 地址）。</span><span class="sxs-lookup"><span data-stu-id="056ee-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="056ee-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="056ee-114">prefixSize</span></span>|<span data-ttu-id="056ee-115">Int32</span><span class="sxs-lookup"><span data-stu-id="056ee-115">Int32</span></span>|<span data-ttu-id="056ee-116">前缀大小。</span><span class="sxs-lookup"><span data-stu-id="056ee-116">Prefix size.</span></span> <span data-ttu-id="056ee-117">（1-32）。</span><span class="sxs-lookup"><span data-stu-id="056ee-117">(1-32).</span></span> <span data-ttu-id="056ee-118">有效值为1至32</span><span class="sxs-lookup"><span data-stu-id="056ee-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="056ee-119">关系</span><span class="sxs-lookup"><span data-stu-id="056ee-119">Relationships</span></span>
<span data-ttu-id="056ee-120">无</span><span class="sxs-lookup"><span data-stu-id="056ee-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="056ee-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="056ee-121">JSON Representation</span></span>
<span data-ttu-id="056ee-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="056ee-122">Here is a JSON representation of the resource.</span></span>
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



