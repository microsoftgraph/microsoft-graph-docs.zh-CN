---
title: deviceProtectionOverview 资源类型
description: 硬件的给定设备的信息。
author: tfitzmac
ms.openlocfilehash: e705324bfc611117657ec629f8770e76c69be28d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317050"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="c532b-103">deviceProtectionOverview 资源类型</span><span class="sxs-lookup"><span data-stu-id="c532b-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="c532b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c532b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c532b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c532b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c532b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c532b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c532b-107">硬件的给定设备的信息。</span><span class="sxs-lookup"><span data-stu-id="c532b-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="c532b-108">属性</span><span class="sxs-lookup"><span data-stu-id="c532b-108">Properties</span></span>
|<span data-ttu-id="c532b-109">属性</span><span class="sxs-lookup"><span data-stu-id="c532b-109">Property</span></span>|<span data-ttu-id="c532b-110">类型</span><span class="sxs-lookup"><span data-stu-id="c532b-110">Type</span></span>|<span data-ttu-id="c532b-111">说明</span><span class="sxs-lookup"><span data-stu-id="c532b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c532b-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="c532b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-113">Int32</span></span>|<span data-ttu-id="c532b-114">总设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-114">Total device count.</span></span>|
|<span data-ttu-id="c532b-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="c532b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-116">Int32</span></span>|<span data-ttu-id="c532b-117">非活动威胁代理计数设备</span><span class="sxs-lookup"><span data-stu-id="c532b-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="c532b-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="c532b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-119">Int32</span></span>|<span data-ttu-id="c532b-120">与为未知计数的威胁代理状态的设备。</span><span class="sxs-lookup"><span data-stu-id="c532b-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="c532b-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="c532b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-122">Int32</span></span>|<span data-ttu-id="c532b-123">使用旧签名计数的设备。</span><span class="sxs-lookup"><span data-stu-id="c532b-123">Device with old signature count.</span></span>|
|<span data-ttu-id="c532b-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-124">cleanDeviceCount</span></span>|<span data-ttu-id="c532b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-125">Int32</span></span>|<span data-ttu-id="c532b-126">清理设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-126">Clean device count.</span></span>|
|<span data-ttu-id="c532b-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="c532b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-128">Int32</span></span>|<span data-ttu-id="c532b-129">待处理的完全扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="c532b-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="c532b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-131">Int32</span></span>|<span data-ttu-id="c532b-132">挂起的重新启动设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-132">Pending restart device count.</span></span>|
|<span data-ttu-id="c532b-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="c532b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-134">Int32</span></span>|<span data-ttu-id="c532b-135">待处理的手动步骤设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="c532b-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="c532b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-137">Int32</span></span>|<span data-ttu-id="c532b-138">待处理的脱机扫描设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="c532b-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c532b-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="c532b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c532b-140">Int32</span></span>|<span data-ttu-id="c532b-141">严重故障设备计数。</span><span class="sxs-lookup"><span data-stu-id="c532b-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c532b-142">Relationships</span><span class="sxs-lookup"><span data-stu-id="c532b-142">Relationships</span></span>
<span data-ttu-id="c532b-143">无</span><span class="sxs-lookup"><span data-stu-id="c532b-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c532b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c532b-144">JSON Representation</span></span>
<span data-ttu-id="c532b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c532b-145">Here is a JSON representation of the resource.</span></span>
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





