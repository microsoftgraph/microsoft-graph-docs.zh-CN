---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90b9eaff6f291205acc559101e8ff4f64a33c8c8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611928"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="58573-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="58573-103">deviceManagementScriptDeviceState resource type</span></span>

<span data-ttu-id="58573-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58573-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58573-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58573-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58573-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58573-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58573-107">包含设备管理脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="58573-107">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="58573-108">方法</span><span class="sxs-lookup"><span data-stu-id="58573-108">Methods</span></span>
|<span data-ttu-id="58573-109">方法</span><span class="sxs-lookup"><span data-stu-id="58573-109">Method</span></span>|<span data-ttu-id="58573-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="58573-110">Return Type</span></span>|<span data-ttu-id="58573-111">Description</span><span class="sxs-lookup"><span data-stu-id="58573-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="58573-112">列出 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="58573-112">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="58573-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58573-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="58573-114">列出 [deviceManagementScriptDeviceState 对象的属性和](../resources/intune-devices-devicemanagementscriptdevicestate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="58573-114">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="58573-115">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-115">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="58573-116">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-116">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="58573-117">读取 [deviceManagementScriptDeviceState 对象的属性和](../resources/intune-devices-devicemanagementscriptdevicestate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="58573-117">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="58573-118">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-118">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="58573-119">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-119">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="58573-120">创建新的 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58573-120">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="58573-121">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-121">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="58573-122">无</span><span class="sxs-lookup"><span data-stu-id="58573-122">None</span></span>|<span data-ttu-id="58573-123">删除 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="58573-123">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="58573-124">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-124">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="58573-125">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="58573-125">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="58573-126">更新 [deviceManagementScriptDeviceState 对象](../resources/intune-devices-devicemanagementscriptdevicestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="58573-126">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="58573-127">属性</span><span class="sxs-lookup"><span data-stu-id="58573-127">Properties</span></span>
|<span data-ttu-id="58573-128">属性</span><span class="sxs-lookup"><span data-stu-id="58573-128">Property</span></span>|<span data-ttu-id="58573-129">类型</span><span class="sxs-lookup"><span data-stu-id="58573-129">Type</span></span>|<span data-ttu-id="58573-130">说明</span><span class="sxs-lookup"><span data-stu-id="58573-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58573-131">id</span><span class="sxs-lookup"><span data-stu-id="58573-131">id</span></span>|<span data-ttu-id="58573-132">String</span><span class="sxs-lookup"><span data-stu-id="58573-132">String</span></span>|<span data-ttu-id="58573-133">设备管理脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="58573-133">Key of the device management script device state entity.</span></span> <span data-ttu-id="58573-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="58573-134">This property is read-only.</span></span>|
|<span data-ttu-id="58573-135">runState</span><span class="sxs-lookup"><span data-stu-id="58573-135">runState</span></span>|[<span data-ttu-id="58573-136">runState</span><span class="sxs-lookup"><span data-stu-id="58573-136">runState</span></span>](../resources/intune-devices-runstate.md)|<span data-ttu-id="58573-137">设备管理脚本的最新运行状态。</span><span class="sxs-lookup"><span data-stu-id="58573-137">State of latest run of the device management script.</span></span> <span data-ttu-id="58573-138">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="58573-138">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="58573-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="58573-139">resultMessage</span></span>|<span data-ttu-id="58573-140">String</span><span class="sxs-lookup"><span data-stu-id="58573-140">String</span></span>|<span data-ttu-id="58573-141">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="58573-141">Details of execution output.</span></span>|
|<span data-ttu-id="58573-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="58573-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="58573-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58573-143">DateTimeOffset</span></span>|<span data-ttu-id="58573-144">设备管理脚本执行的最新时间。</span><span class="sxs-lookup"><span data-stu-id="58573-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="58573-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="58573-145">errorCode</span></span>|<span data-ttu-id="58573-146">Int32</span><span class="sxs-lookup"><span data-stu-id="58573-146">Int32</span></span>|<span data-ttu-id="58573-147">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="58573-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="58573-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="58573-148">errorDescription</span></span>|<span data-ttu-id="58573-149">String</span><span class="sxs-lookup"><span data-stu-id="58573-149">String</span></span>|<span data-ttu-id="58573-150">与设备管理脚本的错误执行相对应的错误描述。</span><span class="sxs-lookup"><span data-stu-id="58573-150">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58573-151">关系</span><span class="sxs-lookup"><span data-stu-id="58573-151">Relationships</span></span>
|<span data-ttu-id="58573-152">关系</span><span class="sxs-lookup"><span data-stu-id="58573-152">Relationship</span></span>|<span data-ttu-id="58573-153">类型</span><span class="sxs-lookup"><span data-stu-id="58573-153">Type</span></span>|<span data-ttu-id="58573-154">Description</span><span class="sxs-lookup"><span data-stu-id="58573-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58573-155">managedDevice</span><span class="sxs-lookup"><span data-stu-id="58573-155">managedDevice</span></span>|[<span data-ttu-id="58573-156">managedDevice</span><span class="sxs-lookup"><span data-stu-id="58573-156">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="58573-157">执行设备管理脚本的托管设备。</span><span class="sxs-lookup"><span data-stu-id="58573-157">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58573-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58573-158">JSON Representation</span></span>
<span data-ttu-id="58573-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58573-159">Here is a JSON representation of the resource.</span></span>
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
  "errorDescription": "String"
}
```




