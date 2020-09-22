---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8054cea2a55ec9de260d2fcbc683aba341389b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048972"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="34ad4-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="34ad4-103">vpnServer resource type</span></span>

<span data-ttu-id="34ad4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34ad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34ad4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34ad4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34ad4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34ad4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ad4-107">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="34ad4-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="34ad4-108">属性</span><span class="sxs-lookup"><span data-stu-id="34ad4-108">Properties</span></span>
|<span data-ttu-id="34ad4-109">属性</span><span class="sxs-lookup"><span data-stu-id="34ad4-109">Property</span></span>|<span data-ttu-id="34ad4-110">类型</span><span class="sxs-lookup"><span data-stu-id="34ad4-110">Type</span></span>|<span data-ttu-id="34ad4-111">说明</span><span class="sxs-lookup"><span data-stu-id="34ad4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ad4-112">说明</span><span class="sxs-lookup"><span data-stu-id="34ad4-112">description</span></span>|<span data-ttu-id="34ad4-113">String</span><span class="sxs-lookup"><span data-stu-id="34ad4-113">String</span></span>|<span data-ttu-id="34ad4-114">说明。</span><span class="sxs-lookup"><span data-stu-id="34ad4-114">Description.</span></span>|
|<span data-ttu-id="34ad4-115">address</span><span class="sxs-lookup"><span data-stu-id="34ad4-115">address</span></span>|<span data-ttu-id="34ad4-116">String</span><span class="sxs-lookup"><span data-stu-id="34ad4-116">String</span></span>|<span data-ttu-id="34ad4-117">地址 (IP 地址、FQDN 或 URL) </span><span class="sxs-lookup"><span data-stu-id="34ad4-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="34ad4-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="34ad4-118">isDefaultServer</span></span>|<span data-ttu-id="34ad4-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ad4-119">Boolean</span></span>|<span data-ttu-id="34ad4-120">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="34ad4-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34ad4-121">关系</span><span class="sxs-lookup"><span data-stu-id="34ad4-121">Relationships</span></span>
<span data-ttu-id="34ad4-122">无</span><span class="sxs-lookup"><span data-stu-id="34ad4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34ad4-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34ad4-123">JSON Representation</span></span>
<span data-ttu-id="34ad4-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34ad4-124">Here is a JSON representation of the resource.</span></span>
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






