---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c2fda07e416c43246a035b556e6ee23f36ff56a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728312"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="8c7e7-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c7e7-103">vpnServer resource type</span></span>

<span data-ttu-id="8c7e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c7e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c7e7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c7e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c7e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c7e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c7e7-107">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="8c7e7-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8c7e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c7e7-108">Properties</span></span>
|<span data-ttu-id="8c7e7-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c7e7-109">Property</span></span>|<span data-ttu-id="8c7e7-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c7e7-110">Type</span></span>|<span data-ttu-id="8c7e7-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c7e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c7e7-112">说明</span><span class="sxs-lookup"><span data-stu-id="8c7e7-112">description</span></span>|<span data-ttu-id="8c7e7-113">String</span><span class="sxs-lookup"><span data-stu-id="8c7e7-113">String</span></span>|<span data-ttu-id="8c7e7-114">说明。</span><span class="sxs-lookup"><span data-stu-id="8c7e7-114">Description.</span></span>|
|<span data-ttu-id="8c7e7-115">address</span><span class="sxs-lookup"><span data-stu-id="8c7e7-115">address</span></span>|<span data-ttu-id="8c7e7-116">String</span><span class="sxs-lookup"><span data-stu-id="8c7e7-116">String</span></span>|<span data-ttu-id="8c7e7-117">地址 (IP 地址、FQDN 或 URL) </span><span class="sxs-lookup"><span data-stu-id="8c7e7-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="8c7e7-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="8c7e7-118">isDefaultServer</span></span>|<span data-ttu-id="8c7e7-119">布尔</span><span class="sxs-lookup"><span data-stu-id="8c7e7-119">Boolean</span></span>|<span data-ttu-id="8c7e7-120">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="8c7e7-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c7e7-121">关系</span><span class="sxs-lookup"><span data-stu-id="8c7e7-121">Relationships</span></span>
<span data-ttu-id="8c7e7-122">无</span><span class="sxs-lookup"><span data-stu-id="8c7e7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c7e7-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c7e7-123">JSON Representation</span></span>
<span data-ttu-id="8c7e7-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c7e7-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





