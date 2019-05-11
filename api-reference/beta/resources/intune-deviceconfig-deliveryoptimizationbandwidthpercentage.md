---
title: deliveryOptimizationBandwidthPercentage 资源类型
description: 以百分比形式指定的带宽限制。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bae3771f6c0d8d13edda7bed3d7968da48e042db
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947279"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="84bba-103">deliveryOptimizationBandwidthPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="84bba-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="84bba-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84bba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84bba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84bba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84bba-106">以百分比形式指定的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="84bba-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="84bba-107">继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="84bba-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84bba-108">属性</span><span class="sxs-lookup"><span data-stu-id="84bba-108">Properties</span></span>
|<span data-ttu-id="84bba-109">属性</span><span class="sxs-lookup"><span data-stu-id="84bba-109">Property</span></span>|<span data-ttu-id="84bba-110">类型</span><span class="sxs-lookup"><span data-stu-id="84bba-110">Type</span></span>|<span data-ttu-id="84bba-111">说明</span><span class="sxs-lookup"><span data-stu-id="84bba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84bba-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="84bba-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="84bba-113">Int32</span><span class="sxs-lookup"><span data-stu-id="84bba-113">Int32</span></span>|<span data-ttu-id="84bba-114">指定传递优化在所有并发下载活动中使用的最大后台下载带宽, 以可用下载带宽的百分比 (0-100) 为依据。</span><span class="sxs-lookup"><span data-stu-id="84bba-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="84bba-115">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="84bba-115">Valid values 0 to 100</span></span>
<span data-ttu-id="84bba-116">默认值为 0 (零) 意味着传递优化将动态调整, 以使用可用带宽进行后台下载。</span><span class="sxs-lookup"><span data-stu-id="84bba-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="84bba-117">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="84bba-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="84bba-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="84bba-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="84bba-119">Int32</span><span class="sxs-lookup"><span data-stu-id="84bba-119">Int32</span></span>|<span data-ttu-id="84bba-120">指定传递优化在所有并发下载活动中使用的最大前台下载带宽, 以可用下载带宽的百分比 (0-100) 为依据。</span><span class="sxs-lookup"><span data-stu-id="84bba-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="84bba-121">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="84bba-121">Valid values 0 to 100</span></span>
<span data-ttu-id="84bba-122">默认值为 0 (零) 意味着传递优化将动态调整, 以使用可用带宽进行前台下载。</span><span class="sxs-lookup"><span data-stu-id="84bba-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="84bba-123">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="84bba-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="84bba-124">关系</span><span class="sxs-lookup"><span data-stu-id="84bba-124">Relationships</span></span>
<span data-ttu-id="84bba-125">无</span><span class="sxs-lookup"><span data-stu-id="84bba-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84bba-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84bba-126">JSON Representation</span></span>
<span data-ttu-id="84bba-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84bba-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```




