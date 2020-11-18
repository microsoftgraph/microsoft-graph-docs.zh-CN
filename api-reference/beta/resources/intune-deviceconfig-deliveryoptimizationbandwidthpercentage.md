---
title: deliveryOptimizationBandwidthPercentage 资源类型
description: 以百分比形式指定的带宽限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85dc858431b15a142a42afc74b1b7c1ba76a4667
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199607"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="adacf-103">deliveryOptimizationBandwidthPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="adacf-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="adacf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adacf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adacf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="adacf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adacf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="adacf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adacf-107">以百分比形式指定的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="adacf-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="adacf-108">继承自 [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="adacf-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="adacf-109">属性</span><span class="sxs-lookup"><span data-stu-id="adacf-109">Properties</span></span>
|<span data-ttu-id="adacf-110">属性</span><span class="sxs-lookup"><span data-stu-id="adacf-110">Property</span></span>|<span data-ttu-id="adacf-111">类型</span><span class="sxs-lookup"><span data-stu-id="adacf-111">Type</span></span>|<span data-ttu-id="adacf-112">说明</span><span class="sxs-lookup"><span data-stu-id="adacf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adacf-113">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="adacf-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="adacf-114">Int32</span><span class="sxs-lookup"><span data-stu-id="adacf-114">Int32</span></span>|<span data-ttu-id="adacf-115">指定传递优化在所有并发下载活动中使用的最大后台下载带宽，以 (0-100) 的可用下载带宽的百分比表示。</span><span class="sxs-lookup"><span data-stu-id="adacf-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="adacf-116">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="adacf-116">Valid values 0 to 100</span></span>
<span data-ttu-id="adacf-117">默认值 0 (零) 意味着传递优化将动态调整，以使用可用带宽进行后台下载。</span><span class="sxs-lookup"><span data-stu-id="adacf-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="adacf-118">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="adacf-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="adacf-119">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="adacf-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="adacf-120">Int32</span><span class="sxs-lookup"><span data-stu-id="adacf-120">Int32</span></span>|<span data-ttu-id="adacf-121">指定传递优化在所有并发下载活动中使用的最大前台下载带宽，以可用下载带宽的百分比 (0-100) 为依据。</span><span class="sxs-lookup"><span data-stu-id="adacf-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="adacf-122">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="adacf-122">Valid values 0 to 100</span></span>
<span data-ttu-id="adacf-123">默认值 0 (零) 意味着传递优化将动态调整，以使用可用带宽进行前台下载。</span><span class="sxs-lookup"><span data-stu-id="adacf-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="adacf-124">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="adacf-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="adacf-125">关系</span><span class="sxs-lookup"><span data-stu-id="adacf-125">Relationships</span></span>
<span data-ttu-id="adacf-126">无</span><span class="sxs-lookup"><span data-stu-id="adacf-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="adacf-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adacf-127">JSON Representation</span></span>
<span data-ttu-id="adacf-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adacf-128">Here is a JSON representation of the resource.</span></span>
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




