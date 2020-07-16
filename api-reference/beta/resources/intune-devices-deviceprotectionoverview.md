---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f6d4c325d11ee5f02277ad86f7bb038a2ac3b0f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123720"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="02480-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="02480-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="02480-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02480-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02480-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02480-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02480-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02480-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02480-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="02480-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="02480-108">属性</span><span class="sxs-lookup"><span data-stu-id="02480-108">Properties</span></span>
|<span data-ttu-id="02480-109">属性</span><span class="sxs-lookup"><span data-stu-id="02480-109">Property</span></span>|<span data-ttu-id="02480-110">类型</span><span class="sxs-lookup"><span data-stu-id="02480-110">Type</span></span>|<span data-ttu-id="02480-111">说明</span><span class="sxs-lookup"><span data-stu-id="02480-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02480-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="02480-113">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-113">Int32</span></span>|<span data-ttu-id="02480-114">设备计数总数。</span><span class="sxs-lookup"><span data-stu-id="02480-114">Total device count.</span></span>|
|<span data-ttu-id="02480-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="02480-116">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-116">Int32</span></span>|<span data-ttu-id="02480-117">带有非活动威胁代理计数的设备</span><span class="sxs-lookup"><span data-stu-id="02480-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="02480-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="02480-119">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-119">Int32</span></span>|<span data-ttu-id="02480-120">包含威胁代理状态的设备作为未知计数。</span><span class="sxs-lookup"><span data-stu-id="02480-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="02480-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="02480-122">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-122">Int32</span></span>|<span data-ttu-id="02480-123">具有旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="02480-123">Device with old signature count.</span></span>|
|<span data-ttu-id="02480-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-124">cleanDeviceCount</span></span>|<span data-ttu-id="02480-125">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-125">Int32</span></span>|<span data-ttu-id="02480-126">清洗设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-126">Clean device count.</span></span>|
|<span data-ttu-id="02480-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="02480-128">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-128">Int32</span></span>|<span data-ttu-id="02480-129">正在等待完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="02480-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="02480-131">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-131">Int32</span></span>|<span data-ttu-id="02480-132">等待重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-132">Pending restart device count.</span></span>|
|<span data-ttu-id="02480-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="02480-134">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-134">Int32</span></span>|<span data-ttu-id="02480-135">正在等待手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="02480-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="02480-137">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-137">Int32</span></span>|<span data-ttu-id="02480-138">等待脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="02480-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="02480-140">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-140">Int32</span></span>|<span data-ttu-id="02480-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-141">Critical failures device count.</span></span>|
|<span data-ttu-id="02480-142">pendingQuickScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02480-142">pendingQuickScanDeviceCount</span></span>|<span data-ttu-id="02480-143">Int32</span><span class="sxs-lookup"><span data-stu-id="02480-143">Int32</span></span>|<span data-ttu-id="02480-144">等待快速扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="02480-144">Pending quick scan device count.</span></span> <span data-ttu-id="02480-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="02480-145">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="02480-146">关系</span><span class="sxs-lookup"><span data-stu-id="02480-146">Relationships</span></span>
<span data-ttu-id="02480-147">无</span><span class="sxs-lookup"><span data-stu-id="02480-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02480-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02480-148">JSON Representation</span></span>
<span data-ttu-id="02480-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02480-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```



