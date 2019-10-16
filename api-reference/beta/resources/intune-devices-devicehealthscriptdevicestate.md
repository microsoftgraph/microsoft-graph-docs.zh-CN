---
title: deviceHealthScriptDeviceState 资源类型
description: 包含设备运行状况脚本的设备运行状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f9ae4ae7e6f014b52f4049d6663b732680d033d5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539083"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a><span data-ttu-id="6c525-103">deviceHealthScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c525-103">deviceHealthScriptDeviceState resource type</span></span>

> <span data-ttu-id="6c525-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c525-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c525-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c525-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c525-106">包含设备运行状况脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="6c525-106">Contains properties for device run state of the device health script.</span></span>

## <a name="methods"></a><span data-ttu-id="6c525-107">方法</span><span class="sxs-lookup"><span data-stu-id="6c525-107">Methods</span></span>
|<span data-ttu-id="6c525-108">方法</span><span class="sxs-lookup"><span data-stu-id="6c525-108">Method</span></span>|<span data-ttu-id="6c525-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c525-109">Return Type</span></span>|<span data-ttu-id="6c525-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c525-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c525-111">列出 deviceHealthScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="6c525-111">List deviceHealthScriptDeviceStates</span></span>](../api/intune-devices-devicehealthscriptdevicestate-list.md)|<span data-ttu-id="6c525-112">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="6c525-112">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="6c525-113">列出[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c525-113">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="6c525-114">获取 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-114">Get deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[<span data-ttu-id="6c525-115">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-115">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="6c525-116">读取[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c525-116">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="6c525-117">创建 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-117">Create deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[<span data-ttu-id="6c525-118">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-118">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="6c525-119">创建新的[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c525-119">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="6c525-120">删除 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-120">Delete deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|<span data-ttu-id="6c525-121">无</span><span class="sxs-lookup"><span data-stu-id="6c525-121">None</span></span>|<span data-ttu-id="6c525-122">删除[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="6c525-122">Deletes a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="6c525-123">更新 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-123">Update deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[<span data-ttu-id="6c525-124">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="6c525-124">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="6c525-125">更新[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6c525-125">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c525-126">属性</span><span class="sxs-lookup"><span data-stu-id="6c525-126">Properties</span></span>
|<span data-ttu-id="6c525-127">属性</span><span class="sxs-lookup"><span data-stu-id="6c525-127">Property</span></span>|<span data-ttu-id="6c525-128">类型</span><span class="sxs-lookup"><span data-stu-id="6c525-128">Type</span></span>|<span data-ttu-id="6c525-129">说明</span><span class="sxs-lookup"><span data-stu-id="6c525-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c525-130">id</span><span class="sxs-lookup"><span data-stu-id="6c525-130">id</span></span>|<span data-ttu-id="6c525-131">字符串</span><span class="sxs-lookup"><span data-stu-id="6c525-131">String</span></span>|<span data-ttu-id="6c525-132">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="6c525-132">Key of the device health script device state entity.</span></span> <span data-ttu-id="6c525-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6c525-133">This property is read-only.</span></span>|
|<span data-ttu-id="6c525-134">detectionState</span><span class="sxs-lookup"><span data-stu-id="6c525-134">detectionState</span></span>|[<span data-ttu-id="6c525-135">runState</span><span class="sxs-lookup"><span data-stu-id="6c525-135">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="6c525-136">Lastest 设备运行状况脚本执行的检测状态。</span><span class="sxs-lookup"><span data-stu-id="6c525-136">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="6c525-137">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="6c525-137">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="6c525-138">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6c525-138">lastStateUpdateDateTime</span></span>|<span data-ttu-id="6c525-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c525-139">DateTimeOffset</span></span>|<span data-ttu-id="6c525-140">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="6c525-140">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="6c525-141">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6c525-141">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="6c525-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c525-142">DateTimeOffset</span></span>|<span data-ttu-id="6c525-143">应在何时执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="6c525-143">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="6c525-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6c525-144">lastSyncDateTime</span></span>|<span data-ttu-id="6c525-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c525-145">DateTimeOffset</span></span>|<span data-ttu-id="6c525-146">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="6c525-146">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="6c525-147">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="6c525-147">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="6c525-148">字符串</span><span class="sxs-lookup"><span data-stu-id="6c525-148">String</span></span>|<span data-ttu-id="6c525-149">修正前的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="6c525-149">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="6c525-150">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="6c525-150">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="6c525-151">字符串</span><span class="sxs-lookup"><span data-stu-id="6c525-151">String</span></span>|<span data-ttu-id="6c525-152">修正前的检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="6c525-152">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="6c525-153">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="6c525-153">remediationScriptError</span></span>|<span data-ttu-id="6c525-154">字符串</span><span class="sxs-lookup"><span data-stu-id="6c525-154">String</span></span>|<span data-ttu-id="6c525-155">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="6c525-155">Error output of the remediation script</span></span>|
|<span data-ttu-id="6c525-156">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="6c525-156">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="6c525-157">字符串</span><span class="sxs-lookup"><span data-stu-id="6c525-157">String</span></span>|<span data-ttu-id="6c525-158">修正后的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="6c525-158">Detection script output after remediation</span></span>|
|<span data-ttu-id="6c525-159">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="6c525-159">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="6c525-160">字符串</span><span class="sxs-lookup"><span data-stu-id="6c525-160">String</span></span>|<span data-ttu-id="6c525-161">更正后来自检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="6c525-161">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="6c525-162">remediationState</span><span class="sxs-lookup"><span data-stu-id="6c525-162">remediationState</span></span>|[<span data-ttu-id="6c525-163">remediationState</span><span class="sxs-lookup"><span data-stu-id="6c525-163">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="6c525-164">来自 lastest 设备运行状况脚本执行的修正状态。</span><span class="sxs-lookup"><span data-stu-id="6c525-164">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="6c525-165">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="6c525-165">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c525-166">关系</span><span class="sxs-lookup"><span data-stu-id="6c525-166">Relationships</span></span>
|<span data-ttu-id="6c525-167">关系</span><span class="sxs-lookup"><span data-stu-id="6c525-167">Relationship</span></span>|<span data-ttu-id="6c525-168">类型</span><span class="sxs-lookup"><span data-stu-id="6c525-168">Type</span></span>|<span data-ttu-id="6c525-169">说明</span><span class="sxs-lookup"><span data-stu-id="6c525-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c525-170">managedDevice</span><span class="sxs-lookup"><span data-stu-id="6c525-170">managedDevice</span></span>|[<span data-ttu-id="6c525-171">managedDevice</span><span class="sxs-lookup"><span data-stu-id="6c525-171">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="6c525-172">在其上执行设备运行状况脚本的托管设备</span><span class="sxs-lookup"><span data-stu-id="6c525-172">The managed device on which the device health script executed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c525-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c525-173">JSON Representation</span></span>
<span data-ttu-id="6c525-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c525-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String"
}
```



