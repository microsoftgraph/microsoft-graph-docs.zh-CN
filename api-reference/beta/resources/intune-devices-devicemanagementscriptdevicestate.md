---
title: deviceManagementScriptDeviceState 资源类型
description: 包含设备运行的设备管理脚本的状态属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d67b7a43817864906984ce21c90536572b0747d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890536"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a><span data-ttu-id="14e4e-103">deviceManagementScriptDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="14e4e-103">deviceManagementScriptDeviceState resource type</span></span>

> <span data-ttu-id="14e4e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14e4e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14e4e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14e4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14e4e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="14e4e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14e4e-107">包含设备运行的设备管理脚本的状态属性。</span><span class="sxs-lookup"><span data-stu-id="14e4e-107">Contains properties for device run state of the device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="14e4e-108">方法</span><span class="sxs-lookup"><span data-stu-id="14e4e-108">Methods</span></span>
|<span data-ttu-id="14e4e-109">方法</span><span class="sxs-lookup"><span data-stu-id="14e4e-109">Method</span></span>|<span data-ttu-id="14e4e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="14e4e-110">Return Type</span></span>|<span data-ttu-id="14e4e-111">说明</span><span class="sxs-lookup"><span data-stu-id="14e4e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14e4e-112">列表 deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="14e4e-112">List deviceManagementScriptDeviceStates</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|<span data-ttu-id="14e4e-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="14e4e-113">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="14e4e-114">列出属性和[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="14e4e-114">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="14e4e-115">获取 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-115">Get deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[<span data-ttu-id="14e4e-116">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-116">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="14e4e-117">读取属性和[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="14e4e-117">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="14e4e-118">创建 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-118">Create deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[<span data-ttu-id="14e4e-119">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-119">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="14e4e-120">创建新的[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14e4e-120">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|
|[<span data-ttu-id="14e4e-121">删除 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-121">Delete deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|<span data-ttu-id="14e4e-122">无</span><span class="sxs-lookup"><span data-stu-id="14e4e-122">None</span></span>|<span data-ttu-id="14e4e-123">删除[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="14e4e-123">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>|
|[<span data-ttu-id="14e4e-124">更新 deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-124">Update deviceManagementScriptDeviceState</span></span>](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[<span data-ttu-id="14e4e-125">deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="14e4e-125">deviceManagementScriptDeviceState</span></span>](../resources/intune-devices-devicemanagementscriptdevicestate.md)|<span data-ttu-id="14e4e-126">更新[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="14e4e-126">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14e4e-127">属性</span><span class="sxs-lookup"><span data-stu-id="14e4e-127">Properties</span></span>
|<span data-ttu-id="14e4e-128">属性</span><span class="sxs-lookup"><span data-stu-id="14e4e-128">Property</span></span>|<span data-ttu-id="14e4e-129">类型</span><span class="sxs-lookup"><span data-stu-id="14e4e-129">Type</span></span>|<span data-ttu-id="14e4e-130">说明</span><span class="sxs-lookup"><span data-stu-id="14e4e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e4e-131">id</span><span class="sxs-lookup"><span data-stu-id="14e4e-131">id</span></span>|<span data-ttu-id="14e4e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="14e4e-132">String</span></span>|<span data-ttu-id="14e4e-133">设备管理脚本设备状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="14e4e-133">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="14e4e-134">runState</span><span class="sxs-lookup"><span data-stu-id="14e4e-134">runState</span></span>|[<span data-ttu-id="14e4e-135">runState</span><span class="sxs-lookup"><span data-stu-id="14e4e-135">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="14e4e-136">设备管理脚本的最新运行状态。</span><span class="sxs-lookup"><span data-stu-id="14e4e-136">State of latest run of the device management script.</span></span> <span data-ttu-id="14e4e-137">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="14e4e-137">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="14e4e-138">resultMessage</span><span class="sxs-lookup"><span data-stu-id="14e4e-138">resultMessage</span></span>|<span data-ttu-id="14e4e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="14e4e-139">String</span></span>|<span data-ttu-id="14e4e-140">执行输出的详细信息。</span><span class="sxs-lookup"><span data-stu-id="14e4e-140">Details of execution output.</span></span>|
|<span data-ttu-id="14e4e-141">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="14e4e-141">lastStateUpdateDateTime</span></span>|<span data-ttu-id="14e4e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14e4e-142">DateTimeOffset</span></span>|<span data-ttu-id="14e4e-143">最新时间设备管理脚本执行。</span><span class="sxs-lookup"><span data-stu-id="14e4e-143">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="14e4e-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="14e4e-144">errorCode</span></span>|<span data-ttu-id="14e4e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="14e4e-145">Int32</span></span>|<span data-ttu-id="14e4e-146">错误代码对应的设备管理脚本错误执行。</span><span class="sxs-lookup"><span data-stu-id="14e4e-146">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="14e4e-147">errorDescription</span><span class="sxs-lookup"><span data-stu-id="14e4e-147">errorDescription</span></span>|<span data-ttu-id="14e4e-148">String</span><span class="sxs-lookup"><span data-stu-id="14e4e-148">String</span></span>|<span data-ttu-id="14e4e-149">设备管理脚本错误执行所对应的错误描述。</span><span class="sxs-lookup"><span data-stu-id="14e4e-149">Error description corresponding to erroneous execution of the device management script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14e4e-150">Relationships</span><span class="sxs-lookup"><span data-stu-id="14e4e-150">Relationships</span></span>
|<span data-ttu-id="14e4e-151">关系</span><span class="sxs-lookup"><span data-stu-id="14e4e-151">Relationship</span></span>|<span data-ttu-id="14e4e-152">类型</span><span class="sxs-lookup"><span data-stu-id="14e4e-152">Type</span></span>|<span data-ttu-id="14e4e-153">Description</span><span class="sxs-lookup"><span data-stu-id="14e4e-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e4e-154">managedDevice</span><span class="sxs-lookup"><span data-stu-id="14e4e-154">managedDevice</span></span>|[<span data-ttu-id="14e4e-155">managedDevice</span><span class="sxs-lookup"><span data-stu-id="14e4e-155">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="14e4e-156">执行设备管理脚本托管的设备。</span><span class="sxs-lookup"><span data-stu-id="14e4e-156">The managed devices that executes the device management script.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14e4e-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14e4e-157">JSON Representation</span></span>
<span data-ttu-id="14e4e-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14e4e-158">Here is a JSON representation of the resource.</span></span>
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





