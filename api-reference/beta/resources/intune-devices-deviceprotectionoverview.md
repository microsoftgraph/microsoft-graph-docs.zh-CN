---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f76918b5a959a6621fb7f5c6480a7a2513afead
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804310"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="77b3b-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="77b3b-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="77b3b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77b3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77b3b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77b3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77b3b-106">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="77b3b-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="77b3b-107">属性</span><span class="sxs-lookup"><span data-stu-id="77b3b-107">Properties</span></span>
|<span data-ttu-id="77b3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="77b3b-108">Property</span></span>|<span data-ttu-id="77b3b-109">类型</span><span class="sxs-lookup"><span data-stu-id="77b3b-109">Type</span></span>|<span data-ttu-id="77b3b-110">说明</span><span class="sxs-lookup"><span data-stu-id="77b3b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77b3b-111">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="77b3b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-112">Int32</span></span>|<span data-ttu-id="77b3b-113">设备计数总数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-113">Total device count.</span></span>|
|<span data-ttu-id="77b3b-114">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="77b3b-115">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-115">Int32</span></span>|<span data-ttu-id="77b3b-116">带有非活动威胁代理计数的设备</span><span class="sxs-lookup"><span data-stu-id="77b3b-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="77b3b-117">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="77b3b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-118">Int32</span></span>|<span data-ttu-id="77b3b-119">包含威胁代理状态的设备作为未知计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="77b3b-120">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="77b3b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-121">Int32</span></span>|<span data-ttu-id="77b3b-122">具有旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="77b3b-122">Device with old signature count.</span></span>|
|<span data-ttu-id="77b3b-123">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-123">cleanDeviceCount</span></span>|<span data-ttu-id="77b3b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-124">Int32</span></span>|<span data-ttu-id="77b3b-125">清洗设备计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-125">Clean device count.</span></span>|
|<span data-ttu-id="77b3b-126">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="77b3b-127">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-127">Int32</span></span>|<span data-ttu-id="77b3b-128">正在等待完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="77b3b-129">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="77b3b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-130">Int32</span></span>|<span data-ttu-id="77b3b-131">等待重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-131">Pending restart device count.</span></span>|
|<span data-ttu-id="77b3b-132">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="77b3b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-133">Int32</span></span>|<span data-ttu-id="77b3b-134">正在等待手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="77b3b-135">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="77b3b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-136">Int32</span></span>|<span data-ttu-id="77b3b-137">等待脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="77b3b-138">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="77b3b-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="77b3b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="77b3b-139">Int32</span></span>|<span data-ttu-id="77b3b-140">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="77b3b-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77b3b-141">关系</span><span class="sxs-lookup"><span data-stu-id="77b3b-141">Relationships</span></span>
<span data-ttu-id="77b3b-142">无</span><span class="sxs-lookup"><span data-stu-id="77b3b-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77b3b-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77b3b-143">JSON Representation</span></span>
<span data-ttu-id="77b3b-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77b3b-144">Here is a JSON representation of the resource.</span></span>
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
  "criticalFailuresDeviceCount": 1024
}
```





