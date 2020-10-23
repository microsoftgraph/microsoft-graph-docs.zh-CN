---
title: deliveryOptimizationMaxCacheSizePercentage 资源类型
description: 传递优化最大缓存大小百分比类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02b522ccfac58a6c4ff9f9780512e83abf2cdec8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692546"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="3016a-103">deliveryOptimizationMaxCacheSizePercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="3016a-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

<span data-ttu-id="3016a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3016a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3016a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3016a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3016a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3016a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3016a-107">传递优化最大缓存大小百分比类型。</span><span class="sxs-lookup"><span data-stu-id="3016a-107">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="3016a-108">继承自 [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="3016a-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3016a-109">属性</span><span class="sxs-lookup"><span data-stu-id="3016a-109">Properties</span></span>
|<span data-ttu-id="3016a-110">属性</span><span class="sxs-lookup"><span data-stu-id="3016a-110">Property</span></span>|<span data-ttu-id="3016a-111">类型</span><span class="sxs-lookup"><span data-stu-id="3016a-111">Type</span></span>|<span data-ttu-id="3016a-112">说明</span><span class="sxs-lookup"><span data-stu-id="3016a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3016a-113">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="3016a-113">maximumCacheSizePercentage</span></span>|<span data-ttu-id="3016a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3016a-114">Int32</span></span>|<span data-ttu-id="3016a-115">指定传递优化可以使用的最大缓存大小，以磁盘大小的百分比 (1-100) 为依据。</span><span class="sxs-lookup"><span data-stu-id="3016a-115">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="3016a-116">有效值为1至100</span><span class="sxs-lookup"><span data-stu-id="3016a-116">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="3016a-117">关系</span><span class="sxs-lookup"><span data-stu-id="3016a-117">Relationships</span></span>
<span data-ttu-id="3016a-118">无</span><span class="sxs-lookup"><span data-stu-id="3016a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3016a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3016a-119">JSON Representation</span></span>
<span data-ttu-id="3016a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3016a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```





