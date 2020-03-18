---
title: deliveryOptimizationBandwidthPercentage 资源类型
description: 以百分比形式指定的带宽限制。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34e3a76bf7b7ef70f880d4de8c432f84d7eb3509
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794373"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="94785-103">deliveryOptimizationBandwidthPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="94785-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="94785-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94785-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94785-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94785-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94785-106">以百分比形式指定的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="94785-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="94785-107">继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="94785-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94785-108">属性</span><span class="sxs-lookup"><span data-stu-id="94785-108">Properties</span></span>
|<span data-ttu-id="94785-109">属性</span><span class="sxs-lookup"><span data-stu-id="94785-109">Property</span></span>|<span data-ttu-id="94785-110">类型</span><span class="sxs-lookup"><span data-stu-id="94785-110">Type</span></span>|<span data-ttu-id="94785-111">说明</span><span class="sxs-lookup"><span data-stu-id="94785-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94785-112">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="94785-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="94785-113">Int32</span><span class="sxs-lookup"><span data-stu-id="94785-113">Int32</span></span>|<span data-ttu-id="94785-114">指定传递优化在所有并发下载活动中使用的最大后台下载带宽，以可用下载带宽的百分比（0-100）为依据。</span><span class="sxs-lookup"><span data-stu-id="94785-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="94785-115">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="94785-115">Valid values 0 to 100</span></span>
<span data-ttu-id="94785-116">默认值为0（零）意味着传递优化将动态调整，以使用可用带宽进行后台下载。</span><span class="sxs-lookup"><span data-stu-id="94785-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="94785-117">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="94785-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="94785-118">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="94785-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="94785-119">Int32</span><span class="sxs-lookup"><span data-stu-id="94785-119">Int32</span></span>|<span data-ttu-id="94785-120">指定传递优化在所有并发下载活动中使用的最大前台下载带宽，以可用下载带宽的百分比（0-100）为依据。</span><span class="sxs-lookup"><span data-stu-id="94785-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="94785-121">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="94785-121">Valid values 0 to 100</span></span>
<span data-ttu-id="94785-122">默认值为0（零）意味着传递优化将动态调整，以使用可用带宽进行前台下载。</span><span class="sxs-lookup"><span data-stu-id="94785-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="94785-123">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="94785-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="94785-124">关系</span><span class="sxs-lookup"><span data-stu-id="94785-124">Relationships</span></span>
<span data-ttu-id="94785-125">无</span><span class="sxs-lookup"><span data-stu-id="94785-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94785-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94785-126">JSON Representation</span></span>
<span data-ttu-id="94785-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94785-127">Here is a JSON representation of the resource.</span></span>
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



