---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 533d4c0706f319f4b127f78af8340f215232e2b9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333385"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="cd827-103">deliveryOptimizationBandwidthBusinessHoursLimit 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd827-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="cd827-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd827-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd827-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd827-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd827-106">带宽业务时间和百分比类型</span><span class="sxs-lookup"><span data-stu-id="cd827-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="cd827-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd827-107">Properties</span></span>
|<span data-ttu-id="cd827-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd827-108">Property</span></span>|<span data-ttu-id="cd827-109">类型</span><span class="sxs-lookup"><span data-stu-id="cd827-109">Type</span></span>|<span data-ttu-id="cd827-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd827-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd827-111">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="cd827-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="cd827-112">Int32</span><span class="sxs-lookup"><span data-stu-id="cd827-112">Int32</span></span>|<span data-ttu-id="cd827-113">指定使用24小时制的营业时间的开始时间 (0-23)。</span><span class="sxs-lookup"><span data-stu-id="cd827-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="cd827-114">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="cd827-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="cd827-115">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="cd827-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="cd827-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cd827-116">Int32</span></span>|<span data-ttu-id="cd827-117">指定使用24小时制的营业时间结束 (0-23)。</span><span class="sxs-lookup"><span data-stu-id="cd827-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="cd827-118">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="cd827-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="cd827-119">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="cd827-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="cd827-120">Int32</span><span class="sxs-lookup"><span data-stu-id="cd827-120">Int32</span></span>|<span data-ttu-id="cd827-121">指定在营业时间内要限制的带宽百分比 (0-100)。</span><span class="sxs-lookup"><span data-stu-id="cd827-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="cd827-122">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="cd827-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="cd827-123">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="cd827-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="cd827-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cd827-124">Int32</span></span>|<span data-ttu-id="cd827-125">指定要限制 outsidse 营业时间 (0-100) 的带宽百分比。</span><span class="sxs-lookup"><span data-stu-id="cd827-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="cd827-126">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="cd827-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd827-127">关系</span><span class="sxs-lookup"><span data-stu-id="cd827-127">Relationships</span></span>
<span data-ttu-id="cd827-128">无</span><span class="sxs-lookup"><span data-stu-id="cd827-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd827-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd827-129">JSON Representation</span></span>
<span data-ttu-id="cd827-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd827-130">Here is a JSON representation of the resource.</span></span>
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



