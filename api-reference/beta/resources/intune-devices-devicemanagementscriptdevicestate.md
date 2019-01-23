---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备运行的设备管理脚本的状态属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8274a6dd5b38ee419738d250af0267533de6f00a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422472"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="a5a8f-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5a8f-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="a5a8f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5a8f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5a8f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5a8f-107">包含设备运行的设备管理脚本的状态属性。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-107">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="a5a8f-108">方法</span><span class="sxs-lookup"><span data-stu-id="a5a8f-108">Methods</span></span>
|<span data-ttu-id="a5a8f-109">方法</span><span class="sxs-lookup"><span data-stu-id="a5a8f-109">Method</span></span>|<span data-ttu-id="a5a8f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a5a8f-110">Return Type</span></span>|<span data-ttu-id="a5a8f-111">说明</span><span class="sxs-lookup"><span data-stu-id="a5a8f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a5a8f-112">列表 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="a5a8f-112">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="a5a8f-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="a5a8f-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="a5a8f-114">列出属性和[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-114">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="a5a8f-115">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-115">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="a5a8f-116">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-116">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="a5a8f-117">读取属性和[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-117">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="a5a8f-118">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-118">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="a5a8f-119">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-119">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="a5a8f-120">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-120">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="a5a8f-121">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-121">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="a5a8f-122">无</span><span class="sxs-lookup"><span data-stu-id="a5a8f-122">None</span></span>|<span data-ttu-id="a5a8f-123">删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-123">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="a5a8f-124">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-124">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="a5a8f-125">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-125">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="a5a8f-126">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-126">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5a8f-127">属性</span><span class="sxs-lookup"><span data-stu-id="a5a8f-127">Properties</span></span>
|<span data-ttu-id="a5a8f-128">属性</span><span class="sxs-lookup"><span data-stu-id="a5a8f-128">Property</span></span>|<span data-ttu-id="a5a8f-129">类型</span><span class="sxs-lookup"><span data-stu-id="a5a8f-129">Type</span></span>|<span data-ttu-id="a5a8f-130">说明</span><span class="sxs-lookup"><span data-stu-id="a5a8f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5a8f-131">id</span><span class="sxs-lookup"><span data-stu-id="a5a8f-131">id</span></span>|<span data-ttu-id="a5a8f-132">String</span><span class="sxs-lookup"><span data-stu-id="a5a8f-132">String</span></span>|<span data-ttu-id="a5a8f-133">设备管理脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-133">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="a5a8f-134">runState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-134">runState</span></span>|[<span data-ttu-id="a5a8f-135">runState</span><span class="sxs-lookup"><span data-stu-id="a5a8f-135">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="a5a8f-136">设备管理脚本的最新运行状态。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-136">State of latest run of the device management script.</span></span> <span data-ttu-id="a5a8f-137">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-137">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="a5a8f-138">resultMessage</span><span class="sxs-lookup"><span data-stu-id="a5a8f-138">resultMessage</span></span>|<span data-ttu-id="a5a8f-139">String</span><span class="sxs-lookup"><span data-stu-id="a5a8f-139">String</span></span>|<span data-ttu-id="a5a8f-140">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-140">Details of execution output.</span></span>|
|<span data-ttu-id="a5a8f-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a5a8f-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="a5a8f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5a8f-142">DateTimeOffset</span></span>|<span data-ttu-id="a5a8f-143">最新时间设备管理脚本执行。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-143">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="a5a8f-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="a5a8f-144">errorCode</span></span>|<span data-ttu-id="a5a8f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a5a8f-145">Int32</span></span>|<span data-ttu-id="a5a8f-146">错误代码对应的设备管理脚本错误执行。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-146">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="a5a8f-147">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a5a8f-147">errorDescription</span></span>|<span data-ttu-id="a5a8f-148">String</span><span class="sxs-lookup"><span data-stu-id="a5a8f-148">String</span></span>|<span data-ttu-id="a5a8f-149">设备管理脚本错误执行所对应的错误描述。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-149">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5a8f-150">关系</span><span class="sxs-lookup"><span data-stu-id="a5a8f-150">Relationships</span></span>
|<span data-ttu-id="a5a8f-151">关系</span><span class="sxs-lookup"><span data-stu-id="a5a8f-151">Relationship</span></span>|<span data-ttu-id="a5a8f-152">类型</span><span class="sxs-lookup"><span data-stu-id="a5a8f-152">Type</span></span>|<span data-ttu-id="a5a8f-153">说明</span><span class="sxs-lookup"><span data-stu-id="a5a8f-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5a8f-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="a5a8f-154">managedDevice</span></span>|[<span data-ttu-id="a5a8f-155">managedDevice</span><span class="sxs-lookup"><span data-stu-id="a5a8f-155">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="a5a8f-156">执行设备管理脚本托管的设备。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-156">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5a8f-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5a8f-157">JSON Representation</span></span>
<span data-ttu-id="a5a8f-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5a8f-158">Here is a JSON representation of the resource.</span></span>
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




