---
title: deliveryOptimizationBandwidthHoursWithPercentage 资源类型
description: 以工作时间表示的百分比的带宽限制。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d51f975c083c4033c01caf7363f94288cb3ddad
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794380"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="0d776-103">deliveryOptimizationBandwidthHoursWithPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d776-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="0d776-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d776-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d776-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d776-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d776-106">以工作时间表示的百分比的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="0d776-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="0d776-107">继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="0d776-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d776-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d776-108">Properties</span></span>
|<span data-ttu-id="0d776-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d776-109">Property</span></span>|<span data-ttu-id="0d776-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d776-110">Type</span></span>|<span data-ttu-id="0d776-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d776-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d776-112">bandwidthBackgroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="0d776-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="0d776-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="0d776-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="0d776-114">后台下载百分比小时数。</span><span class="sxs-lookup"><span data-stu-id="0d776-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="0d776-115">bandwidthForegroundPercentageHours</span><span class="sxs-lookup"><span data-stu-id="0d776-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="0d776-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="0d776-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="0d776-117">前台下载百分比小时。</span><span class="sxs-lookup"><span data-stu-id="0d776-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d776-118">关系</span><span class="sxs-lookup"><span data-stu-id="0d776-118">Relationships</span></span>
<span data-ttu-id="0d776-119">无</span><span class="sxs-lookup"><span data-stu-id="0d776-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d776-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d776-120">JSON Representation</span></span>
<span data-ttu-id="0d776-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d776-121">Here is a JSON representation of the resource.</span></span>
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



