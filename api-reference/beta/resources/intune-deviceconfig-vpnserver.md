---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540741a6b3df349e5a096070e7973e3dadc2533e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987514"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="2d38d-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d38d-103">vpnServer resource type</span></span>

> <span data-ttu-id="2d38d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d38d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d38d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d38d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d38d-106">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="2d38d-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2d38d-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d38d-107">Properties</span></span>
|<span data-ttu-id="2d38d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d38d-108">Property</span></span>|<span data-ttu-id="2d38d-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d38d-109">Type</span></span>|<span data-ttu-id="2d38d-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d38d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d38d-111">说明</span><span class="sxs-lookup"><span data-stu-id="2d38d-111">description</span></span>|<span data-ttu-id="2d38d-112">String</span><span class="sxs-lookup"><span data-stu-id="2d38d-112">String</span></span>|<span data-ttu-id="2d38d-113">说明。</span><span class="sxs-lookup"><span data-stu-id="2d38d-113">Description.</span></span>|
|<span data-ttu-id="2d38d-114">address</span><span class="sxs-lookup"><span data-stu-id="2d38d-114">address</span></span>|<span data-ttu-id="2d38d-115">String</span><span class="sxs-lookup"><span data-stu-id="2d38d-115">String</span></span>|<span data-ttu-id="2d38d-116">地址 (IP 地址、FQDN 或 URL)</span><span class="sxs-lookup"><span data-stu-id="2d38d-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="2d38d-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="2d38d-117">isDefaultServer</span></span>|<span data-ttu-id="2d38d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d38d-118">Boolean</span></span>|<span data-ttu-id="2d38d-119">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="2d38d-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d38d-120">关系</span><span class="sxs-lookup"><span data-stu-id="2d38d-120">Relationships</span></span>
<span data-ttu-id="2d38d-121">无</span><span class="sxs-lookup"><span data-stu-id="2d38d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d38d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d38d-122">JSON Representation</span></span>
<span data-ttu-id="2d38d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d38d-123">Here is a JSON representation of the resource.</span></span>
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





