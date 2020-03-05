---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcdcbe69c1c5d94a00ec50e7e7b29b11a471441f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528595"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="05063-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="05063-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="05063-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="05063-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05063-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05063-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05063-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05063-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05063-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="05063-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="05063-108">属性</span><span class="sxs-lookup"><span data-stu-id="05063-108">Properties</span></span>
|<span data-ttu-id="05063-109">属性</span><span class="sxs-lookup"><span data-stu-id="05063-109">Property</span></span>|<span data-ttu-id="05063-110">类型</span><span class="sxs-lookup"><span data-stu-id="05063-110">Type</span></span>|<span data-ttu-id="05063-111">说明</span><span class="sxs-lookup"><span data-stu-id="05063-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05063-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="05063-113">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-113">Int32</span></span>|<span data-ttu-id="05063-114">设备计数总数。</span><span class="sxs-lookup"><span data-stu-id="05063-114">Total device count.</span></span>|
|<span data-ttu-id="05063-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="05063-116">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-116">Int32</span></span>|<span data-ttu-id="05063-117">带有非活动威胁代理计数的设备</span><span class="sxs-lookup"><span data-stu-id="05063-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="05063-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="05063-119">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-119">Int32</span></span>|<span data-ttu-id="05063-120">包含威胁代理状态的设备作为未知计数。</span><span class="sxs-lookup"><span data-stu-id="05063-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="05063-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="05063-122">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-122">Int32</span></span>|<span data-ttu-id="05063-123">具有旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="05063-123">Device with old signature count.</span></span>|
|<span data-ttu-id="05063-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-124">cleanDeviceCount</span></span>|<span data-ttu-id="05063-125">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-125">Int32</span></span>|<span data-ttu-id="05063-126">清洗设备计数。</span><span class="sxs-lookup"><span data-stu-id="05063-126">Clean device count.</span></span>|
|<span data-ttu-id="05063-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="05063-128">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-128">Int32</span></span>|<span data-ttu-id="05063-129">正在等待完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="05063-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="05063-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="05063-131">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-131">Int32</span></span>|<span data-ttu-id="05063-132">等待重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="05063-132">Pending restart device count.</span></span>|
|<span data-ttu-id="05063-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="05063-134">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-134">Int32</span></span>|<span data-ttu-id="05063-135">正在等待手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="05063-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="05063-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="05063-137">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-137">Int32</span></span>|<span data-ttu-id="05063-138">等待脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="05063-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="05063-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05063-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="05063-140">Int32</span><span class="sxs-lookup"><span data-stu-id="05063-140">Int32</span></span>|<span data-ttu-id="05063-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="05063-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05063-142">关系</span><span class="sxs-lookup"><span data-stu-id="05063-142">Relationships</span></span>
<span data-ttu-id="05063-143">无</span><span class="sxs-lookup"><span data-stu-id="05063-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05063-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05063-144">JSON Representation</span></span>
<span data-ttu-id="05063-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05063-145">Here is a JSON representation of the resource.</span></span>
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



