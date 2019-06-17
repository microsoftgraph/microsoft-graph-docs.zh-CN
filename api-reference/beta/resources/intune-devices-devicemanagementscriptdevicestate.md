---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a6517f0dea1bac5219d7aa9d5e4158ea5bea8ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995327"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="4adc4-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="4adc4-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="4adc4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4adc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4adc4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4adc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4adc4-106">包含设备管理脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="4adc4-106">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="4adc4-107">方法</span><span class="sxs-lookup"><span data-stu-id="4adc4-107">Methods</span></span>
|<span data-ttu-id="4adc4-108">方法</span><span class="sxs-lookup"><span data-stu-id="4adc4-108">Method</span></span>|<span data-ttu-id="4adc4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4adc4-109">Return Type</span></span>|<span data-ttu-id="4adc4-110">说明</span><span class="sxs-lookup"><span data-stu-id="4adc4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4adc4-111">列出 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="4adc4-111">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="4adc4-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="4adc4-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="4adc4-113">列出[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4adc4-113">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="4adc4-114">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-114">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="4adc4-115">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-115">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="4adc4-116">读取[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4adc4-116">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="4adc4-117">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-117">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="4adc4-118">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-118">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="4adc4-119">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4adc4-119">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="4adc4-120">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-120">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="4adc4-121">无</span><span class="sxs-lookup"><span data-stu-id="4adc4-121">None</span></span>|<span data-ttu-id="4adc4-122">删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="4adc4-122">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="4adc4-123">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-123">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="4adc4-124">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4adc4-124">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="4adc4-125">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4adc4-125">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4adc4-126">属性</span><span class="sxs-lookup"><span data-stu-id="4adc4-126">Properties</span></span>
|<span data-ttu-id="4adc4-127">属性</span><span class="sxs-lookup"><span data-stu-id="4adc4-127">Property</span></span>|<span data-ttu-id="4adc4-128">类型</span><span class="sxs-lookup"><span data-stu-id="4adc4-128">Type</span></span>|<span data-ttu-id="4adc4-129">说明</span><span class="sxs-lookup"><span data-stu-id="4adc4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4adc4-130">id</span><span class="sxs-lookup"><span data-stu-id="4adc4-130">id</span></span>|<span data-ttu-id="4adc4-131">String</span><span class="sxs-lookup"><span data-stu-id="4adc4-131">String</span></span>|<span data-ttu-id="4adc4-132">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="4adc4-132">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="4adc4-133">runState</span><span class="sxs-lookup"><span data-stu-id="4adc4-133">runState</span></span>|[<span data-ttu-id="4adc4-134">runState</span><span class="sxs-lookup"><span data-stu-id="4adc4-134">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4adc4-135">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="4adc4-135">State of latest run of the device management script.</span></span> <span data-ttu-id="4adc4-136">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="4adc4-136">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="4adc4-137">resultMessage</span><span class="sxs-lookup"><span data-stu-id="4adc4-137">resultMessage</span></span>|<span data-ttu-id="4adc4-138">String</span><span class="sxs-lookup"><span data-stu-id="4adc4-138">String</span></span>|<span data-ttu-id="4adc4-139">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4adc4-139">Details of execution output.</span></span>|
|<span data-ttu-id="4adc4-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4adc4-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="4adc4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4adc4-141">DateTimeOffset</span></span>|<span data-ttu-id="4adc4-142">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="4adc4-142">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="4adc4-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="4adc4-143">errorCode</span></span>|<span data-ttu-id="4adc4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4adc4-144">Int32</span></span>|<span data-ttu-id="4adc4-145">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="4adc4-145">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="4adc4-146">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4adc4-146">errorDescription</span></span>|<span data-ttu-id="4adc4-147">String</span><span class="sxs-lookup"><span data-stu-id="4adc4-147">String</span></span>|<span data-ttu-id="4adc4-148">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="4adc4-148">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4adc4-149">关系</span><span class="sxs-lookup"><span data-stu-id="4adc4-149">Relationships</span></span>
|<span data-ttu-id="4adc4-150">关系</span><span class="sxs-lookup"><span data-stu-id="4adc4-150">Relationship</span></span>|<span data-ttu-id="4adc4-151">类型</span><span class="sxs-lookup"><span data-stu-id="4adc4-151">Type</span></span>|<span data-ttu-id="4adc4-152">说明</span><span class="sxs-lookup"><span data-stu-id="4adc4-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4adc4-153">managedDevice</span><span class="sxs-lookup"><span data-stu-id="4adc4-153">managedDevice</span></span>|[<span data-ttu-id="4adc4-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="4adc4-154">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="4adc4-155">执行设备管理脚本的托管设备。</span><span class="sxs-lookup"><span data-stu-id="4adc4-155">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4adc4-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4adc4-156">JSON Representation</span></span>
<span data-ttu-id="4adc4-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4adc4-157">Here is a JSON representation of the resource.</span></span>
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





