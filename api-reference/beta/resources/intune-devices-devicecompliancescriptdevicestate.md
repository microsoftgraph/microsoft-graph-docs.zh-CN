---
title: deviceComplianceScriptDeviceState 资源类型
description: 包含设备合规性脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5a3dcd3a1c79d33cfba11a0a04b2ef93f1a8f3c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734166"
---
# <a name="devicecompliancescriptdevicestate-resource-type"></a><span data-ttu-id="0fadb-103">deviceComplianceScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fadb-103">deviceComplianceScriptDeviceState resource type</span></span>

<span data-ttu-id="0fadb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fadb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fadb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fadb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fadb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fadb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fadb-107">包含设备合规性脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="0fadb-107">Contains properties for device run state of the device compliance script.</span></span>

## <a name="methods"></a><span data-ttu-id="0fadb-108">Methods</span><span class="sxs-lookup"><span data-stu-id="0fadb-108">Methods</span></span>
|<span data-ttu-id="0fadb-109">方法</span><span class="sxs-lookup"><span data-stu-id="0fadb-109">Method</span></span>|<span data-ttu-id="0fadb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fadb-110">Return Type</span></span>|<span data-ttu-id="0fadb-111">说明</span><span class="sxs-lookup"><span data-stu-id="0fadb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fadb-112">列出 deviceComplianceScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="0fadb-112">List deviceComplianceScriptDeviceStates</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-list.md)|<span data-ttu-id="0fadb-113">[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fadb-113">[deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) collection</span></span>|<span data-ttu-id="0fadb-114">列出 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fadb-114">List properties and relationships of the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="0fadb-115">获取 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-115">Get deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-get.md)|[<span data-ttu-id="0fadb-116">deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-116">deviceComplianceScriptDeviceState</span></span>](../resources/intune-devices-devicecompliancescriptdevicestate.md)|<span data-ttu-id="0fadb-117">读取 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fadb-117">Read properties and relationships of the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0fadb-118">创建 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-118">Create deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-create.md)|[<span data-ttu-id="0fadb-119">deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-119">deviceComplianceScriptDeviceState</span></span>](../resources/intune-devices-devicecompliancescriptdevicestate.md)|<span data-ttu-id="0fadb-120">创建新的 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fadb-120">Create a new [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0fadb-121">删除 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-121">Delete deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-delete.md)|<span data-ttu-id="0fadb-122">无</span><span class="sxs-lookup"><span data-stu-id="0fadb-122">None</span></span>|<span data-ttu-id="0fadb-123">删除 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="0fadb-123">Deletes a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md).</span></span>|
|[<span data-ttu-id="0fadb-124">更新 deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-124">Update deviceComplianceScriptDeviceState</span></span>](../api/intune-devices-devicecompliancescriptdevicestate-update.md)|[<span data-ttu-id="0fadb-125">deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="0fadb-125">deviceComplianceScriptDeviceState</span></span>](../resources/intune-devices-devicecompliancescriptdevicestate.md)|<span data-ttu-id="0fadb-126">更新 [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fadb-126">Update the properties of a [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fadb-127">属性</span><span class="sxs-lookup"><span data-stu-id="0fadb-127">Properties</span></span>
|<span data-ttu-id="0fadb-128">属性</span><span class="sxs-lookup"><span data-stu-id="0fadb-128">Property</span></span>|<span data-ttu-id="0fadb-129">类型</span><span class="sxs-lookup"><span data-stu-id="0fadb-129">Type</span></span>|<span data-ttu-id="0fadb-130">说明</span><span class="sxs-lookup"><span data-stu-id="0fadb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fadb-131">id</span><span class="sxs-lookup"><span data-stu-id="0fadb-131">id</span></span>|<span data-ttu-id="0fadb-132">String</span><span class="sxs-lookup"><span data-stu-id="0fadb-132">String</span></span>|<span data-ttu-id="0fadb-133">设备合规性脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fadb-133">Key of the device compliance script device state entity.</span></span> <span data-ttu-id="0fadb-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0fadb-134">This property is read-only.</span></span>|
|<span data-ttu-id="0fadb-135">detectionState</span><span class="sxs-lookup"><span data-stu-id="0fadb-135">detectionState</span></span>|[<span data-ttu-id="0fadb-136">runState</span><span class="sxs-lookup"><span data-stu-id="0fadb-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="0fadb-137">Lastest 设备合规性脚本执行中的检测状态。</span><span class="sxs-lookup"><span data-stu-id="0fadb-137">Detection state from the lastest device compliance script execution.</span></span> <span data-ttu-id="0fadb-138">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="0fadb-138">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="0fadb-139">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0fadb-139">lastStateUpdateDateTime</span></span>|<span data-ttu-id="0fadb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fadb-140">DateTimeOffset</span></span>|<span data-ttu-id="0fadb-141">执行设备符合性脚本的最后时间戳</span><span class="sxs-lookup"><span data-stu-id="0fadb-141">The last timestamp of when the device compliance script executed</span></span>|
|<span data-ttu-id="0fadb-142">expectedStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0fadb-142">expectedStateUpdateDateTime</span></span>|<span data-ttu-id="0fadb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fadb-143">DateTimeOffset</span></span>|<span data-ttu-id="0fadb-144">预期何时执行设备符合性脚本的下一个时间戳</span><span class="sxs-lookup"><span data-stu-id="0fadb-144">The next timestamp of when the device compliance script is expected to execute</span></span>|
|<span data-ttu-id="0fadb-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0fadb-145">lastSyncDateTime</span></span>|<span data-ttu-id="0fadb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fadb-146">DateTimeOffset</span></span>|<span data-ttu-id="0fadb-147">上次 Intune 管理扩展与 Intune 同步的时间</span><span class="sxs-lookup"><span data-stu-id="0fadb-147">The last time that Intune Managment Extension synced with Intune</span></span>|
|<span data-ttu-id="0fadb-148">scriptOutput</span><span class="sxs-lookup"><span data-stu-id="0fadb-148">scriptOutput</span></span>|<span data-ttu-id="0fadb-149">String</span><span class="sxs-lookup"><span data-stu-id="0fadb-149">String</span></span>|<span data-ttu-id="0fadb-150">检测脚本的输出</span><span class="sxs-lookup"><span data-stu-id="0fadb-150">Output of the detection script</span></span>|
|<span data-ttu-id="0fadb-151">scriptError</span><span class="sxs-lookup"><span data-stu-id="0fadb-151">scriptError</span></span>|<span data-ttu-id="0fadb-152">String</span><span class="sxs-lookup"><span data-stu-id="0fadb-152">String</span></span>|<span data-ttu-id="0fadb-153">检测脚本中的错误</span><span class="sxs-lookup"><span data-stu-id="0fadb-153">Error from the detection script</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fadb-154">关系</span><span class="sxs-lookup"><span data-stu-id="0fadb-154">Relationships</span></span>
|<span data-ttu-id="0fadb-155">关系</span><span class="sxs-lookup"><span data-stu-id="0fadb-155">Relationship</span></span>|<span data-ttu-id="0fadb-156">类型</span><span class="sxs-lookup"><span data-stu-id="0fadb-156">Type</span></span>|<span data-ttu-id="0fadb-157">说明</span><span class="sxs-lookup"><span data-stu-id="0fadb-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fadb-158">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0fadb-158">managedDevice</span></span>|[<span data-ttu-id="0fadb-159">managedDevice</span><span class="sxs-lookup"><span data-stu-id="0fadb-159">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="0fadb-160">在其上执行设备合规性脚本的托管设备</span><span class="sxs-lookup"><span data-stu-id="0fadb-160">The managed device on which the device compliance script executed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fadb-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fadb-161">JSON Representation</span></span>
<span data-ttu-id="0fadb-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fadb-162">Here is a JSON representation of the resource.</span></span>
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





