---
title: deviceHealthScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1c1b31413c19436c7dceb34a2055a238fe5881a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665229"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="aec99-103">deviceHealthScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="aec99-103">deviceHealthScriptRunSummary resource type</span></span>

<span data-ttu-id="aec99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aec99-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aec99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aec99-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aec99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec99-107">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="aec99-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="aec99-108">方法</span><span class="sxs-lookup"><span data-stu-id="aec99-108">Methods</span></span>
|<span data-ttu-id="aec99-109">方法</span><span class="sxs-lookup"><span data-stu-id="aec99-109">Method</span></span>|<span data-ttu-id="aec99-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="aec99-110">Return Type</span></span>|<span data-ttu-id="aec99-111">说明</span><span class="sxs-lookup"><span data-stu-id="aec99-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aec99-112">获取 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aec99-112">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="aec99-113">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aec99-113">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="aec99-114">读取 [deviceHealthScriptRunSummary 对象的属性和](../resources/intune-devices-devicehealthscriptrunsummary.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="aec99-114">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="aec99-115">更新 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aec99-115">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="aec99-116">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="aec99-116">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="aec99-117">更新 [deviceHealthScriptRunSummary 对象](../resources/intune-devices-devicehealthscriptrunsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="aec99-117">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aec99-118">属性</span><span class="sxs-lookup"><span data-stu-id="aec99-118">Properties</span></span>
|<span data-ttu-id="aec99-119">属性</span><span class="sxs-lookup"><span data-stu-id="aec99-119">Property</span></span>|<span data-ttu-id="aec99-120">类型</span><span class="sxs-lookup"><span data-stu-id="aec99-120">Type</span></span>|<span data-ttu-id="aec99-121">说明</span><span class="sxs-lookup"><span data-stu-id="aec99-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec99-122">id</span><span class="sxs-lookup"><span data-stu-id="aec99-122">id</span></span>|<span data-ttu-id="aec99-123">String</span><span class="sxs-lookup"><span data-stu-id="aec99-123">String</span></span>|<span data-ttu-id="aec99-124">设备运行状况脚本运行摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="aec99-124">Key of the device health script run summary entity.</span></span> <span data-ttu-id="aec99-125">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aec99-125">This property is read-only.</span></span>|
|<span data-ttu-id="aec99-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="aec99-127">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-127">Int32</span></span>|<span data-ttu-id="aec99-128">检测脚本未发现问题且设备正常运行的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-128">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="aec99-129">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-129">issueDetectedDeviceCount</span></span>|<span data-ttu-id="aec99-130">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-130">Int32</span></span>|<span data-ttu-id="aec99-131">检测脚本发现问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-131">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="aec99-132">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-132">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="aec99-133">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-133">Int32</span></span>|<span data-ttu-id="aec99-134">检测脚本执行遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-134">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="aec99-135">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-135">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="aec99-136">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-136">Int32</span></span>|<span data-ttu-id="aec99-137">尚未运行最新版本的设备运行状况脚本的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-137">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="aec99-138">detectionScriptNotApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-138">detectionScriptNotApplicableDeviceCount</span></span>|<span data-ttu-id="aec99-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-139">Int32</span></span>|<span data-ttu-id="aec99-140">检测脚本不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-140">Number of devices for which the detection script was not applicable</span></span>|
|<span data-ttu-id="aec99-141">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-141">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="aec99-142">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-142">Int32</span></span>|<span data-ttu-id="aec99-143">修正脚本能够解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-143">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="aec99-144">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-144">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="aec99-145">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-145">Int32</span></span>|<span data-ttu-id="aec99-146">已跳过修正的设备数</span><span class="sxs-lookup"><span data-stu-id="aec99-146">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="aec99-147">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-147">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="aec99-148">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-148">Int32</span></span>|<span data-ttu-id="aec99-149">修复脚本成功执行但未能解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-149">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="aec99-150">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-150">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="aec99-151">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-151">Int32</span></span>|<span data-ttu-id="aec99-152">修正脚本执行遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="aec99-152">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="aec99-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="aec99-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="aec99-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec99-154">DateTimeOffset</span></span>|<span data-ttu-id="aec99-155">脚本跨所有设备的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="aec99-155">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="aec99-156">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aec99-156">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="aec99-157">Int32</span><span class="sxs-lookup"><span data-stu-id="aec99-157">Int32</span></span>|<span data-ttu-id="aec99-158">过去 30 天内修正的设备数</span><span class="sxs-lookup"><span data-stu-id="aec99-158">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="aec99-159">关系</span><span class="sxs-lookup"><span data-stu-id="aec99-159">Relationships</span></span>
<span data-ttu-id="aec99-160">无</span><span class="sxs-lookup"><span data-stu-id="aec99-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aec99-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aec99-161">JSON Representation</span></span>
<span data-ttu-id="aec99-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aec99-162">Here is a JSON representation of the resource.</span></span>
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
  "detectionScriptNotApplicableDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```




