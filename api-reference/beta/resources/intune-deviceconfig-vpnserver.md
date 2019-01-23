---
title: vpnServer 资源类型
description: VPN 服务器定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0febdae5745f1295e9c690213d4a51b79d7d3bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406806"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="1a225-103">vpnServer 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a225-103">vpnServer resource type</span></span>

> <span data-ttu-id="1a225-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1a225-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a225-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a225-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a225-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a225-107">VPN 服务器定义。</span><span class="sxs-lookup"><span data-stu-id="1a225-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1a225-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a225-108">Properties</span></span>
|<span data-ttu-id="1a225-109">属性</span><span class="sxs-lookup"><span data-stu-id="1a225-109">Property</span></span>|<span data-ttu-id="1a225-110">类型</span><span class="sxs-lookup"><span data-stu-id="1a225-110">Type</span></span>|<span data-ttu-id="1a225-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a225-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a225-112">说明</span><span class="sxs-lookup"><span data-stu-id="1a225-112">description</span></span>|<span data-ttu-id="1a225-113">String</span><span class="sxs-lookup"><span data-stu-id="1a225-113">String</span></span>|<span data-ttu-id="1a225-114">说明。</span><span class="sxs-lookup"><span data-stu-id="1a225-114">Description.</span></span>|
|<span data-ttu-id="1a225-115">address</span><span class="sxs-lookup"><span data-stu-id="1a225-115">address</span></span>|<span data-ttu-id="1a225-116">String</span><span class="sxs-lookup"><span data-stu-id="1a225-116">String</span></span>|<span data-ttu-id="1a225-117">地址 （IP 地址、 FQDN 或 URL）</span><span class="sxs-lookup"><span data-stu-id="1a225-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="1a225-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="1a225-118">isDefaultServer</span></span>|<span data-ttu-id="1a225-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a225-119">Boolean</span></span>|<span data-ttu-id="1a225-120">默认服务器。</span><span class="sxs-lookup"><span data-stu-id="1a225-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a225-121">关系</span><span class="sxs-lookup"><span data-stu-id="1a225-121">Relationships</span></span>
<span data-ttu-id="1a225-122">无</span><span class="sxs-lookup"><span data-stu-id="1a225-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a225-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a225-123">JSON Representation</span></span>
<span data-ttu-id="1a225-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a225-124">Here is a JSON representation of the resource.</span></span>
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




