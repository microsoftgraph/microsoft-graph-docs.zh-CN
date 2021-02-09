---
title: deviceComplianceScriptDeviceState 资源类型
description: 包含设备合规性脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ad167c9145cebb965ec807a88c58588b3a8a1c8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158504"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a><span data-ttu-id="0eee2-103">deviceComplianceScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0eee2-103">deviceComplianceScriptDeviceState resource type</span></span>

<span data-ttu-id="0eee2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eee2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0eee2-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0eee2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eee2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0eee2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eee2-107">包含设备合规性脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="0eee2-107">Contains properties for device run state of the device compliance script.</span></span>

## <a name="methods"></a><span data-ttu-id="0eee2-108">方法</span><span class="sxs-lookup"><span data-stu-id="0eee2-108">Methods</span></span>
|<span data-ttu-id="0eee2-109">方法</span><span class="sxs-lookup"><span data-stu-id="0eee2-109">Method</span></span>|<span data-ttu-id="0eee2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0eee2-110">Return Type</span></span>|<span data-ttu-id="0eee2-111">说明</span><span class="sxs-lookup"><span data-stu-id="0eee2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0eee2-112">列出 deviceComplianceScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="0eee2-112">List deviceComplianceScriptDeviceStates</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|<span data-ttu-id="0eee2-113">[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0eee2-113">[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) collection</span></span>|<span data-ttu-id="0eee2-114">列出 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0eee2-114">List properties and relationships of the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="0eee2-115">获取 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-115">Get deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[<span data-ttu-id="0eee2-116">deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-116">deviceComplianceScriptDeviceState</span></span>](../resources/intune-devices-devicecompliancescriptdevicestate.md)|<span data-ttu-id="0eee2-117">读取 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0eee2-117">Read properties and relationships of the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0eee2-118">创建 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-118">Create deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[<span data-ttu-id="0eee2-119">deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-119">deviceComplianceScriptDeviceState</span></span>](../resources/intune-devices-devicecompliancescriptdevicestate.md)|<span data-ttu-id="0eee2-120">创建新的 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0eee2-120">Create a new [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0eee2-121">删除 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-121">Delete deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|<span data-ttu-id="0eee2-122">无</span><span class="sxs-lookup"><span data-stu-id="0eee2-122">None</span></span>|<span data-ttu-id="0eee2-123">删除 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="0eee2-123">Deletes a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>|
|[<span data-ttu-id="0eee2-124">更新 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-124">Update deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[<span data-ttu-id="0eee2-125">deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0eee2-125">deviceComplianceScriptDeviceState</span></span>](../resources/intune-devices-devicecompliancescriptdevicestate.md)|<span data-ttu-id="0eee2-126">更新 [deviceComplianceScriptDeviceState 对象](../resources/intune-devices-devicecompliancescriptdevicestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0eee2-126">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0eee2-127">属性</span><span class="sxs-lookup"><span data-stu-id="0eee2-127">Properties</span></span>
|<span data-ttu-id="0eee2-128">属性</span><span class="sxs-lookup"><span data-stu-id="0eee2-128">Property</span></span>|<span data-ttu-id="0eee2-129">类型</span><span class="sxs-lookup"><span data-stu-id="0eee2-129">Type</span></span>|<span data-ttu-id="0eee2-130">说明</span><span class="sxs-lookup"><span data-stu-id="0eee2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eee2-131">id</span><span class="sxs-lookup"><span data-stu-id="0eee2-131">id</span></span>|<span data-ttu-id="0eee2-132">String</span><span class="sxs-lookup"><span data-stu-id="0eee2-132">String</span></span>|<span data-ttu-id="0eee2-133">设备合规性脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="0eee2-133">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="0eee2-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0eee2-134">This property is read-only.</span></span>|
|<span data-ttu-id="0eee2-135">detectionState</span><span class="sxs-lookup"><span data-stu-id="0eee2-135">detectionState</span></span>|[<span data-ttu-id="0eee2-136">runState</span><span class="sxs-lookup"><span data-stu-id="0eee2-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="0eee2-137">最近一次执行设备合规性脚本的检测状态。</span><span class="sxs-lookup"><span data-stu-id="0eee2-137">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="0eee2-138">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="0eee2-138">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="0eee2-139">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0eee2-139">lastStateUpdateDateTime</span></span>|<span data-ttu-id="0eee2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eee2-140">DateTimeOffset</span></span>|<span data-ttu-id="0eee2-141">设备合规性脚本执行时间的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="0eee2-141">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="0eee2-142">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0eee2-142">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="0eee2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eee2-143">DateTimeOffset</span></span>|<span data-ttu-id="0eee2-144">预计执行设备合规性脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="0eee2-144">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="0eee2-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0eee2-145">lastSyncDateTime</span></span>|<span data-ttu-id="0eee2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eee2-146">DateTimeOffset</span></span>|<span data-ttu-id="0eee2-147">Intune 管理扩展上次与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="0eee2-147">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="0eee2-148">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="0eee2-148">scriptOutput</span></span>|<span data-ttu-id="0eee2-149">String</span><span class="sxs-lookup"><span data-stu-id="0eee2-149">String</span></span>|<span data-ttu-id="0eee2-150">检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="0eee2-150">Output of the detection script</span></span>|
|<span data-ttu-id="0eee2-151">scriptError</span><span class="sxs-lookup"><span data-stu-id="0eee2-151">scriptError</span></span>|<span data-ttu-id="0eee2-152">String</span><span class="sxs-lookup"><span data-stu-id="0eee2-152">String</span></span>|<span data-ttu-id="0eee2-153">检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="0eee2-153">Error from the detection script</span></span>|

## <a name="relationships"></a><span data-ttu-id="0eee2-154">关系</span><span class="sxs-lookup"><span data-stu-id="0eee2-154">Relationships</span></span>
|<span data-ttu-id="0eee2-155">关系</span><span class="sxs-lookup"><span data-stu-id="0eee2-155">Relationship</span></span>|<span data-ttu-id="0eee2-156">类型</span><span class="sxs-lookup"><span data-stu-id="0eee2-156">Type</span></span>|<span data-ttu-id="0eee2-157">说明</span><span class="sxs-lookup"><span data-stu-id="0eee2-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eee2-158">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0eee2-158">managedDevice</span></span>|[<span data-ttu-id="0eee2-159">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0eee2-159">managedDevice</span></span>](../resources/intune-shared-manageddevice.md)|<span data-ttu-id="0eee2-160">执行设备合规性脚本的托管设备</span><span class="sxs-lookup"><span data-stu-id="0eee2-160">The managed device on which the device compliance script executed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0eee2-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0eee2-161">JSON Representation</span></span>
<span data-ttu-id="0eee2-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0eee2-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "scriptOutput": "String",
  "scriptError": "String"
}
```




