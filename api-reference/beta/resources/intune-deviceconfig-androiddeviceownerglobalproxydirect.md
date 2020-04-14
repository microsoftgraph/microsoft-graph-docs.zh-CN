---
title: androidDeviceOwnerGlobalProxyDirect 资源类型
description: Android 设备所有者全局代理 Direct。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f1b57ebdfb44504295824637352d543ff64111e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463484"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="a62e5-103">androidDeviceOwnerGlobalProxyDirect 资源类型</span><span class="sxs-lookup"><span data-stu-id="a62e5-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

<span data-ttu-id="a62e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a62e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a62e5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a62e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a62e5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a62e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a62e5-107">Android 设备所有者全局代理 Direct。</span><span class="sxs-lookup"><span data-stu-id="a62e5-107">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="a62e5-108">继承自[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="a62e5-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a62e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="a62e5-109">Properties</span></span>
|<span data-ttu-id="a62e5-110">属性</span><span class="sxs-lookup"><span data-stu-id="a62e5-110">Property</span></span>|<span data-ttu-id="a62e5-111">类型</span><span class="sxs-lookup"><span data-stu-id="a62e5-111">Type</span></span>|<span data-ttu-id="a62e5-112">说明</span><span class="sxs-lookup"><span data-stu-id="a62e5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a62e5-113">host</span><span class="sxs-lookup"><span data-stu-id="a62e5-113">host</span></span>|<span data-ttu-id="a62e5-114">String</span><span class="sxs-lookup"><span data-stu-id="a62e5-114">String</span></span>|<span data-ttu-id="a62e5-115">主机名</span><span class="sxs-lookup"><span data-stu-id="a62e5-115">The host name</span></span>|
|<span data-ttu-id="a62e5-116">端口</span><span class="sxs-lookup"><span data-stu-id="a62e5-116">port</span></span>|<span data-ttu-id="a62e5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="a62e5-117">Int32</span></span>|<span data-ttu-id="a62e5-118">端口</span><span class="sxs-lookup"><span data-stu-id="a62e5-118">The port</span></span>|
|<span data-ttu-id="a62e5-119">excludedHosts</span><span class="sxs-lookup"><span data-stu-id="a62e5-119">excludedHosts</span></span>|<span data-ttu-id="a62e5-120">String collection</span><span class="sxs-lookup"><span data-stu-id="a62e5-120">String collection</span></span>|<span data-ttu-id="a62e5-121">已排除的主机</span><span class="sxs-lookup"><span data-stu-id="a62e5-121">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="a62e5-122">关系</span><span class="sxs-lookup"><span data-stu-id="a62e5-122">Relationships</span></span>
<span data-ttu-id="a62e5-123">无</span><span class="sxs-lookup"><span data-stu-id="a62e5-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a62e5-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a62e5-124">JSON Representation</span></span>
<span data-ttu-id="a62e5-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a62e5-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyDirect"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyDirect",
  "host": "String",
  "port": 1024,
  "excludedHosts": [
    "String"
  ]
}
```



