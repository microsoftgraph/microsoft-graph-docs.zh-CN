---
title: deliveryOptimizationMaxCacheSizeAbsolute 资源类型
description: 传递优化最大缓存大小绝对类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dfb158b30c8c2d75a58ddcbab190eaa37e9153bd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294716"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="1f450-103">deliveryOptimizationMaxCacheSizeAbsolute 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f450-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="1f450-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f450-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f450-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f450-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f450-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f450-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f450-107">传递优化最大缓存大小绝对类型。</span><span class="sxs-lookup"><span data-stu-id="1f450-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="1f450-108">继承自 [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="1f450-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f450-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f450-109">Properties</span></span>
|<span data-ttu-id="1f450-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f450-110">Property</span></span>|<span data-ttu-id="1f450-111">类型</span><span class="sxs-lookup"><span data-stu-id="1f450-111">Type</span></span>|<span data-ttu-id="1f450-112">Description</span><span class="sxs-lookup"><span data-stu-id="1f450-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f450-113">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="1f450-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="1f450-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1f450-114">Int64</span></span>|<span data-ttu-id="1f450-115">指定传递优化缓存的最大大小（以 GB 为单位）。</span><span class="sxs-lookup"><span data-stu-id="1f450-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="1f450-116">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="1f450-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="1f450-117">值 0 (零) 表示 "无限制" 缓存。</span><span class="sxs-lookup"><span data-stu-id="1f450-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="1f450-118">当设备的磁盘空间不足时，传递优化将清除缓存。</span><span class="sxs-lookup"><span data-stu-id="1f450-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="1f450-119">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="1f450-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f450-120">关系</span><span class="sxs-lookup"><span data-stu-id="1f450-120">Relationships</span></span>
<span data-ttu-id="1f450-121">无</span><span class="sxs-lookup"><span data-stu-id="1f450-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f450-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f450-122">JSON Representation</span></span>
<span data-ttu-id="1f450-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f450-123">Here is a JSON representation of the resource.</span></span>
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




