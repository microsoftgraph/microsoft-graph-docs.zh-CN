---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备管理脚本的设备运行状态的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b985b7641d66c806acc544174fffff4a2216421a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522438"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="b3451-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3451-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="b3451-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3451-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3451-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3451-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3451-106">包含设备管理脚本的设备运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="b3451-106">Contains properties for device run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="b3451-107">方法</span><span class="sxs-lookup"><span data-stu-id="b3451-107">Methods</span></span>
|<span data-ttu-id="b3451-108">方法</span><span class="sxs-lookup"><span data-stu-id="b3451-108">Method</span></span>|<span data-ttu-id="b3451-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3451-109">Return Type</span></span>|<span data-ttu-id="b3451-110">说明</span><span class="sxs-lookup"><span data-stu-id="b3451-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3451-111">列出 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="b3451-111">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="b3451-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3451-112">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="b3451-113">列出[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3451-113">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="b3451-114">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-114">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="b3451-115">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-115">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="b3451-116">读取[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3451-116">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="b3451-117">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-117">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="b3451-118">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-118">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="b3451-119">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3451-119">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="b3451-120">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-120">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="b3451-121">无</span><span class="sxs-lookup"><span data-stu-id="b3451-121">None</span></span>|<span data-ttu-id="b3451-122">删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="b3451-122">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="b3451-123">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-123">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="b3451-124">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="b3451-124">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="b3451-125">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3451-125">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3451-126">属性</span><span class="sxs-lookup"><span data-stu-id="b3451-126">Properties</span></span>
|<span data-ttu-id="b3451-127">属性</span><span class="sxs-lookup"><span data-stu-id="b3451-127">Property</span></span>|<span data-ttu-id="b3451-128">类型</span><span class="sxs-lookup"><span data-stu-id="b3451-128">Type</span></span>|<span data-ttu-id="b3451-129">说明</span><span class="sxs-lookup"><span data-stu-id="b3451-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3451-130">id</span><span class="sxs-lookup"><span data-stu-id="b3451-130">id</span></span>|<span data-ttu-id="b3451-131">String</span><span class="sxs-lookup"><span data-stu-id="b3451-131">String</span></span>|<span data-ttu-id="b3451-132">设备管理脚本设备状态实体的密钥。</span><span class="sxs-lookup"><span data-stu-id="b3451-132">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="b3451-133">runState</span><span class="sxs-lookup"><span data-stu-id="b3451-133">runState</span></span>|[<span data-ttu-id="b3451-134">runState</span><span class="sxs-lookup"><span data-stu-id="b3451-134">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="b3451-135">设备管理脚本最新运行的状态。</span><span class="sxs-lookup"><span data-stu-id="b3451-135">State of latest run of the device management script.</span></span> <span data-ttu-id="b3451-136">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="b3451-136">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="b3451-137">resultMessage</span><span class="sxs-lookup"><span data-stu-id="b3451-137">resultMessage</span></span>|<span data-ttu-id="b3451-138">String</span><span class="sxs-lookup"><span data-stu-id="b3451-138">String</span></span>|<span data-ttu-id="b3451-139">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b3451-139">Details of execution output.</span></span>|
|<span data-ttu-id="b3451-140">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b3451-140">lastStateUpdateDateTime</span></span>|<span data-ttu-id="b3451-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3451-141">DateTimeOffset</span></span>|<span data-ttu-id="b3451-142">最近执行设备管理脚本的时间。</span><span class="sxs-lookup"><span data-stu-id="b3451-142">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="b3451-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="b3451-143">errorCode</span></span>|<span data-ttu-id="b3451-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b3451-144">Int32</span></span>|<span data-ttu-id="b3451-145">与设备管理脚本的错误执行相对应的错误代码。</span><span class="sxs-lookup"><span data-stu-id="b3451-145">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="b3451-146">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b3451-146">errorDescription</span></span>|<span data-ttu-id="b3451-147">String</span><span class="sxs-lookup"><span data-stu-id="b3451-147">String</span></span>|<span data-ttu-id="b3451-148">与设备管理脚本的错误执行相对应的错误说明。</span><span class="sxs-lookup"><span data-stu-id="b3451-148">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3451-149">关系</span><span class="sxs-lookup"><span data-stu-id="b3451-149">Relationships</span></span>
|<span data-ttu-id="b3451-150">关系</span><span class="sxs-lookup"><span data-stu-id="b3451-150">Relationship</span></span>|<span data-ttu-id="b3451-151">类型</span><span class="sxs-lookup"><span data-stu-id="b3451-151">Type</span></span>|<span data-ttu-id="b3451-152">说明</span><span class="sxs-lookup"><span data-stu-id="b3451-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3451-153">managedDevice</span><span class="sxs-lookup"><span data-stu-id="b3451-153">managedDevice</span></span>|[<span data-ttu-id="b3451-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="b3451-154">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="b3451-155">执行设备管理脚本的托管设备。</span><span class="sxs-lookup"><span data-stu-id="b3451-155">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3451-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3451-156">JSON Representation</span></span>
<span data-ttu-id="b3451-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3451-157">Here is a JSON representation of the resource.</span></span>
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





