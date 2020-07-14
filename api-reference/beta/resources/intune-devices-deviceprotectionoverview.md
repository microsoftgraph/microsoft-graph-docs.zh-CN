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
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="1efb6-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="1efb6-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="1efb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1efb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1efb6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1efb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1efb6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1efb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1efb6-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="1efb6-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="1efb6-108">属性</span><span class="sxs-lookup"><span data-stu-id="1efb6-108">Properties</span></span>
|<span data-ttu-id="1efb6-109">属性</span><span class="sxs-lookup"><span data-stu-id="1efb6-109">Property</span></span>|<span data-ttu-id="1efb6-110">类型</span><span class="sxs-lookup"><span data-stu-id="1efb6-110">Type</span></span>|<span data-ttu-id="1efb6-111">说明</span><span class="sxs-lookup"><span data-stu-id="1efb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efb6-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="1efb6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-113">Int32</span></span>|<span data-ttu-id="1efb6-114">设备计数总数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-114">Total device count.</span></span>|
|<span data-ttu-id="1efb6-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="1efb6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-116">Int32</span></span>|<span data-ttu-id="1efb6-117">带有非活动威胁代理计数的设备</span><span class="sxs-lookup"><span data-stu-id="1efb6-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="1efb6-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="1efb6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-119">Int32</span></span>|<span data-ttu-id="1efb6-120">包含威胁代理状态的设备作为未知计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="1efb6-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="1efb6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-122">Int32</span></span>|<span data-ttu-id="1efb6-123">具有旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="1efb6-123">Device with old signature count.</span></span>|
|<span data-ttu-id="1efb6-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-124">cleanDeviceCount</span></span>|<span data-ttu-id="1efb6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-125">Int32</span></span>|<span data-ttu-id="1efb6-126">清洗设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-126">Clean device count.</span></span>|
|<span data-ttu-id="1efb6-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="1efb6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-128">Int32</span></span>|<span data-ttu-id="1efb6-129">正在等待完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="1efb6-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="1efb6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-131">Int32</span></span>|<span data-ttu-id="1efb6-132">等待重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-132">Pending restart device count.</span></span>|
|<span data-ttu-id="1efb6-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="1efb6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-134">Int32</span></span>|<span data-ttu-id="1efb6-135">正在等待手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="1efb6-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="1efb6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-137">Int32</span></span>|<span data-ttu-id="1efb6-138">等待脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="1efb6-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="1efb6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-140">Int32</span></span>|<span data-ttu-id="1efb6-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-141">Critical failures device count.</span></span>|
|<span data-ttu-id="1efb6-142">pendingQuickScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1efb6-142">pendingQuickScanDeviceCount</span></span>|<span data-ttu-id="1efb6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1efb6-143">Int32</span></span>|<span data-ttu-id="1efb6-144">等待快速扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="1efb6-144">Pending quick scan device count.</span></span> <span data-ttu-id="1efb6-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="1efb6-145">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="1efb6-146">关系</span><span class="sxs-lookup"><span data-stu-id="1efb6-146">Relationships</span></span>
<span data-ttu-id="1efb6-147">无</span><span class="sxs-lookup"><span data-stu-id="1efb6-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1efb6-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1efb6-148">JSON Representation</span></span>
<span data-ttu-id="1efb6-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1efb6-149">Here is a JSON representation of the resource.</span></span>
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



