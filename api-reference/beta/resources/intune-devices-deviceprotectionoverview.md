---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a815dbd43f8b47f872b51ecb3eee8791b622d505
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691363"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="8ae26-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ae26-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="8ae26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ae26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ae26-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ae26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ae26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ae26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae26-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="8ae26-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="8ae26-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ae26-108">Properties</span></span>
|<span data-ttu-id="8ae26-109">属性</span><span class="sxs-lookup"><span data-stu-id="8ae26-109">Property</span></span>|<span data-ttu-id="8ae26-110">类型</span><span class="sxs-lookup"><span data-stu-id="8ae26-110">Type</span></span>|<span data-ttu-id="8ae26-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ae26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae26-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="8ae26-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-113">Int32</span></span>|<span data-ttu-id="8ae26-114">设备计数总数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-114">Total device count.</span></span>|
|<span data-ttu-id="8ae26-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="8ae26-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-116">Int32</span></span>|<span data-ttu-id="8ae26-117">带有非活动威胁代理计数的设备</span><span class="sxs-lookup"><span data-stu-id="8ae26-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="8ae26-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="8ae26-119">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-119">Int32</span></span>|<span data-ttu-id="8ae26-120">包含威胁代理状态的设备作为未知计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="8ae26-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="8ae26-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-122">Int32</span></span>|<span data-ttu-id="8ae26-123">具有旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="8ae26-123">Device with old signature count.</span></span>|
|<span data-ttu-id="8ae26-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-124">cleanDeviceCount</span></span>|<span data-ttu-id="8ae26-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-125">Int32</span></span>|<span data-ttu-id="8ae26-126">清洗设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-126">Clean device count.</span></span>|
|<span data-ttu-id="8ae26-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="8ae26-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-128">Int32</span></span>|<span data-ttu-id="8ae26-129">正在等待完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="8ae26-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="8ae26-131">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-131">Int32</span></span>|<span data-ttu-id="8ae26-132">等待重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-132">Pending restart device count.</span></span>|
|<span data-ttu-id="8ae26-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="8ae26-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-134">Int32</span></span>|<span data-ttu-id="8ae26-135">正在等待手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="8ae26-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="8ae26-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-137">Int32</span></span>|<span data-ttu-id="8ae26-138">等待脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="8ae26-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="8ae26-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-140">Int32</span></span>|<span data-ttu-id="8ae26-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-141">Critical failures device count.</span></span>|
|<span data-ttu-id="8ae26-142">pendingQuickScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ae26-142">pendingQuickScanDeviceCount</span></span>|<span data-ttu-id="8ae26-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae26-143">Int32</span></span>|<span data-ttu-id="8ae26-144">等待快速扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="8ae26-144">Pending quick scan device count.</span></span> <span data-ttu-id="8ae26-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="8ae26-145">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ae26-146">关系</span><span class="sxs-lookup"><span data-stu-id="8ae26-146">Relationships</span></span>
<span data-ttu-id="8ae26-147">无</span><span class="sxs-lookup"><span data-stu-id="8ae26-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ae26-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ae26-148">JSON Representation</span></span>
<span data-ttu-id="8ae26-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ae26-149">Here is a JSON representation of the resource.</span></span>
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





