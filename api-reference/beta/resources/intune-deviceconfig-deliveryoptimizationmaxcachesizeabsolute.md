---
title: deliveryOptimizationMaxCacheSizeAbsolute 资源类型
description: 传递优化最大缓存大小绝对类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a15b1bfea6da2af43c360ff143d8bb55bc44f6b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420455"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="818c1-103">deliveryOptimizationMaxCacheSizeAbsolute 资源类型</span><span class="sxs-lookup"><span data-stu-id="818c1-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="818c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="818c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="818c1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="818c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="818c1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="818c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="818c1-107">传递优化最大缓存大小绝对类型。</span><span class="sxs-lookup"><span data-stu-id="818c1-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="818c1-108">继承自[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="818c1-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="818c1-109">属性</span><span class="sxs-lookup"><span data-stu-id="818c1-109">Properties</span></span>
|<span data-ttu-id="818c1-110">属性</span><span class="sxs-lookup"><span data-stu-id="818c1-110">Property</span></span>|<span data-ttu-id="818c1-111">类型</span><span class="sxs-lookup"><span data-stu-id="818c1-111">Type</span></span>|<span data-ttu-id="818c1-112">说明</span><span class="sxs-lookup"><span data-stu-id="818c1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="818c1-113">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="818c1-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="818c1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="818c1-114">Int64</span></span>|<span data-ttu-id="818c1-115">指定传递优化缓存的最大大小（以 GB 为单位）。</span><span class="sxs-lookup"><span data-stu-id="818c1-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="818c1-116">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="818c1-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="818c1-117">值为0（零）表示 "无限制" 缓存。</span><span class="sxs-lookup"><span data-stu-id="818c1-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="818c1-118">当设备的磁盘空间不足时，传递优化将清除缓存。</span><span class="sxs-lookup"><span data-stu-id="818c1-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="818c1-119">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="818c1-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="818c1-120">关系</span><span class="sxs-lookup"><span data-stu-id="818c1-120">Relationships</span></span>
<span data-ttu-id="818c1-121">无</span><span class="sxs-lookup"><span data-stu-id="818c1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="818c1-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="818c1-122">JSON Representation</span></span>
<span data-ttu-id="818c1-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="818c1-123">Here is a JSON representation of the resource.</span></span>
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



