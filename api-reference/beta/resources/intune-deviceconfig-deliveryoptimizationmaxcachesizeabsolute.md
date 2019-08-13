---
title: deliveryOptimizationMaxCacheSizeAbsolute 资源类型
description: 传递优化最大缓存大小绝对类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 096dbdd27d31e51849b8e8f53967e08a8029f756
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333284"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="f3b68-103">deliveryOptimizationMaxCacheSizeAbsolute 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3b68-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="f3b68-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3b68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3b68-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3b68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3b68-106">传递优化最大缓存大小绝对类型。</span><span class="sxs-lookup"><span data-stu-id="f3b68-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="f3b68-107">继承自[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="f3b68-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3b68-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3b68-108">Properties</span></span>
|<span data-ttu-id="f3b68-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3b68-109">Property</span></span>|<span data-ttu-id="f3b68-110">类型</span><span class="sxs-lookup"><span data-stu-id="f3b68-110">Type</span></span>|<span data-ttu-id="f3b68-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3b68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b68-112">maximumCacheSizeInGigabytes</span><span class="sxs-lookup"><span data-stu-id="f3b68-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="f3b68-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f3b68-113">Int64</span></span>|<span data-ttu-id="f3b68-114">指定传递优化缓存的最大大小 (以 GB 为单位)。</span><span class="sxs-lookup"><span data-stu-id="f3b68-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="f3b68-115">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="f3b68-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="f3b68-116">值为 0 (零) 表示 "无限制" 缓存。</span><span class="sxs-lookup"><span data-stu-id="f3b68-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="f3b68-117">当设备的磁盘空间不足时, 传递优化将清除缓存。</span><span class="sxs-lookup"><span data-stu-id="f3b68-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="f3b68-118">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="f3b68-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3b68-119">关系</span><span class="sxs-lookup"><span data-stu-id="f3b68-119">Relationships</span></span>
<span data-ttu-id="f3b68-120">无</span><span class="sxs-lookup"><span data-stu-id="f3b68-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3b68-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3b68-121">JSON Representation</span></span>
<span data-ttu-id="f3b68-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3b68-122">Here is a JSON representation of the resource.</span></span>
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



