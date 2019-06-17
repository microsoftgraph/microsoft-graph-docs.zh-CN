---
title: deliveryOptimizationBandwidthAbsolute 资源类型
description: 带宽限制, 以千字节/秒为单位。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 626c46c035ec4a7af44c06a31f7269cde96a2b8b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979716"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="c97c1-103">deliveryOptimizationBandwidthAbsolute 资源类型</span><span class="sxs-lookup"><span data-stu-id="c97c1-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

> <span data-ttu-id="c97c1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c97c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c97c1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c97c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c97c1-106">带宽限制, 以千字节/秒为单位。</span><span class="sxs-lookup"><span data-stu-id="c97c1-106">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="c97c1-107">继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="c97c1-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c97c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="c97c1-108">Properties</span></span>
|<span data-ttu-id="c97c1-109">属性</span><span class="sxs-lookup"><span data-stu-id="c97c1-109">Property</span></span>|<span data-ttu-id="c97c1-110">类型</span><span class="sxs-lookup"><span data-stu-id="c97c1-110">Type</span></span>|<span data-ttu-id="c97c1-111">说明</span><span class="sxs-lookup"><span data-stu-id="c97c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97c1-112">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="c97c1-112">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="c97c1-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c97c1-113">Int64</span></span>|<span data-ttu-id="c97c1-114">指定设备可在使用传递优化的所有并发下载活动中使用的最大下载带宽 (以千字节/秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="c97c1-114">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="c97c1-115">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="c97c1-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="c97c1-116">值为 0 (零) 表示传递优化将动态调整, 以使用可用带宽进行下载。</span><span class="sxs-lookup"><span data-stu-id="c97c1-116">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="c97c1-117">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="c97c1-117">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="c97c1-118">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="c97c1-118">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="c97c1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c97c1-119">Int64</span></span>|<span data-ttu-id="c97c1-120">指定设备将使用传递优化 (0-4000000) 在所有并发上载活动中使用的最大上载带宽 (以千字节/秒为单位)。</span><span class="sxs-lookup"><span data-stu-id="c97c1-120">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="c97c1-121">有效值为0至4000000</span><span class="sxs-lookup"><span data-stu-id="c97c1-121">Valid values 0 to 4000000</span></span>
<span data-ttu-id="c97c1-122">默认值为 0, 它允许无限制的可能带宽 (针对最小上载带宽的使用情况进行了优化)。</span><span class="sxs-lookup"><span data-stu-id="c97c1-122">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="c97c1-123">有效值为0至4000000</span><span class="sxs-lookup"><span data-stu-id="c97c1-123">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="c97c1-124">关系</span><span class="sxs-lookup"><span data-stu-id="c97c1-124">Relationships</span></span>
<span data-ttu-id="c97c1-125">无</span><span class="sxs-lookup"><span data-stu-id="c97c1-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c97c1-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c97c1-126">JSON Representation</span></span>
<span data-ttu-id="c97c1-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c97c1-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```





