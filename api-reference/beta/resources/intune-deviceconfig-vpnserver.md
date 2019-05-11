---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67f0e91c0b2d024a07ab632a5e61e1106bbc65fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944521"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="93edf-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="93edf-103">vpnServer resource type</span></span>

> <span data-ttu-id="93edf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93edf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93edf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93edf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93edf-106">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="93edf-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="93edf-107">属性</span><span class="sxs-lookup"><span data-stu-id="93edf-107">Properties</span></span>
|<span data-ttu-id="93edf-108">属性</span><span class="sxs-lookup"><span data-stu-id="93edf-108">Property</span></span>|<span data-ttu-id="93edf-109">类型</span><span class="sxs-lookup"><span data-stu-id="93edf-109">Type</span></span>|<span data-ttu-id="93edf-110">说明</span><span class="sxs-lookup"><span data-stu-id="93edf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93edf-111">说明</span><span class="sxs-lookup"><span data-stu-id="93edf-111">description</span></span>|<span data-ttu-id="93edf-112">String</span><span class="sxs-lookup"><span data-stu-id="93edf-112">String</span></span>|<span data-ttu-id="93edf-113">说明。</span><span class="sxs-lookup"><span data-stu-id="93edf-113">Description.</span></span>|
|<span data-ttu-id="93edf-114">address</span><span class="sxs-lookup"><span data-stu-id="93edf-114">address</span></span>|<span data-ttu-id="93edf-115">String</span><span class="sxs-lookup"><span data-stu-id="93edf-115">String</span></span>|<span data-ttu-id="93edf-116">地址 (IP 地址、FQDN 或 URL)</span><span class="sxs-lookup"><span data-stu-id="93edf-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="93edf-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="93edf-117">isDefaultServer</span></span>|<span data-ttu-id="93edf-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="93edf-118">Boolean</span></span>|<span data-ttu-id="93edf-119">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="93edf-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93edf-120">关系</span><span class="sxs-lookup"><span data-stu-id="93edf-120">Relationships</span></span>
<span data-ttu-id="93edf-121">无</span><span class="sxs-lookup"><span data-stu-id="93edf-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93edf-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93edf-122">JSON Representation</span></span>
<span data-ttu-id="93edf-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93edf-123">Here is a JSON representation of the resource.</span></span>
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




