---
title: deviceHealthScriptRunSummary 资源类型
description: 包含设备管理脚本的运行摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 959b6722f1a72ff1f423f4288ebebdcd14aada11
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528613"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="05a1a-103">deviceHealthScriptRunSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="05a1a-103">deviceHealthScriptRunSummary resource type</span></span>

<span data-ttu-id="05a1a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="05a1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05a1a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05a1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05a1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05a1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05a1a-107">包含设备管理脚本的运行摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="05a1a-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="05a1a-108">方法</span><span class="sxs-lookup"><span data-stu-id="05a1a-108">Methods</span></span>
|<span data-ttu-id="05a1a-109">方法</span><span class="sxs-lookup"><span data-stu-id="05a1a-109">Method</span></span>|<span data-ttu-id="05a1a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="05a1a-110">Return Type</span></span>|<span data-ttu-id="05a1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="05a1a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05a1a-112">获取 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="05a1a-112">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="05a1a-113">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="05a1a-113">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="05a1a-114">读取[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05a1a-114">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="05a1a-115">更新 deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="05a1a-115">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="05a1a-116">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="05a1a-116">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="05a1a-117">更新[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="05a1a-117">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05a1a-118">属性</span><span class="sxs-lookup"><span data-stu-id="05a1a-118">Properties</span></span>
|<span data-ttu-id="05a1a-119">属性</span><span class="sxs-lookup"><span data-stu-id="05a1a-119">Property</span></span>|<span data-ttu-id="05a1a-120">类型</span><span class="sxs-lookup"><span data-stu-id="05a1a-120">Type</span></span>|<span data-ttu-id="05a1a-121">说明</span><span class="sxs-lookup"><span data-stu-id="05a1a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05a1a-122">id</span><span class="sxs-lookup"><span data-stu-id="05a1a-122">id</span></span>|<span data-ttu-id="05a1a-123">String</span><span class="sxs-lookup"><span data-stu-id="05a1a-123">String</span></span>|<span data-ttu-id="05a1a-124">设备运行状况脚本的键运行摘要实体。</span><span class="sxs-lookup"><span data-stu-id="05a1a-124">Key of the device health script run summary entity.</span></span> <span data-ttu-id="05a1a-125">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="05a1a-125">This property is read-only.</span></span>|
|<span data-ttu-id="05a1a-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="05a1a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-127">Int32</span></span>|<span data-ttu-id="05a1a-128">检测脚本找不到问题且设备正常运行的设备数</span><span class="sxs-lookup"><span data-stu-id="05a1a-128">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="05a1a-129">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-129">issueDetectedDeviceCount</span></span>|<span data-ttu-id="05a1a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-130">Int32</span></span>|<span data-ttu-id="05a1a-131">检测脚本发现问题的设备数</span><span class="sxs-lookup"><span data-stu-id="05a1a-131">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="05a1a-132">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-132">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="05a1a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-133">Int32</span></span>|<span data-ttu-id="05a1a-134">检测脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="05a1a-134">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="05a1a-135">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-135">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="05a1a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-136">Int32</span></span>|<span data-ttu-id="05a1a-137">尚未运行的设备运行状况脚本的最新版本的设备数量</span><span class="sxs-lookup"><span data-stu-id="05a1a-137">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="05a1a-138">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-138">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="05a1a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-139">Int32</span></span>|<span data-ttu-id="05a1a-140">修正脚本能够解决检测到的问题的设备数</span><span class="sxs-lookup"><span data-stu-id="05a1a-140">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="05a1a-141">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-141">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="05a1a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-142">Int32</span></span>|<span data-ttu-id="05a1a-143">跳过修正的设备数</span><span class="sxs-lookup"><span data-stu-id="05a1a-143">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="05a1a-144">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-144">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="05a1a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-145">Int32</span></span>|<span data-ttu-id="05a1a-146">已成功执行修正脚本但未能解决检测到的问题的设备数量</span><span class="sxs-lookup"><span data-stu-id="05a1a-146">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="05a1a-147">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-147">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="05a1a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-148">Int32</span></span>|<span data-ttu-id="05a1a-149">修正脚本执行时遇到错误且未完成的设备数量</span><span class="sxs-lookup"><span data-stu-id="05a1a-149">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="05a1a-150">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="05a1a-150">lastScriptRunDateTime</span></span>|<span data-ttu-id="05a1a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05a1a-151">DateTimeOffset</span></span>|<span data-ttu-id="05a1a-152">在所有设备上的脚本的上次运行时间</span><span class="sxs-lookup"><span data-stu-id="05a1a-152">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="05a1a-153">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05a1a-153">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="05a1a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="05a1a-154">Int32</span></span>|<span data-ttu-id="05a1a-155">最近30天内修正的设备数量</span><span class="sxs-lookup"><span data-stu-id="05a1a-155">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="05a1a-156">关系</span><span class="sxs-lookup"><span data-stu-id="05a1a-156">Relationships</span></span>
<span data-ttu-id="05a1a-157">无</span><span class="sxs-lookup"><span data-stu-id="05a1a-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05a1a-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05a1a-158">JSON Representation</span></span>
<span data-ttu-id="05a1a-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05a1a-159">Here is a JSON representation of the resource.</span></span>
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



