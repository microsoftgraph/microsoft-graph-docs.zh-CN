---
title: deviceHealthScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1be7c470bb2776b16f74f352dc93e1f56163abf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784935"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="e0426-103">deviceHealthScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0426-103">deviceHealthScriptRunSummary resource type</span></span>

> <span data-ttu-id="e0426-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0426-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0426-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0426-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0426-106">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="e0426-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="e0426-107">方法</span><span class="sxs-lookup"><span data-stu-id="e0426-107">Methods</span></span>
|<span data-ttu-id="e0426-108">方法</span><span class="sxs-lookup"><span data-stu-id="e0426-108">Method</span></span>|<span data-ttu-id="e0426-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0426-109">Return Type</span></span>|<span data-ttu-id="e0426-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0426-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0426-111">获取 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e0426-111">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="e0426-112">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e0426-112">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="e0426-113">读取[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0426-113">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="e0426-114">更新 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e0426-114">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="e0426-115">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e0426-115">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="e0426-116">更新[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0426-116">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0426-117">属性</span><span class="sxs-lookup"><span data-stu-id="e0426-117">Properties</span></span>
|<span data-ttu-id="e0426-118">属性</span><span class="sxs-lookup"><span data-stu-id="e0426-118">Property</span></span>|<span data-ttu-id="e0426-119">类型</span><span class="sxs-lookup"><span data-stu-id="e0426-119">Type</span></span>|<span data-ttu-id="e0426-120">说明</span><span class="sxs-lookup"><span data-stu-id="e0426-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0426-121">id</span><span class="sxs-lookup"><span data-stu-id="e0426-121">id</span></span>|<span data-ttu-id="e0426-122">String</span><span class="sxs-lookup"><span data-stu-id="e0426-122">String</span></span>|<span data-ttu-id="e0426-123">设备运行状况脚本的键运行摘要实体。</span><span class="sxs-lookup"><span data-stu-id="e0426-123">Key of the device health script run summary entity.</span></span> <span data-ttu-id="e0426-124">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e0426-124">This property is read-only.</span></span>|
|<span data-ttu-id="e0426-125">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-125">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="e0426-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-126">Int32</span></span>|<span data-ttu-id="e0426-127">检测脚本找不到问题且设备正常运行的设备数</span><span class="sxs-lookup"><span data-stu-id="e0426-127">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="e0426-128">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-128">issueDetectedDeviceCount</span></span>|<span data-ttu-id="e0426-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-129">Int32</span></span>|<span data-ttu-id="e0426-130">检测脚本发现问题的设备数</span><span class="sxs-lookup"><span data-stu-id="e0426-130">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="e0426-131">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-131">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="e0426-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-132">Int32</span></span>|<span data-ttu-id="e0426-133">检测脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="e0426-133">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="e0426-134">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-134">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="e0426-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-135">Int32</span></span>|<span data-ttu-id="e0426-136">尚未运行的设备运行状况脚本的最新版本的设备数量</span><span class="sxs-lookup"><span data-stu-id="e0426-136">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="e0426-137">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-137">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="e0426-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-138">Int32</span></span>|<span data-ttu-id="e0426-139">修正脚本能够解决检测到的问题的设备数</span><span class="sxs-lookup"><span data-stu-id="e0426-139">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="e0426-140">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-140">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="e0426-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-141">Int32</span></span>|<span data-ttu-id="e0426-142">跳过修正的设备数</span><span class="sxs-lookup"><span data-stu-id="e0426-142">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="e0426-143">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-143">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="e0426-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-144">Int32</span></span>|<span data-ttu-id="e0426-145">已成功执行修正脚本但未能解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="e0426-145">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="e0426-146">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-146">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="e0426-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-147">Int32</span></span>|<span data-ttu-id="e0426-148">修正脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="e0426-148">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="e0426-149">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="e0426-149">lastScriptRunDateTime</span></span>|<span data-ttu-id="e0426-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0426-150">DateTimeOffset</span></span>|<span data-ttu-id="e0426-151">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="e0426-151">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="e0426-152">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0426-152">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="e0426-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e0426-153">Int32</span></span>|<span data-ttu-id="e0426-154">最近30天内修正的设备数量</span><span class="sxs-lookup"><span data-stu-id="e0426-154">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0426-155">关系</span><span class="sxs-lookup"><span data-stu-id="e0426-155">Relationships</span></span>
<span data-ttu-id="e0426-156">无</span><span class="sxs-lookup"><span data-stu-id="e0426-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0426-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0426-157">JSON Representation</span></span>
<span data-ttu-id="e0426-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0426-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```



