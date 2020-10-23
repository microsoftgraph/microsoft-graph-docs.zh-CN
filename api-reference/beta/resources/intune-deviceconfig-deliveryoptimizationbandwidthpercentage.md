---
title: deliveryOptimizationBandwidthPercentage 资源类型
description: 以百分比形式指定的带宽限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3186e573b40cdaa4d56ace97a2ff985d7589db86
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696221"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="3ba3a-103">deliveryOptimizationBandwidthPercentage 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ba3a-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="3ba3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ba3a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ba3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ba3a-107">以百分比形式指定的带宽限制。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="3ba3a-108">继承自 [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="3ba3a-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ba3a-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ba3a-109">Properties</span></span>
|<span data-ttu-id="3ba3a-110">属性</span><span class="sxs-lookup"><span data-stu-id="3ba3a-110">Property</span></span>|<span data-ttu-id="3ba3a-111">类型</span><span class="sxs-lookup"><span data-stu-id="3ba3a-111">Type</span></span>|<span data-ttu-id="3ba3a-112">说明</span><span class="sxs-lookup"><span data-stu-id="3ba3a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ba3a-113">maximumBackgroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="3ba3a-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="3ba3a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3ba3a-114">Int32</span></span>|<span data-ttu-id="3ba3a-115">指定传递优化在所有并发下载活动中使用的最大后台下载带宽，以 (0-100) 的可用下载带宽的百分比表示。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="3ba3a-116">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="3ba3a-116">Valid values 0 to 100</span></span>
<span data-ttu-id="3ba3a-117">默认值 0 (零) 意味着传递优化将动态调整，以使用可用带宽进行后台下载。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="3ba3a-118">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="3ba3a-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3ba3a-119">maximumForegroundBandwidthPercentage</span><span class="sxs-lookup"><span data-stu-id="3ba3a-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="3ba3a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3ba3a-120">Int32</span></span>|<span data-ttu-id="3ba3a-121">指定传递优化在所有并发下载活动中使用的最大前台下载带宽，以可用下载带宽的百分比 (0-100) 为依据。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="3ba3a-122">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="3ba3a-122">Valid values 0 to 100</span></span>
<span data-ttu-id="3ba3a-123">默认值 0 (零) 意味着传递优化将动态调整，以使用可用带宽进行前台下载。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="3ba3a-124">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="3ba3a-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ba3a-125">关系</span><span class="sxs-lookup"><span data-stu-id="3ba3a-125">Relationships</span></span>
<span data-ttu-id="3ba3a-126">无</span><span class="sxs-lookup"><span data-stu-id="3ba3a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba3a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ba3a-127">JSON Representation</span></span>
<span data-ttu-id="3ba3a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ba3a-128">Here is a JSON representation of the resource.</span></span>
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





