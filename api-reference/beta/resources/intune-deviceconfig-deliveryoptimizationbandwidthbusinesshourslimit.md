---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4044b62a42c37abf030ff0a5d206093d4a2b8c80
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420586"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="44c38-103">deliveryOptimizationBandwidthBusinessHoursLimit 资源类型</span><span class="sxs-lookup"><span data-stu-id="44c38-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="44c38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44c38-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44c38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44c38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44c38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44c38-107">带宽业务时间和百分比类型</span><span class="sxs-lookup"><span data-stu-id="44c38-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="44c38-108">属性</span><span class="sxs-lookup"><span data-stu-id="44c38-108">Properties</span></span>
|<span data-ttu-id="44c38-109">属性</span><span class="sxs-lookup"><span data-stu-id="44c38-109">Property</span></span>|<span data-ttu-id="44c38-110">类型</span><span class="sxs-lookup"><span data-stu-id="44c38-110">Type</span></span>|<span data-ttu-id="44c38-111">说明</span><span class="sxs-lookup"><span data-stu-id="44c38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c38-112">bandwidthBeginBusinessHours</span><span class="sxs-lookup"><span data-stu-id="44c38-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="44c38-113">Int32</span><span class="sxs-lookup"><span data-stu-id="44c38-113">Int32</span></span>|<span data-ttu-id="44c38-114">指定使用24小时制的营业时间的开始时间（0-23）。</span><span class="sxs-lookup"><span data-stu-id="44c38-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="44c38-115">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="44c38-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="44c38-116">bandwidthEndBusinessHours</span><span class="sxs-lookup"><span data-stu-id="44c38-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="44c38-117">Int32</span><span class="sxs-lookup"><span data-stu-id="44c38-117">Int32</span></span>|<span data-ttu-id="44c38-118">指定使用24小时制的营业时间结束（0-23）。</span><span class="sxs-lookup"><span data-stu-id="44c38-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="44c38-119">有效值为0到23</span><span class="sxs-lookup"><span data-stu-id="44c38-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="44c38-120">bandwidthPercentageDuringBusinessHours</span><span class="sxs-lookup"><span data-stu-id="44c38-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="44c38-121">Int32</span><span class="sxs-lookup"><span data-stu-id="44c38-121">Int32</span></span>|<span data-ttu-id="44c38-122">指定在营业时间内要限制的带宽百分比（0-100）。</span><span class="sxs-lookup"><span data-stu-id="44c38-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="44c38-123">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="44c38-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="44c38-124">bandwidthPercentageOutsideBusinessHours</span><span class="sxs-lookup"><span data-stu-id="44c38-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="44c38-125">Int32</span><span class="sxs-lookup"><span data-stu-id="44c38-125">Int32</span></span>|<span data-ttu-id="44c38-126">指定要限制 outsidse 营业时间（0-100）的带宽百分比。</span><span class="sxs-lookup"><span data-stu-id="44c38-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="44c38-127">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="44c38-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="44c38-128">关系</span><span class="sxs-lookup"><span data-stu-id="44c38-128">Relationships</span></span>
<span data-ttu-id="44c38-129">无</span><span class="sxs-lookup"><span data-stu-id="44c38-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44c38-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44c38-130">JSON Representation</span></span>
<span data-ttu-id="44c38-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44c38-131">Here is a JSON representation of the resource.</span></span>
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



