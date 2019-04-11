---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bf45848059f7cbd74b408b4074b0ebc5c31b4e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782833"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="97118-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="97118-103">vpnServer resource type</span></span>

> <span data-ttu-id="97118-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97118-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97118-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97118-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97118-106">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="97118-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="97118-107">属性</span><span class="sxs-lookup"><span data-stu-id="97118-107">Properties</span></span>
|<span data-ttu-id="97118-108">属性</span><span class="sxs-lookup"><span data-stu-id="97118-108">Property</span></span>|<span data-ttu-id="97118-109">类型</span><span class="sxs-lookup"><span data-stu-id="97118-109">Type</span></span>|<span data-ttu-id="97118-110">说明</span><span class="sxs-lookup"><span data-stu-id="97118-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97118-111">说明</span><span class="sxs-lookup"><span data-stu-id="97118-111">description</span></span>|<span data-ttu-id="97118-112">String</span><span class="sxs-lookup"><span data-stu-id="97118-112">String</span></span>|<span data-ttu-id="97118-113">说明。</span><span class="sxs-lookup"><span data-stu-id="97118-113">Description.</span></span>|
|<span data-ttu-id="97118-114">address</span><span class="sxs-lookup"><span data-stu-id="97118-114">address</span></span>|<span data-ttu-id="97118-115">String</span><span class="sxs-lookup"><span data-stu-id="97118-115">String</span></span>|<span data-ttu-id="97118-116">地址 (IP 地址、FQDN 或 URL)</span><span class="sxs-lookup"><span data-stu-id="97118-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="97118-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="97118-117">isDefaultServer</span></span>|<span data-ttu-id="97118-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="97118-118">Boolean</span></span>|<span data-ttu-id="97118-119">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="97118-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97118-120">关系</span><span class="sxs-lookup"><span data-stu-id="97118-120">Relationships</span></span>
<span data-ttu-id="97118-121">无</span><span class="sxs-lookup"><span data-stu-id="97118-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97118-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97118-122">JSON Representation</span></span>
<span data-ttu-id="97118-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97118-123">Here is a JSON representation of the resource.</span></span>
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





