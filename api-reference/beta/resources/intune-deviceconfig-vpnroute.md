---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ee8e52bb838a688f11d4242ce85241fe0c06122
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420323"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="32d27-103">vpnRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="32d27-103">vpnRoute resource type</span></span>

<span data-ttu-id="32d27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32d27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32d27-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32d27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32d27-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32d27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32d27-107">VPN 路由定义。</span><span class="sxs-lookup"><span data-stu-id="32d27-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="32d27-108">属性</span><span class="sxs-lookup"><span data-stu-id="32d27-108">Properties</span></span>
|<span data-ttu-id="32d27-109">属性</span><span class="sxs-lookup"><span data-stu-id="32d27-109">Property</span></span>|<span data-ttu-id="32d27-110">类型</span><span class="sxs-lookup"><span data-stu-id="32d27-110">Type</span></span>|<span data-ttu-id="32d27-111">说明</span><span class="sxs-lookup"><span data-stu-id="32d27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32d27-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="32d27-112">destinationPrefix</span></span>|<span data-ttu-id="32d27-113">String</span><span class="sxs-lookup"><span data-stu-id="32d27-113">String</span></span>|<span data-ttu-id="32d27-114">目标前缀（IPv4/v6 地址）。</span><span class="sxs-lookup"><span data-stu-id="32d27-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="32d27-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="32d27-115">prefixSize</span></span>|<span data-ttu-id="32d27-116">Int32</span><span class="sxs-lookup"><span data-stu-id="32d27-116">Int32</span></span>|<span data-ttu-id="32d27-117">前缀大小。</span><span class="sxs-lookup"><span data-stu-id="32d27-117">Prefix size.</span></span> <span data-ttu-id="32d27-118">（1-32）。</span><span class="sxs-lookup"><span data-stu-id="32d27-118">(1-32).</span></span> <span data-ttu-id="32d27-119">有效值为1至32</span><span class="sxs-lookup"><span data-stu-id="32d27-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="32d27-120">关系</span><span class="sxs-lookup"><span data-stu-id="32d27-120">Relationships</span></span>
<span data-ttu-id="32d27-121">无</span><span class="sxs-lookup"><span data-stu-id="32d27-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32d27-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32d27-122">JSON Representation</span></span>
<span data-ttu-id="32d27-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32d27-123">Here is a JSON representation of the resource.</span></span>
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



