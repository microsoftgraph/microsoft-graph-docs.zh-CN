---
title: deviceHealthScriptDeviceState 资源类型
description: 包含设备运行状况脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3973b74215acc1aa817653cec3354f01c49cb8b5
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612068"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a><span data-ttu-id="3cb78-103">deviceHealthScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="3cb78-103">deviceHealthScriptDeviceState resource type</span></span>

<span data-ttu-id="3cb78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cb78-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3cb78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cb78-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cb78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cb78-107">包含设备运行状况脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="3cb78-107">Contains properties for device run state of the device health script.</span></span>

## <a name="methods"></a><span data-ttu-id="3cb78-108">方法</span><span class="sxs-lookup"><span data-stu-id="3cb78-108">Methods</span></span>
|<span data-ttu-id="3cb78-109">方法</span><span class="sxs-lookup"><span data-stu-id="3cb78-109">Method</span></span>|<span data-ttu-id="3cb78-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3cb78-110">Return Type</span></span>|<span data-ttu-id="3cb78-111">Description</span><span class="sxs-lookup"><span data-stu-id="3cb78-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3cb78-112">列出 deviceHealthScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="3cb78-112">List deviceHealthScriptDeviceStates</span></span>](../api/intune-devices-devicehealthscriptdevicestate-list.md)|<span data-ttu-id="3cb78-113">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3cb78-113">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="3cb78-114">列出 [deviceHealthScriptDeviceState 对象的属性和](../resources/intune-devices-devicehealthscriptdevicestate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3cb78-114">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="3cb78-115">获取 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-115">Get deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[<span data-ttu-id="3cb78-116">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-116">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="3cb78-117">读取 [deviceHealthScriptDeviceState 对象的属性和](../resources/intune-devices-devicehealthscriptdevicestate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3cb78-117">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="3cb78-118">创建 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-118">Create deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[<span data-ttu-id="3cb78-119">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-119">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="3cb78-120">创建新的 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cb78-120">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="3cb78-121">删除 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-121">Delete deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|<span data-ttu-id="3cb78-122">无</span><span class="sxs-lookup"><span data-stu-id="3cb78-122">None</span></span>|<span data-ttu-id="3cb78-123">删除 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="3cb78-123">Deletes a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="3cb78-124">更新 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-124">Update deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[<span data-ttu-id="3cb78-125">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="3cb78-125">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="3cb78-126">更新 [deviceHealthScriptDeviceState 对象](../resources/intune-devices-devicehealthscriptdevicestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3cb78-126">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3cb78-127">属性</span><span class="sxs-lookup"><span data-stu-id="3cb78-127">Properties</span></span>
|<span data-ttu-id="3cb78-128">属性</span><span class="sxs-lookup"><span data-stu-id="3cb78-128">Property</span></span>|<span data-ttu-id="3cb78-129">类型</span><span class="sxs-lookup"><span data-stu-id="3cb78-129">Type</span></span>|<span data-ttu-id="3cb78-130">说明</span><span class="sxs-lookup"><span data-stu-id="3cb78-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb78-131">id</span><span class="sxs-lookup"><span data-stu-id="3cb78-131">id</span></span>|<span data-ttu-id="3cb78-132">String</span><span class="sxs-lookup"><span data-stu-id="3cb78-132">String</span></span>|<span data-ttu-id="3cb78-133">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="3cb78-133">Key of the device health script device state entity.</span></span> <span data-ttu-id="3cb78-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3cb78-134">This property is read-only.</span></span>|
|<span data-ttu-id="3cb78-135">detectionState</span><span class="sxs-lookup"><span data-stu-id="3cb78-135">detectionState</span></span>|[<span data-ttu-id="3cb78-136">runState</span><span class="sxs-lookup"><span data-stu-id="3cb78-136">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="3cb78-137">最近一次执行设备运行状况脚本的检测状态。</span><span class="sxs-lookup"><span data-stu-id="3cb78-137">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="3cb78-138">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="3cb78-138">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="3cb78-139">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3cb78-139">lastStateUpdateDateTime</span></span>|<span data-ttu-id="3cb78-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb78-140">DateTimeOffset</span></span>|<span data-ttu-id="3cb78-141">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="3cb78-141">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="3cb78-142">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3cb78-142">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="3cb78-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb78-143">DateTimeOffset</span></span>|<span data-ttu-id="3cb78-144">预计执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="3cb78-144">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="3cb78-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3cb78-145">lastSyncDateTime</span></span>|<span data-ttu-id="3cb78-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb78-146">DateTimeOffset</span></span>|<span data-ttu-id="3cb78-147">Intune 管理扩展上次与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="3cb78-147">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="3cb78-148">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="3cb78-148">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="3cb78-149">String</span><span class="sxs-lookup"><span data-stu-id="3cb78-149">String</span></span>|<span data-ttu-id="3cb78-150">修正前检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="3cb78-150">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="3cb78-151">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="3cb78-151">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="3cb78-152">String</span><span class="sxs-lookup"><span data-stu-id="3cb78-152">String</span></span>|<span data-ttu-id="3cb78-153">修正前检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="3cb78-153">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="3cb78-154">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="3cb78-154">remediationScriptError</span></span>|<span data-ttu-id="3cb78-155">String</span><span class="sxs-lookup"><span data-stu-id="3cb78-155">String</span></span>|<span data-ttu-id="3cb78-156">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="3cb78-156">Error output of the remediation script</span></span>|
|<span data-ttu-id="3cb78-157">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="3cb78-157">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="3cb78-158">String</span><span class="sxs-lookup"><span data-stu-id="3cb78-158">String</span></span>|<span data-ttu-id="3cb78-159">修正后检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="3cb78-159">Detection script output after remediation</span></span>|
|<span data-ttu-id="3cb78-160">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="3cb78-160">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="3cb78-161">String</span><span class="sxs-lookup"><span data-stu-id="3cb78-161">String</span></span>|<span data-ttu-id="3cb78-162">修正后检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="3cb78-162">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="3cb78-163">remediationState</span><span class="sxs-lookup"><span data-stu-id="3cb78-163">remediationState</span></span>|[<span data-ttu-id="3cb78-164">remediationState</span><span class="sxs-lookup"><span data-stu-id="3cb78-164">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="3cb78-165">自上次设备运行状况脚本执行以来的修正状态。</span><span class="sxs-lookup"><span data-stu-id="3cb78-165">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="3cb78-166">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="3cb78-166">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cb78-167">关系</span><span class="sxs-lookup"><span data-stu-id="3cb78-167">Relationships</span></span>
|<span data-ttu-id="3cb78-168">关系</span><span class="sxs-lookup"><span data-stu-id="3cb78-168">Relationship</span></span>|<span data-ttu-id="3cb78-169">类型</span><span class="sxs-lookup"><span data-stu-id="3cb78-169">Type</span></span>|<span data-ttu-id="3cb78-170">Description</span><span class="sxs-lookup"><span data-stu-id="3cb78-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb78-171">managedDevice</span><span class="sxs-lookup"><span data-stu-id="3cb78-171">managedDevice</span></span>|[<span data-ttu-id="3cb78-172">managedDevice</span><span class="sxs-lookup"><span data-stu-id="3cb78-172">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="3cb78-173">执行设备运行状况脚本的托管设备</span><span class="sxs-lookup"><span data-stu-id="3cb78-173">The managed device on which the device health script executed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cb78-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cb78-174">JSON Representation</span></span>
<span data-ttu-id="3cb78-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cb78-175">Here is a JSON representation of the resource.</span></span>
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




