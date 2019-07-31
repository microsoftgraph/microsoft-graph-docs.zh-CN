---
title: deliveryOptimizationMaxCacheSizePercentage 资源类型
description: 传递优化最大缓存大小百分比类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: adc27f85a4b02adbf5a8a589fd2bd07db0622978
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970722"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="0f5df-103">deliveryOptimizationMaxCacheSizePercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f5df-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

> <span data-ttu-id="0f5df-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f5df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f5df-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f5df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f5df-106">传递优化最大缓存大小百分比类型。</span><span class="sxs-lookup"><span data-stu-id="0f5df-106">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="0f5df-107">继承自[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="0f5df-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f5df-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f5df-108">Properties</span></span>
|<span data-ttu-id="0f5df-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f5df-109">Property</span></span>|<span data-ttu-id="0f5df-110">类型</span><span class="sxs-lookup"><span data-stu-id="0f5df-110">Type</span></span>|<span data-ttu-id="0f5df-111">说明</span><span class="sxs-lookup"><span data-stu-id="0f5df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f5df-112">maximumCacheSizePercentage</span><span class="sxs-lookup"><span data-stu-id="0f5df-112">maximumCacheSizePercentage</span></span>|<span data-ttu-id="0f5df-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5df-113">Int32</span></span>|<span data-ttu-id="0f5df-114">指定传递优化可以使用的最大缓存大小, 以占磁盘大小的百分比 (1-100)。</span><span class="sxs-lookup"><span data-stu-id="0f5df-114">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="0f5df-115">有效值为1至100</span><span class="sxs-lookup"><span data-stu-id="0f5df-115">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f5df-116">关系</span><span class="sxs-lookup"><span data-stu-id="0f5df-116">Relationships</span></span>
<span data-ttu-id="0f5df-117">无</span><span class="sxs-lookup"><span data-stu-id="0f5df-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f5df-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f5df-118">JSON Representation</span></span>
<span data-ttu-id="0f5df-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f5df-119">Here is a JSON representation of the resource.</span></span>
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





