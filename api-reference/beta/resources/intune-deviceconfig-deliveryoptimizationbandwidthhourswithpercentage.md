---
title: deliveryOptimizationBandwidthHoursWithPercentage 资源类型
description: 以工作时间表示的百分比的带宽限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bac0cd6232983e506ea9fafd3167910ea0bcae7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078414"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="bf862-103">deliveryOptimizationBandwidthHoursWithPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf862-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="bf862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf862-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf862-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf862-107">以工作时间表示的百分比的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="bf862-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="bf862-108">继承自 [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="bf862-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf862-109">属性</span><span class="sxs-lookup"><span data-stu-id="bf862-109">Properties</span></span>
|<span data-ttu-id="bf862-110">属性</span><span class="sxs-lookup"><span data-stu-id="bf862-110">Property</span></span>|<span data-ttu-id="bf862-111">类型</span><span class="sxs-lookup"><span data-stu-id="bf862-111">Type</span></span>|<span data-ttu-id="bf862-112">说明</span><span class="sxs-lookup"><span data-stu-id="bf862-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf862-113">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="bf862-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="bf862-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="bf862-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="bf862-115">后台下载百分比小时数。</span><span class="sxs-lookup"><span data-stu-id="bf862-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="bf862-116">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="bf862-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="bf862-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="bf862-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="bf862-118">前台下载百分比小时。</span><span class="sxs-lookup"><span data-stu-id="bf862-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf862-119">关系</span><span class="sxs-lookup"><span data-stu-id="bf862-119">Relationships</span></span>
<span data-ttu-id="bf862-120">无</span><span class="sxs-lookup"><span data-stu-id="bf862-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf862-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf862-121">JSON Representation</span></span>
<span data-ttu-id="bf862-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf862-122">Here is a JSON representation of the resource.</span></span>
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






