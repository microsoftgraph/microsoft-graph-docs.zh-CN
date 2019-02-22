---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba15df46075e5cbea1a2eab8a798c333f4a60ae6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178113"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="18f0d-103">deliveryOptimizationBandwidthBusinessHoursLimit 资源类型</span><span class="sxs-lookup"><span data-stu-id="18f0d-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="18f0d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18f0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18f0d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18f0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18f0d-106">带宽业务时间和百分比类型</span><span class="sxs-lookup"><span data-stu-id="18f0d-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="18f0d-107">属性</span><span class="sxs-lookup"><span data-stu-id="18f0d-107">Properties</span></span>
|<span data-ttu-id="18f0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="18f0d-108">Property</span></span>|<span data-ttu-id="18f0d-109">类型</span><span class="sxs-lookup"><span data-stu-id="18f0d-109">Type</span></span>|<span data-ttu-id="18f0d-110">说明</span><span class="sxs-lookup"><span data-stu-id="18f0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18f0d-111">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0d-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="18f0d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0d-112">Int32</span></span>|<span data-ttu-id="18f0d-113">指定使用24小时制的营业时间的开始时间 (0-23)。</span><span class="sxs-lookup"><span data-stu-id="18f0d-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="18f0d-114">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="18f0d-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="18f0d-115">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0d-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="18f0d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0d-116">Int32</span></span>|<span data-ttu-id="18f0d-117">指定使用24小时制的营业时间结束 (0-23)。</span><span class="sxs-lookup"><span data-stu-id="18f0d-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="18f0d-118">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="18f0d-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="18f0d-119">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0d-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="18f0d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0d-120">Int32</span></span>|<span data-ttu-id="18f0d-121">指定在营业时间内要限制的带宽百分比 (0-100)。</span><span class="sxs-lookup"><span data-stu-id="18f0d-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="18f0d-122">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="18f0d-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="18f0d-123">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="18f0d-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="18f0d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="18f0d-124">Int32</span></span>|<span data-ttu-id="18f0d-125">指定要限制 outsidse 营业时间 (0-100) 的带宽百分比。</span><span class="sxs-lookup"><span data-stu-id="18f0d-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="18f0d-126">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="18f0d-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="18f0d-127">关系</span><span class="sxs-lookup"><span data-stu-id="18f0d-127">Relationships</span></span>
<span data-ttu-id="18f0d-128">无</span><span class="sxs-lookup"><span data-stu-id="18f0d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18f0d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18f0d-129">JSON Representation</span></span>
<span data-ttu-id="18f0d-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18f0d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```




