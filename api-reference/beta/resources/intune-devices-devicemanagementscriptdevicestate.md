---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86f3dcfefb80765ff13bb8742d88fdd869072f66
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370044"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="2c339-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c339-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="2c339-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c339-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c339-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c339-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c339-106">包含设备管理脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="2c339-106">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="2c339-107">方法</span><span class="sxs-lookup"><span data-stu-id="2c339-107">Methods</span></span>
|<span data-ttu-id="2c339-108">方法</span><span class="sxs-lookup"><span data-stu-id="2c339-108">Method</span></span>|<span data-ttu-id="2c339-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c339-109">Return Type</span></span>|<span data-ttu-id="2c339-110">说明</span><span class="sxs-lookup"><span data-stu-id="2c339-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c339-111">列出 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="2c339-111">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="2c339-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c339-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="2c339-113">列出[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c339-113">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="2c339-114">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-114">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="2c339-115">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-115">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="2c339-116">读取[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c339-116">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="2c339-117">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-117">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="2c339-118">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-118">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="2c339-119">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c339-119">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="2c339-120">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-120">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="2c339-121">无</span><span class="sxs-lookup"><span data-stu-id="2c339-121">None</span></span>|<span data-ttu-id="2c339-122">删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="2c339-122">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="2c339-123">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-123">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="2c339-124">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="2c339-124">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="2c339-125">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c339-125">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c339-126">属性</span><span class="sxs-lookup"><span data-stu-id="2c339-126">Properties</span></span>
|<span data-ttu-id="2c339-127">属性</span><span class="sxs-lookup"><span data-stu-id="2c339-127">Property</span></span>|<span data-ttu-id="2c339-128">类型</span><span class="sxs-lookup"><span data-stu-id="2c339-128">Type</span></span>|<span data-ttu-id="2c339-129">说明</span><span class="sxs-lookup"><span data-stu-id="2c339-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c339-130">id</span><span class="sxs-lookup"><span data-stu-id="2c339-130">id</span></span>|<span data-ttu-id="2c339-131">String</span><span class="sxs-lookup"><span data-stu-id="2c339-131">String</span></span>|<span data-ttu-id="2c339-132">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="2c339-132">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="2c339-133">runState</span><span class="sxs-lookup"><span data-stu-id="2c339-133">runState</span></span>|[<span data-ttu-id="2c339-134">runState</span><span class="sxs-lookup"><span data-stu-id="2c339-134">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="2c339-135">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="2c339-135">State of latest run of the device management script.</span></span> <span data-ttu-id="2c339-136">可取值为：`unknown`、`success`、`fail`、`error`、`pending`。</span><span class="sxs-lookup"><span data-stu-id="2c339-136">Possible values are: `unknown`, `success`, `fail`, `error`, `pending`.</span></span>|
|<span data-ttu-id="2c339-137">resultMessage</span><span class="sxs-lookup"><span data-stu-id="2c339-137">resultMessage</span></span>|<span data-ttu-id="2c339-138">String</span><span class="sxs-lookup"><span data-stu-id="2c339-138">String</span></span>|<span data-ttu-id="2c339-139">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c339-139">Details of execution output.</span></span>|
|<span data-ttu-id="2c339-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2c339-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="2c339-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c339-141">DateTimeOffset</span></span>|<span data-ttu-id="2c339-142">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="2c339-142">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="2c339-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="2c339-143">errorCode</span></span>|<span data-ttu-id="2c339-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2c339-144">Int32</span></span>|<span data-ttu-id="2c339-145">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="2c339-145">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="2c339-146">errorDescription</span><span class="sxs-lookup"><span data-stu-id="2c339-146">errorDescription</span></span>|<span data-ttu-id="2c339-147">String</span><span class="sxs-lookup"><span data-stu-id="2c339-147">String</span></span>|<span data-ttu-id="2c339-148">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="2c339-148">Error description corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="2c339-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2c339-149">lastSyncDateTime</span></span>|<span data-ttu-id="2c339-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c339-150">DateTimeOffset</span></span>|<span data-ttu-id="2c339-151">Intune 管理扩展将同步到 Intune 的最新时间。</span><span class="sxs-lookup"><span data-stu-id="2c339-151">The latest time that Intune Managment Extension syncs to Intune.</span></span>|
|<span data-ttu-id="2c339-152">preRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="2c339-152">preRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="2c339-153">String</span><span class="sxs-lookup"><span data-stu-id="2c339-153">String</span></span>|<span data-ttu-id="2c339-154">修复前的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="2c339-154">Output of the detection script before remediation.</span></span>|
|<span data-ttu-id="2c339-155">remediationScriptError</span><span class="sxs-lookup"><span data-stu-id="2c339-155">remediationScriptError</span></span>|<span data-ttu-id="2c339-156">String</span><span class="sxs-lookup"><span data-stu-id="2c339-156">String</span></span>|<span data-ttu-id="2c339-157">修正脚本的错误输出。</span><span class="sxs-lookup"><span data-stu-id="2c339-157">Error output of the remediation script.</span></span>|
|<span data-ttu-id="2c339-158">postRemediationDetectionScriptOutput</span><span class="sxs-lookup"><span data-stu-id="2c339-158">postRemediationDetectionScriptOutput</span></span>|<span data-ttu-id="2c339-159">String</span><span class="sxs-lookup"><span data-stu-id="2c339-159">String</span></span>|<span data-ttu-id="2c339-160">修正后的检测脚本输出。</span><span class="sxs-lookup"><span data-stu-id="2c339-160">Detection script output after remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c339-161">关系</span><span class="sxs-lookup"><span data-stu-id="2c339-161">Relationships</span></span>
|<span data-ttu-id="2c339-162">关系</span><span class="sxs-lookup"><span data-stu-id="2c339-162">Relationship</span></span>|<span data-ttu-id="2c339-163">类型</span><span class="sxs-lookup"><span data-stu-id="2c339-163">Type</span></span>|<span data-ttu-id="2c339-164">说明</span><span class="sxs-lookup"><span data-stu-id="2c339-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c339-165">managedDevice</span><span class="sxs-lookup"><span data-stu-id="2c339-165">managedDevice</span></span>|[<span data-ttu-id="2c339-166">managedDevice</span><span class="sxs-lookup"><span data-stu-id="2c339-166">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="2c339-167">执行设备管理脚本的托管设备。</span><span class="sxs-lookup"><span data-stu-id="2c339-167">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c339-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c339-168">JSON Representation</span></span>
<span data-ttu-id="2c339-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c339-169">Here is a JSON representation of the resource.</span></span>
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



