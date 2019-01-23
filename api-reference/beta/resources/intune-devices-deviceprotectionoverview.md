---
title: deviceProtectionOverview 资源类型
description: 硬件的给定设备的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418986"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="e06bb-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="e06bb-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="e06bb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e06bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e06bb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e06bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e06bb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e06bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e06bb-107">硬件的给定设备的信息。</span><span class="sxs-lookup"><span data-stu-id="e06bb-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e06bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="e06bb-108">Properties</span></span>
|<span data-ttu-id="e06bb-109">属性</span><span class="sxs-lookup"><span data-stu-id="e06bb-109">Property</span></span>|<span data-ttu-id="e06bb-110">类型</span><span class="sxs-lookup"><span data-stu-id="e06bb-110">Type</span></span>|<span data-ttu-id="e06bb-111">说明</span><span class="sxs-lookup"><span data-stu-id="e06bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e06bb-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="e06bb-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-113">Int32</span></span>|<span data-ttu-id="e06bb-114">总设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-114">Total device count.</span></span>|
|<span data-ttu-id="e06bb-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="e06bb-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-116">Int32</span></span>|<span data-ttu-id="e06bb-117">非活动威胁代理计数设备</span><span class="sxs-lookup"><span data-stu-id="e06bb-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="e06bb-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="e06bb-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-119">Int32</span></span>|<span data-ttu-id="e06bb-120">与为未知计数的威胁代理状态的设备。</span><span class="sxs-lookup"><span data-stu-id="e06bb-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="e06bb-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="e06bb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-122">Int32</span></span>|<span data-ttu-id="e06bb-123">使用旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="e06bb-123">Device with old signature count.</span></span>|
|<span data-ttu-id="e06bb-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-124">cleanDeviceCount</span></span>|<span data-ttu-id="e06bb-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-125">Int32</span></span>|<span data-ttu-id="e06bb-126">清理设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-126">Clean device count.</span></span>|
|<span data-ttu-id="e06bb-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="e06bb-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-128">Int32</span></span>|<span data-ttu-id="e06bb-129">待处理的完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="e06bb-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="e06bb-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-131">Int32</span></span>|<span data-ttu-id="e06bb-132">挂起的重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-132">Pending restart device count.</span></span>|
|<span data-ttu-id="e06bb-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="e06bb-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-134">Int32</span></span>|<span data-ttu-id="e06bb-135">待处理的手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="e06bb-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="e06bb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-137">Int32</span></span>|<span data-ttu-id="e06bb-138">待处理的脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="e06bb-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e06bb-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="e06bb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e06bb-140">Int32</span></span>|<span data-ttu-id="e06bb-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="e06bb-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e06bb-142">关系</span><span class="sxs-lookup"><span data-stu-id="e06bb-142">Relationships</span></span>
<span data-ttu-id="e06bb-143">无</span><span class="sxs-lookup"><span data-stu-id="e06bb-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e06bb-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e06bb-144">JSON Representation</span></span>
<span data-ttu-id="e06bb-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e06bb-145">Here is a JSON representation of the resource.</span></span>
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




