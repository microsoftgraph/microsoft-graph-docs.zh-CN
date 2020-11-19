---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a21a81ebc18616b9d072ba9bba39ec4a1e1ee7db
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231645"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="28a26-103">deliveryOptimizationBandwidthBusinessHoursLimit 资源类型</span><span class="sxs-lookup"><span data-stu-id="28a26-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="28a26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28a26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28a26-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28a26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28a26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28a26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a26-107">带宽业务时间和百分比类型</span><span class="sxs-lookup"><span data-stu-id="28a26-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="28a26-108">属性</span><span class="sxs-lookup"><span data-stu-id="28a26-108">Properties</span></span>
|<span data-ttu-id="28a26-109">属性</span><span class="sxs-lookup"><span data-stu-id="28a26-109">Property</span></span>|<span data-ttu-id="28a26-110">类型</span><span class="sxs-lookup"><span data-stu-id="28a26-110">Type</span></span>|<span data-ttu-id="28a26-111">说明</span><span class="sxs-lookup"><span data-stu-id="28a26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a26-112">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="28a26-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="28a26-113">Int32</span><span class="sxs-lookup"><span data-stu-id="28a26-113">Int32</span></span>|<span data-ttu-id="28a26-114">使用24小时制 (0-23) 指定营业时间的开始时间。</span><span class="sxs-lookup"><span data-stu-id="28a26-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="28a26-115">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="28a26-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="28a26-116">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="28a26-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="28a26-117">Int32</span><span class="sxs-lookup"><span data-stu-id="28a26-117">Int32</span></span>|<span data-ttu-id="28a26-118">使用24小时制 (0-23) 指定营业时间的结束时间。</span><span class="sxs-lookup"><span data-stu-id="28a26-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="28a26-119">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="28a26-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="28a26-120">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="28a26-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="28a26-121">Int32</span><span class="sxs-lookup"><span data-stu-id="28a26-121">Int32</span></span>|<span data-ttu-id="28a26-122">指定在营业时间 (0-100) 时要限制的带宽百分比。</span><span class="sxs-lookup"><span data-stu-id="28a26-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="28a26-123">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="28a26-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="28a26-124">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="28a26-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="28a26-125">Int32</span><span class="sxs-lookup"><span data-stu-id="28a26-125">Int32</span></span>|<span data-ttu-id="28a26-126">指定要限制 outsidse 营业时间 (0-100) 的带宽百分比。</span><span class="sxs-lookup"><span data-stu-id="28a26-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="28a26-127">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="28a26-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="28a26-128">关系</span><span class="sxs-lookup"><span data-stu-id="28a26-128">Relationships</span></span>
<span data-ttu-id="28a26-129">无</span><span class="sxs-lookup"><span data-stu-id="28a26-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28a26-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28a26-130">JSON Representation</span></span>
<span data-ttu-id="28a26-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28a26-131">Here is a JSON representation of the resource.</span></span>
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




