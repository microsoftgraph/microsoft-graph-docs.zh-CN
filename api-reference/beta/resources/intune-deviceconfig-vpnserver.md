---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bf45848059f7cbd74b408b4074b0ebc5c31b4e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573471"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="8d41d-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d41d-103">vpnServer resource type</span></span>

> <span data-ttu-id="8d41d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d41d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d41d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d41d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d41d-106">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="8d41d-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8d41d-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d41d-107">Properties</span></span>
|<span data-ttu-id="8d41d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d41d-108">Property</span></span>|<span data-ttu-id="8d41d-109">类型</span><span class="sxs-lookup"><span data-stu-id="8d41d-109">Type</span></span>|<span data-ttu-id="8d41d-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d41d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d41d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8d41d-111">description</span></span>|<span data-ttu-id="8d41d-112">String</span><span class="sxs-lookup"><span data-stu-id="8d41d-112">String</span></span>|<span data-ttu-id="8d41d-113">说明。</span><span class="sxs-lookup"><span data-stu-id="8d41d-113">Description.</span></span>|
|<span data-ttu-id="8d41d-114">address</span><span class="sxs-lookup"><span data-stu-id="8d41d-114">address</span></span>|<span data-ttu-id="8d41d-115">String</span><span class="sxs-lookup"><span data-stu-id="8d41d-115">String</span></span>|<span data-ttu-id="8d41d-116">地址 (IP 地址、FQDN 或 URL)</span><span class="sxs-lookup"><span data-stu-id="8d41d-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="8d41d-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="8d41d-117">isDefaultServer</span></span>|<span data-ttu-id="8d41d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d41d-118">Boolean</span></span>|<span data-ttu-id="8d41d-119">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="8d41d-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d41d-120">关系</span><span class="sxs-lookup"><span data-stu-id="8d41d-120">Relationships</span></span>
<span data-ttu-id="8d41d-121">无</span><span class="sxs-lookup"><span data-stu-id="8d41d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d41d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d41d-122">JSON Representation</span></span>
<span data-ttu-id="8d41d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d41d-123">Here is a JSON representation of the resource.</span></span>
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





