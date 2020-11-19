---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3b339f468f2fe1b67f5603ec67a16643ced53bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267465"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="224ad-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="224ad-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="224ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="224ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="224ad-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="224ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="224ad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="224ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="224ad-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="224ad-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="224ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="224ad-108">Properties</span></span>
|<span data-ttu-id="224ad-109">属性</span><span class="sxs-lookup"><span data-stu-id="224ad-109">Property</span></span>|<span data-ttu-id="224ad-110">类型</span><span class="sxs-lookup"><span data-stu-id="224ad-110">Type</span></span>|<span data-ttu-id="224ad-111">说明</span><span class="sxs-lookup"><span data-stu-id="224ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224ad-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="224ad-113">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-113">Int32</span></span>|<span data-ttu-id="224ad-114">设备计数总数。</span><span class="sxs-lookup"><span data-stu-id="224ad-114">Total device count.</span></span>|
|<span data-ttu-id="224ad-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="224ad-116">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-116">Int32</span></span>|<span data-ttu-id="224ad-117">带有非活动威胁代理计数的设备</span><span class="sxs-lookup"><span data-stu-id="224ad-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="224ad-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="224ad-119">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-119">Int32</span></span>|<span data-ttu-id="224ad-120">包含威胁代理状态的设备作为未知计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="224ad-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="224ad-122">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-122">Int32</span></span>|<span data-ttu-id="224ad-123">具有旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="224ad-123">Device with old signature count.</span></span>|
|<span data-ttu-id="224ad-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-124">cleanDeviceCount</span></span>|<span data-ttu-id="224ad-125">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-125">Int32</span></span>|<span data-ttu-id="224ad-126">清洗设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-126">Clean device count.</span></span>|
|<span data-ttu-id="224ad-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="224ad-128">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-128">Int32</span></span>|<span data-ttu-id="224ad-129">正在等待完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="224ad-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="224ad-131">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-131">Int32</span></span>|<span data-ttu-id="224ad-132">等待重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-132">Pending restart device count.</span></span>|
|<span data-ttu-id="224ad-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="224ad-134">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-134">Int32</span></span>|<span data-ttu-id="224ad-135">正在等待手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="224ad-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="224ad-137">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-137">Int32</span></span>|<span data-ttu-id="224ad-138">等待脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="224ad-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="224ad-140">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-140">Int32</span></span>|<span data-ttu-id="224ad-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-141">Critical failures device count.</span></span>|
|<span data-ttu-id="224ad-142">pendingQuickScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="224ad-142">pendingQuickScanDeviceCount</span></span>|<span data-ttu-id="224ad-143">Int32</span><span class="sxs-lookup"><span data-stu-id="224ad-143">Int32</span></span>|<span data-ttu-id="224ad-144">等待快速扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="224ad-144">Pending quick scan device count.</span></span> <span data-ttu-id="224ad-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="224ad-145">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="224ad-146">关系</span><span class="sxs-lookup"><span data-stu-id="224ad-146">Relationships</span></span>
<span data-ttu-id="224ad-147">无</span><span class="sxs-lookup"><span data-stu-id="224ad-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="224ad-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="224ad-148">JSON Representation</span></span>
<span data-ttu-id="224ad-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="224ad-149">Here is a JSON representation of the resource.</span></span>
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




