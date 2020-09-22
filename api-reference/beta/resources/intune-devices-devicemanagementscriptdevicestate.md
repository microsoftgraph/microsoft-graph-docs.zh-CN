---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c8ab58f2fddc0030da42c85dbc10a4d8248aed0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060123"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="466e4-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="466e4-103">deviceManagementScriptDeviceState resource type</span></span>

<span data-ttu-id="466e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="466e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="466e4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="466e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="466e4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="466e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="466e4-107">包含设备管理脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="466e4-107">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="466e4-108">方法</span><span class="sxs-lookup"><span data-stu-id="466e4-108">Methods</span></span>
|<span data-ttu-id="466e4-109">方法</span><span class="sxs-lookup"><span data-stu-id="466e4-109">Method</span></span>|<span data-ttu-id="466e4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="466e4-110">Return Type</span></span>|<span data-ttu-id="466e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="466e4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="466e4-112">列出 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="466e4-112">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="466e4-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="466e4-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="466e4-114">列出 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="466e4-114">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="466e4-115">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-115">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="466e4-116">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-116">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="466e4-117">读取 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="466e4-117">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="466e4-118">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-118">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="466e4-119">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-119">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="466e4-120">创建新的 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="466e4-120">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="466e4-121">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-121">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="466e4-122">无</span><span class="sxs-lookup"><span data-stu-id="466e4-122">None</span></span>|<span data-ttu-id="466e4-123">删除 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="466e4-123">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="466e4-124">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-124">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="466e4-125">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="466e4-125">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="466e4-126">更新 [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="466e4-126">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="466e4-127">属性</span><span class="sxs-lookup"><span data-stu-id="466e4-127">Properties</span></span>
|<span data-ttu-id="466e4-128">属性</span><span class="sxs-lookup"><span data-stu-id="466e4-128">Property</span></span>|<span data-ttu-id="466e4-129">类型</span><span class="sxs-lookup"><span data-stu-id="466e4-129">Type</span></span>|<span data-ttu-id="466e4-130">说明</span><span class="sxs-lookup"><span data-stu-id="466e4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="466e4-131">id</span><span class="sxs-lookup"><span data-stu-id="466e4-131">id</span></span>|<span data-ttu-id="466e4-132">String</span><span class="sxs-lookup"><span data-stu-id="466e4-132">String</span></span>|<span data-ttu-id="466e4-133">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="466e4-133">Key of the device management script device state entity.</span></span> <span data-ttu-id="466e4-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="466e4-134">This property is read-only.</span></span>|
|<span data-ttu-id="466e4-135">runState</span><span class="sxs-lookup"><span data-stu-id="466e4-135">runState</span></span>|[<span data-ttu-id="466e4-136">runState</span><span class="sxs-lookup"><span data-stu-id="466e4-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="466e4-137">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="466e4-137">State of latest run of the device management script.</span></span> <span data-ttu-id="466e4-138">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="466e4-138">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="466e4-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="466e4-139">resultMessage</span></span>|<span data-ttu-id="466e4-140">String</span><span class="sxs-lookup"><span data-stu-id="466e4-140">String</span></span>|<span data-ttu-id="466e4-141">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="466e4-141">Details of execution output.</span></span>|
|<span data-ttu-id="466e4-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="466e4-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="466e4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="466e4-143">DateTimeOffset</span></span>|<span data-ttu-id="466e4-144">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="466e4-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="466e4-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="466e4-145">errorCode</span></span>|<span data-ttu-id="466e4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="466e4-146">Int32</span></span>|<span data-ttu-id="466e4-147">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="466e4-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="466e4-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="466e4-148">errorDescription</span></span>|<span data-ttu-id="466e4-149">String</span><span class="sxs-lookup"><span data-stu-id="466e4-149">String</span></span>|<span data-ttu-id="466e4-150">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="466e4-150">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="466e4-151">关系</span><span class="sxs-lookup"><span data-stu-id="466e4-151">Relationships</span></span>
|<span data-ttu-id="466e4-152">关系</span><span class="sxs-lookup"><span data-stu-id="466e4-152">Relationship</span></span>|<span data-ttu-id="466e4-153">类型</span><span class="sxs-lookup"><span data-stu-id="466e4-153">Type</span></span>|<span data-ttu-id="466e4-154">说明</span><span class="sxs-lookup"><span data-stu-id="466e4-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="466e4-155">managedDevice</span><span class="sxs-lookup"><span data-stu-id="466e4-155">managedDevice</span></span>|[<span data-ttu-id="466e4-156">managedDevice</span><span class="sxs-lookup"><span data-stu-id="466e4-156">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="466e4-157">执行设备管理脚本的托管设备。</span><span class="sxs-lookup"><span data-stu-id="466e4-157">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="466e4-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="466e4-158">JSON Representation</span></span>
<span data-ttu-id="466e4-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="466e4-159">Here is a JSON representation of the resource.</span></span>
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






