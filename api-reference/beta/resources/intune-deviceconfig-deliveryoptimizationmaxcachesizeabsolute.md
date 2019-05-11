---
title: deliveryOptimizationMaxCacheSizeAbsolute 资源类型
description: 传递优化最大缓存大小绝对类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 285c1830065d18669bd6d3d02d615400af27e231
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947188"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="63e8e-103">deliveryOptimizationMaxCacheSizeAbsolute 资源类型</span><span class="sxs-lookup"><span data-stu-id="63e8e-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="63e8e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63e8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63e8e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63e8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e8e-106">传递优化最大缓存大小绝对类型。</span><span class="sxs-lookup"><span data-stu-id="63e8e-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="63e8e-107">继承自[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="63e8e-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63e8e-108">属性</span><span class="sxs-lookup"><span data-stu-id="63e8e-108">Properties</span></span>
|<span data-ttu-id="63e8e-109">属性</span><span class="sxs-lookup"><span data-stu-id="63e8e-109">Property</span></span>|<span data-ttu-id="63e8e-110">类型</span><span class="sxs-lookup"><span data-stu-id="63e8e-110">Type</span></span>|<span data-ttu-id="63e8e-111">说明</span><span class="sxs-lookup"><span data-stu-id="63e8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e8e-112">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="63e8e-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="63e8e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="63e8e-113">Int64</span></span>|<span data-ttu-id="63e8e-114">指定传递优化缓存的最大大小 (以 GB 为单位)。</span><span class="sxs-lookup"><span data-stu-id="63e8e-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="63e8e-115">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="63e8e-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="63e8e-116">值为 0 (零) 表示 "无限制" 缓存。</span><span class="sxs-lookup"><span data-stu-id="63e8e-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="63e8e-117">当设备的磁盘空间不足时, 传递优化将清除缓存。</span><span class="sxs-lookup"><span data-stu-id="63e8e-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="63e8e-118">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="63e8e-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="63e8e-119">关系</span><span class="sxs-lookup"><span data-stu-id="63e8e-119">Relationships</span></span>
<span data-ttu-id="63e8e-120">无</span><span class="sxs-lookup"><span data-stu-id="63e8e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63e8e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63e8e-121">JSON Representation</span></span>
<span data-ttu-id="63e8e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63e8e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```




