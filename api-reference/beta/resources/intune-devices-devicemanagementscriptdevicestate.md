---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cffc9ed9c5e4c5590386f022e78f52f2efd56666
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196950"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="26e56-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="26e56-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="26e56-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26e56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26e56-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26e56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e56-106">包含设备管理脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="26e56-106">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="26e56-107">方法</span><span class="sxs-lookup"><span data-stu-id="26e56-107">Methods</span></span>
|<span data-ttu-id="26e56-108">方法</span><span class="sxs-lookup"><span data-stu-id="26e56-108">Method</span></span>|<span data-ttu-id="26e56-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26e56-109">Return Type</span></span>|<span data-ttu-id="26e56-110">说明</span><span class="sxs-lookup"><span data-stu-id="26e56-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26e56-111">列出 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="26e56-111">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="26e56-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="26e56-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="26e56-113">列出[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26e56-113">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="26e56-114">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-114">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="26e56-115">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-115">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="26e56-116">读取[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26e56-116">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="26e56-117">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-117">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="26e56-118">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-118">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="26e56-119">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26e56-119">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="26e56-120">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-120">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="26e56-121">无</span><span class="sxs-lookup"><span data-stu-id="26e56-121">None</span></span>|<span data-ttu-id="26e56-122">删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="26e56-122">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="26e56-123">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-123">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="26e56-124">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="26e56-124">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="26e56-125">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26e56-125">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="26e56-126">属性</span><span class="sxs-lookup"><span data-stu-id="26e56-126">Properties</span></span>
|<span data-ttu-id="26e56-127">属性</span><span class="sxs-lookup"><span data-stu-id="26e56-127">Property</span></span>|<span data-ttu-id="26e56-128">类型</span><span class="sxs-lookup"><span data-stu-id="26e56-128">Type</span></span>|<span data-ttu-id="26e56-129">说明</span><span class="sxs-lookup"><span data-stu-id="26e56-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e56-130">id</span><span class="sxs-lookup"><span data-stu-id="26e56-130">id</span></span>|<span data-ttu-id="26e56-131">String</span><span class="sxs-lookup"><span data-stu-id="26e56-131">String</span></span>|<span data-ttu-id="26e56-132">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="26e56-132">Key of the device management script device state entity.</span></span> <span data-ttu-id="26e56-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="26e56-133">This property is read-only.</span></span>|
|<span data-ttu-id="26e56-134">runState</span><span class="sxs-lookup"><span data-stu-id="26e56-134">runState</span></span>|[<span data-ttu-id="26e56-135">runState</span><span class="sxs-lookup"><span data-stu-id="26e56-135">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="26e56-136">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="26e56-136">State of latest run of the device management script.</span></span> <span data-ttu-id="26e56-137">可取值为：`unknown`、`success`、`fail`、`error`、`pending`。</span><span class="sxs-lookup"><span data-stu-id="26e56-137">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="26e56-138">resultMessage</span><span class="sxs-lookup"><span data-stu-id="26e56-138">resultMessage</span></span>|<span data-ttu-id="26e56-139">String</span><span class="sxs-lookup"><span data-stu-id="26e56-139">String</span></span>|<span data-ttu-id="26e56-140">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26e56-140">Details of execution output.</span></span>|
|<span data-ttu-id="26e56-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="26e56-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="26e56-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e56-142">DateTimeOffset</span></span>|<span data-ttu-id="26e56-143">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="26e56-143">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="26e56-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="26e56-144">errorCode</span></span>|<span data-ttu-id="26e56-145">Int32</span><span class="sxs-lookup"><span data-stu-id="26e56-145">Int32</span></span>|<span data-ttu-id="26e56-146">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="26e56-146">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="26e56-147">errorDescription</span><span class="sxs-lookup"><span data-stu-id="26e56-147">errorDescription</span></span>|<span data-ttu-id="26e56-148">String</span><span class="sxs-lookup"><span data-stu-id="26e56-148">String</span></span>|<span data-ttu-id="26e56-149">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="26e56-149">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="26e56-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="26e56-150">lastSyncDateTime</span></span>|<span data-ttu-id="26e56-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e56-151">DateTimeOffset</span></span>|<span data-ttu-id="26e56-152">Intune 管理扩展将同步到 Intune 的最新时间。</span><span class="sxs-lookup"><span data-stu-id="26e56-152">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="26e56-153">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="26e56-153">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="26e56-154">String</span><span class="sxs-lookup"><span data-stu-id="26e56-154">String</span></span>|<span data-ttu-id="26e56-155">修复前的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="26e56-155">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="26e56-156">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="26e56-156">remediationScriptError</span></span>|<span data-ttu-id="26e56-157">String</span><span class="sxs-lookup"><span data-stu-id="26e56-157">String</span></span>|<span data-ttu-id="26e56-158">修正脚本的错误输出。</span><span class="sxs-lookup"><span data-stu-id="26e56-158">Error output of the remediation script.</span></span>|
|<span data-ttu-id="26e56-159">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="26e56-159">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="26e56-160">String</span><span class="sxs-lookup"><span data-stu-id="26e56-160">String</span></span>|<span data-ttu-id="26e56-161">修正后的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="26e56-161">Detection script output after remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26e56-162">关系</span><span class="sxs-lookup"><span data-stu-id="26e56-162">Relationships</span></span>
|<span data-ttu-id="26e56-163">关系</span><span class="sxs-lookup"><span data-stu-id="26e56-163">Relationship</span></span>|<span data-ttu-id="26e56-164">类型</span><span class="sxs-lookup"><span data-stu-id="26e56-164">Type</span></span>|<span data-ttu-id="26e56-165">说明</span><span class="sxs-lookup"><span data-stu-id="26e56-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e56-166">managedDevice</span><span class="sxs-lookup"><span data-stu-id="26e56-166">managedDevice</span></span>|[<span data-ttu-id="26e56-167">managedDevice</span><span class="sxs-lookup"><span data-stu-id="26e56-167">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="26e56-168">执行设备管理脚本的托管设备。</span><span class="sxs-lookup"><span data-stu-id="26e56-168">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26e56-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26e56-169">JSON Representation</span></span>
<span data-ttu-id="26e56-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26e56-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String"
}
```



