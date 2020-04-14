---
title: deviceHealthScriptDeviceState 资源类型
description: 包含设备运行状况脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15b88acaf91e82981e821d96f8456cc943965081
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448118"
---
# <a name="devicehealthscriptdevicestate-resource-type"></a><span data-ttu-id="88969-103">deviceHealthScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="88969-103">deviceHealthScriptDeviceState resource type</span></span>

<span data-ttu-id="88969-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88969-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88969-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88969-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88969-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88969-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88969-107">包含设备运行状况脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="88969-107">Contains properties for device run state of the device health script.</span></span>

## <a name="methods"></a><span data-ttu-id="88969-108">方法</span><span class="sxs-lookup"><span data-stu-id="88969-108">Methods</span></span>
|<span data-ttu-id="88969-109">方法</span><span class="sxs-lookup"><span data-stu-id="88969-109">Method</span></span>|<span data-ttu-id="88969-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="88969-110">Return Type</span></span>|<span data-ttu-id="88969-111">说明</span><span class="sxs-lookup"><span data-stu-id="88969-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88969-112">列出 deviceHealthScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="88969-112">List deviceHealthScriptDeviceStates</span></span>](../api/intune-devices-devicehealthscriptdevicestate-list.md)|<span data-ttu-id="88969-113">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="88969-113">[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) collection</span></span>|<span data-ttu-id="88969-114">列出[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88969-114">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="88969-115">获取 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-115">Get deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-get.md)|[<span data-ttu-id="88969-116">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-116">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="88969-117">读取[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88969-117">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="88969-118">创建 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-118">Create deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-create.md)|[<span data-ttu-id="88969-119">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-119">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="88969-120">创建新的[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88969-120">Create a new [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="88969-121">删除 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-121">Delete deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-delete.md)|<span data-ttu-id="88969-122">无</span><span class="sxs-lookup"><span data-stu-id="88969-122">None</span></span>|<span data-ttu-id="88969-123">删除[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="88969-123">Deletes a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="88969-124">更新 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-124">Update deviceHealthScriptDeviceState</span></span>](../api/intune-devices-devicehealthscriptdevicestate-update.md)|[<span data-ttu-id="88969-125">deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="88969-125">deviceHealthScriptDeviceState</span></span>](../resources/intune-devices-devicehealthscriptdevicestate.md)|<span data-ttu-id="88969-126">更新[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88969-126">Update the properties of a [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88969-127">属性</span><span class="sxs-lookup"><span data-stu-id="88969-127">Properties</span></span>
|<span data-ttu-id="88969-128">属性</span><span class="sxs-lookup"><span data-stu-id="88969-128">Property</span></span>|<span data-ttu-id="88969-129">类型</span><span class="sxs-lookup"><span data-stu-id="88969-129">Type</span></span>|<span data-ttu-id="88969-130">说明</span><span class="sxs-lookup"><span data-stu-id="88969-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88969-131">id</span><span class="sxs-lookup"><span data-stu-id="88969-131">id</span></span>|<span data-ttu-id="88969-132">String</span><span class="sxs-lookup"><span data-stu-id="88969-132">String</span></span>|<span data-ttu-id="88969-133">设备运行状况脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="88969-133">Key of the device health script device state entity.</span></span> <span data-ttu-id="88969-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88969-134">This property is read-only.</span></span>|
|<span data-ttu-id="88969-135">detectionState</span><span class="sxs-lookup"><span data-stu-id="88969-135">detectionState</span></span>|[<span data-ttu-id="88969-136">runState</span><span class="sxs-lookup"><span data-stu-id="88969-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="88969-137">Lastest 设备运行状况脚本执行的检测状态。</span><span class="sxs-lookup"><span data-stu-id="88969-137">Detection state from the lastest device health script execution.</span></span> <span data-ttu-id="88969-138">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="88969-138">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="88969-139">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="88969-139">lastStateUpdateDateTime</span></span>|<span data-ttu-id="88969-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88969-140">DateTimeOffset</span></span>|<span data-ttu-id="88969-141">执行设备运行状况脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="88969-141">The last timestamp of when the device health script executed</span></span>|
|<span data-ttu-id="88969-142">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="88969-142">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="88969-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88969-143">DateTimeOffset</span></span>|<span data-ttu-id="88969-144">应在何时执行设备运行状况脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="88969-144">The next timestamp of when the device health script is expected to execute</span></span>|
|<span data-ttu-id="88969-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="88969-145">lastSyncDateTime</span></span>|<span data-ttu-id="88969-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88969-146">DateTimeOffset</span></span>|<span data-ttu-id="88969-147">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="88969-147">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="88969-148">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="88969-148">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="88969-149">String</span><span class="sxs-lookup"><span data-stu-id="88969-149">String</span></span>|<span data-ttu-id="88969-150">修正前的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="88969-150">Output of the detection script before remediation</span></span>|
|<span data-ttu-id="88969-151">preRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="88969-151">preRemediationDetectionScriptError</span></span>|<span data-ttu-id="88969-152">String</span><span class="sxs-lookup"><span data-stu-id="88969-152">String</span></span>|<span data-ttu-id="88969-153">修正前的检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="88969-153">Error from the detection script before remediation</span></span>|
|<span data-ttu-id="88969-154">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="88969-154">remediationScriptError</span></span>|<span data-ttu-id="88969-155">String</span><span class="sxs-lookup"><span data-stu-id="88969-155">String</span></span>|<span data-ttu-id="88969-156">修正脚本的错误输出</span><span class="sxs-lookup"><span data-stu-id="88969-156">Error output of the remediation script</span></span>|
|<span data-ttu-id="88969-157">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="88969-157">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="88969-158">String</span><span class="sxs-lookup"><span data-stu-id="88969-158">String</span></span>|<span data-ttu-id="88969-159">修正后的检测脚本输出</span><span class="sxs-lookup"><span data-stu-id="88969-159">Detection script output after remediation</span></span>|
|<span data-ttu-id="88969-160">postRemediationDetectionScriptError</span><span class="sxs-lookup"><span data-stu-id="88969-160">postRemediationDetectionScriptError</span></span>|<span data-ttu-id="88969-161">String</span><span class="sxs-lookup"><span data-stu-id="88969-161">String</span></span>|<span data-ttu-id="88969-162">更正后来自检测脚本的错误</span><span class="sxs-lookup"><span data-stu-id="88969-162">Error from the detection script after remediation</span></span>|
|<span data-ttu-id="88969-163">remediationState</span><span class="sxs-lookup"><span data-stu-id="88969-163">remediationState</span></span>|[<span data-ttu-id="88969-164">remediationState</span><span class="sxs-lookup"><span data-stu-id="88969-164">remediationState</span></span>](../resources/intune-devices-remediationstate.md)|<span data-ttu-id="88969-165">来自 lastest 设备运行状况脚本执行的修正状态。</span><span class="sxs-lookup"><span data-stu-id="88969-165">Remediation state from the lastest device health script execution.</span></span> <span data-ttu-id="88969-166">可取值为：`unknown`、`skipped`、`success`、`remediationFailed`、`scriptError`。</span><span class="sxs-lookup"><span data-stu-id="88969-166">Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88969-167">关系</span><span class="sxs-lookup"><span data-stu-id="88969-167">Relationships</span></span>
|<span data-ttu-id="88969-168">关系</span><span class="sxs-lookup"><span data-stu-id="88969-168">Relationship</span></span>|<span data-ttu-id="88969-169">类型</span><span class="sxs-lookup"><span data-stu-id="88969-169">Type</span></span>|<span data-ttu-id="88969-170">说明</span><span class="sxs-lookup"><span data-stu-id="88969-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88969-171">managedDevice</span><span class="sxs-lookup"><span data-stu-id="88969-171">managedDevice</span></span>|[<span data-ttu-id="88969-172">managedDevice</span><span class="sxs-lookup"><span data-stu-id="88969-172">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="88969-173">在其上执行设备运行状况脚本的托管设备</span><span class="sxs-lookup"><span data-stu-id="88969-173">The managed device on which the device health script executed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88969-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88969-174">JSON Representation</span></span>
<span data-ttu-id="88969-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88969-175">Here is a JSON representation of the resource.</span></span>
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



