---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c383c539cf74bbbd4119294ea150394e37bf1a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529293"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="9351f-103">vpnRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="9351f-103">vpnRoute resource type</span></span>

<span data-ttu-id="9351f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9351f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9351f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9351f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9351f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9351f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9351f-107">VPN 路由定义。</span><span class="sxs-lookup"><span data-stu-id="9351f-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9351f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9351f-108">Properties</span></span>
|<span data-ttu-id="9351f-109">属性</span><span class="sxs-lookup"><span data-stu-id="9351f-109">Property</span></span>|<span data-ttu-id="9351f-110">类型</span><span class="sxs-lookup"><span data-stu-id="9351f-110">Type</span></span>|<span data-ttu-id="9351f-111">说明</span><span class="sxs-lookup"><span data-stu-id="9351f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9351f-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="9351f-112">destinationPrefix</span></span>|<span data-ttu-id="9351f-113">String</span><span class="sxs-lookup"><span data-stu-id="9351f-113">String</span></span>|<span data-ttu-id="9351f-114">目标前缀（IPv4/v6 地址）。</span><span class="sxs-lookup"><span data-stu-id="9351f-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="9351f-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="9351f-115">prefixSize</span></span>|<span data-ttu-id="9351f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9351f-116">Int32</span></span>|<span data-ttu-id="9351f-117">前缀大小。</span><span class="sxs-lookup"><span data-stu-id="9351f-117">Prefix size.</span></span> <span data-ttu-id="9351f-118">（1-32）。</span><span class="sxs-lookup"><span data-stu-id="9351f-118">(1-32).</span></span> <span data-ttu-id="9351f-119">有效值为1至32</span><span class="sxs-lookup"><span data-stu-id="9351f-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="9351f-120">关系</span><span class="sxs-lookup"><span data-stu-id="9351f-120">Relationships</span></span>
<span data-ttu-id="9351f-121">无</span><span class="sxs-lookup"><span data-stu-id="9351f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9351f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9351f-122">JSON Representation</span></span>
<span data-ttu-id="9351f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9351f-123">Here is a JSON representation of the resource.</span></span>
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



