---
title: deliveryOptimizationBandwidthHoursWithPercentage 资源类型
description: 以工作时间表示的百分比的带宽限制。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb4fa251e9f1cb936da0ada158050df42e0aab6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178239"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="8bd81-103">deliveryOptimizationBandwidthHoursWithPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bd81-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="8bd81-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8bd81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bd81-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8bd81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bd81-106">以工作时间表示的百分比的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="8bd81-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="8bd81-107">继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="8bd81-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8bd81-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bd81-108">Properties</span></span>
|<span data-ttu-id="8bd81-109">属性</span><span class="sxs-lookup"><span data-stu-id="8bd81-109">Property</span></span>|<span data-ttu-id="8bd81-110">类型</span><span class="sxs-lookup"><span data-stu-id="8bd81-110">Type</span></span>|<span data-ttu-id="8bd81-111">说明</span><span class="sxs-lookup"><span data-stu-id="8bd81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bd81-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="8bd81-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="8bd81-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="8bd81-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="8bd81-114">后台下载百分比小时数。</span><span class="sxs-lookup"><span data-stu-id="8bd81-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="8bd81-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="8bd81-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="8bd81-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="8bd81-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="8bd81-117">前台下载百分比小时。</span><span class="sxs-lookup"><span data-stu-id="8bd81-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bd81-118">关系</span><span class="sxs-lookup"><span data-stu-id="8bd81-118">Relationships</span></span>
<span data-ttu-id="8bd81-119">无</span><span class="sxs-lookup"><span data-stu-id="8bd81-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bd81-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bd81-120">JSON Representation</span></span>
<span data-ttu-id="8bd81-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bd81-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```




