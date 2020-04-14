---
title: deliveryOptimizationBandwidthAbsolute 资源类型
description: 带宽限制，以千字节/秒为单位。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34199703021805779fef292e906195fbb0f306cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420761"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a><span data-ttu-id="26d0e-103">deliveryOptimizationBandwidthAbsolute 资源类型</span><span class="sxs-lookup"><span data-stu-id="26d0e-103">deliveryOptimizationBandwidthAbsolute resource type</span></span>

<span data-ttu-id="26d0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26d0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26d0e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26d0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26d0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26d0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26d0e-107">带宽限制，以千字节/秒为单位。</span><span class="sxs-lookup"><span data-stu-id="26d0e-107">Bandwidth limits in kilobytes per second.</span></span>


<span data-ttu-id="26d0e-108">继承自[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="26d0e-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26d0e-109">属性</span><span class="sxs-lookup"><span data-stu-id="26d0e-109">Properties</span></span>
|<span data-ttu-id="26d0e-110">属性</span><span class="sxs-lookup"><span data-stu-id="26d0e-110">Property</span></span>|<span data-ttu-id="26d0e-111">类型</span><span class="sxs-lookup"><span data-stu-id="26d0e-111">Type</span></span>|<span data-ttu-id="26d0e-112">说明</span><span class="sxs-lookup"><span data-stu-id="26d0e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26d0e-113">maximumDownloadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="26d0e-113">maximumDownloadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="26d0e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="26d0e-114">Int64</span></span>|<span data-ttu-id="26d0e-115">指定设备可在使用传递优化的所有并发下载活动中使用的最大下载带宽（以千字节/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="26d0e-115">Specifies the maximum download bandwidth in KiloBytes/second that the device can use across all concurrent download activities using Delivery Optimization.</span></span> <span data-ttu-id="26d0e-116">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="26d0e-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="26d0e-117">值为0（零）表示传递优化将动态调整，以使用可用带宽进行下载。</span><span class="sxs-lookup"><span data-stu-id="26d0e-117">The value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for downloads.</span></span> <span data-ttu-id="26d0e-118">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="26d0e-118">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="26d0e-119">maximumUploadBandwidthInKilobytesPerSecond</span><span class="sxs-lookup"><span data-stu-id="26d0e-119">maximumUploadBandwidthInKilobytesPerSecond</span></span>|<span data-ttu-id="26d0e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="26d0e-120">Int64</span></span>|<span data-ttu-id="26d0e-121">指定设备将使用传递优化（0-4000000）在所有并发上载活动中使用的最大上载带宽（以千字节/秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="26d0e-121">Specifies the maximum upload bandwidth in KiloBytes/second that a device will use across all concurrent upload activity using Delivery Optimization (0-4000000).</span></span> <span data-ttu-id="26d0e-122">有效值为0至4000000</span><span class="sxs-lookup"><span data-stu-id="26d0e-122">Valid values 0 to 4000000</span></span>
<span data-ttu-id="26d0e-123">默认值为0，它允许无限制的可能带宽（针对最小上载带宽的使用情况进行了优化）。</span><span class="sxs-lookup"><span data-stu-id="26d0e-123">The default value is 0, which permits unlimited possible bandwidth (optimized for minimal usage of upload bandwidth).</span></span> <span data-ttu-id="26d0e-124">有效值为0至4000000</span><span class="sxs-lookup"><span data-stu-id="26d0e-124">Valid values 0 to 4000000</span></span>|

## <a name="relationships"></a><span data-ttu-id="26d0e-125">关系</span><span class="sxs-lookup"><span data-stu-id="26d0e-125">Relationships</span></span>
<span data-ttu-id="26d0e-126">无</span><span class="sxs-lookup"><span data-stu-id="26d0e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26d0e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26d0e-127">JSON Representation</span></span>
<span data-ttu-id="26d0e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26d0e-128">Here is a JSON representation of the resource.</span></span>
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



