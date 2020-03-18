---
title: androidDeviceOwnerGlobalProxyDirect 资源类型
description: Android 设备所有者全局代理 Direct。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc2b960b85fd7fac506423af4d3a380247fb4892
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797005"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="cbff9-103">androidDeviceOwnerGlobalProxyDirect 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbff9-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

> <span data-ttu-id="cbff9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbff9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbff9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbff9-106">Android 设备所有者全局代理 Direct。</span><span class="sxs-lookup"><span data-stu-id="cbff9-106">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="cbff9-107">继承自[androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="cbff9-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cbff9-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbff9-108">Properties</span></span>
|<span data-ttu-id="cbff9-109">属性</span><span class="sxs-lookup"><span data-stu-id="cbff9-109">Property</span></span>|<span data-ttu-id="cbff9-110">类型</span><span class="sxs-lookup"><span data-stu-id="cbff9-110">Type</span></span>|<span data-ttu-id="cbff9-111">说明</span><span class="sxs-lookup"><span data-stu-id="cbff9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbff9-112">host</span><span class="sxs-lookup"><span data-stu-id="cbff9-112">host</span></span>|<span data-ttu-id="cbff9-113">String</span><span class="sxs-lookup"><span data-stu-id="cbff9-113">String</span></span>|<span data-ttu-id="cbff9-114">主机名</span><span class="sxs-lookup"><span data-stu-id="cbff9-114">The host name</span></span>|
|<span data-ttu-id="cbff9-115">端口</span><span class="sxs-lookup"><span data-stu-id="cbff9-115">port</span></span>|<span data-ttu-id="cbff9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cbff9-116">Int32</span></span>|<span data-ttu-id="cbff9-117">端口</span><span class="sxs-lookup"><span data-stu-id="cbff9-117">The port</span></span>|
|<span data-ttu-id="cbff9-118">excludedHosts</span><span class="sxs-lookup"><span data-stu-id="cbff9-118">excludedHosts</span></span>|<span data-ttu-id="cbff9-119">String collection</span><span class="sxs-lookup"><span data-stu-id="cbff9-119">String collection</span></span>|<span data-ttu-id="cbff9-120">已排除的主机</span><span class="sxs-lookup"><span data-stu-id="cbff9-120">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbff9-121">关系</span><span class="sxs-lookup"><span data-stu-id="cbff9-121">Relationships</span></span>
<span data-ttu-id="cbff9-122">无</span><span class="sxs-lookup"><span data-stu-id="cbff9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbff9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbff9-123">JSON Representation</span></span>
<span data-ttu-id="cbff9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbff9-124">Here is a JSON representation of the resource.</span></span>
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



