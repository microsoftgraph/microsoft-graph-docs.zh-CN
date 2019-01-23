---
title: embeddedSIMDeviceState 资源类型
description: 描述与设备相关的嵌入的 SIM 激活代码部署状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a79453c8d8bcb5682da64ce480f1a2f9f210a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415570"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="9445f-103">embeddedSIMDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="9445f-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="9445f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9445f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9445f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9445f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9445f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9445f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9445f-107">描述与设备相关的嵌入的 SIM 激活代码部署状态。</span><span class="sxs-lookup"><span data-stu-id="9445f-107">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>

## <a name="methods"></a><span data-ttu-id="9445f-108">方法</span><span class="sxs-lookup"><span data-stu-id="9445f-108">Methods</span></span>
|<span data-ttu-id="9445f-109">方法</span><span class="sxs-lookup"><span data-stu-id="9445f-109">Method</span></span>|<span data-ttu-id="9445f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9445f-110">Return Type</span></span>|<span data-ttu-id="9445f-111">说明</span><span class="sxs-lookup"><span data-stu-id="9445f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9445f-112">列表 embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="9445f-112">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="9445f-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="9445f-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="9445f-114">列出属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="9445f-114">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="9445f-115">获取 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-115">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="9445f-116">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-116">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="9445f-117">读取属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9445f-117">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="9445f-118">创建 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-118">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="9445f-119">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-119">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="9445f-120">创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9445f-120">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="9445f-121">删除 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-121">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="9445f-122">无</span><span class="sxs-lookup"><span data-stu-id="9445f-122">None</span></span>|<span data-ttu-id="9445f-123">删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="9445f-123">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="9445f-124">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-124">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="9445f-125">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="9445f-125">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="9445f-126">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9445f-126">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9445f-127">属性</span><span class="sxs-lookup"><span data-stu-id="9445f-127">Properties</span></span>
|<span data-ttu-id="9445f-128">属性</span><span class="sxs-lookup"><span data-stu-id="9445f-128">Property</span></span>|<span data-ttu-id="9445f-129">类型</span><span class="sxs-lookup"><span data-stu-id="9445f-129">Type</span></span>|<span data-ttu-id="9445f-130">说明</span><span class="sxs-lookup"><span data-stu-id="9445f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9445f-131">id</span><span class="sxs-lookup"><span data-stu-id="9445f-131">id</span></span>|<span data-ttu-id="9445f-132">String</span><span class="sxs-lookup"><span data-stu-id="9445f-132">String</span></span>|<span data-ttu-id="9445f-133">嵌入 SIM 设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9445f-133">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="9445f-134">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="9445f-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9445f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9445f-135">createdDateTime</span></span>|<span data-ttu-id="9445f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9445f-136">DateTimeOffset</span></span>|<span data-ttu-id="9445f-137">创建嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="9445f-137">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="9445f-138">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="9445f-138">Generated service side.</span></span>|
|<span data-ttu-id="9445f-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9445f-139">modifiedDateTime</span></span>|<span data-ttu-id="9445f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9445f-140">DateTimeOffset</span></span>|<span data-ttu-id="9445f-141">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="9445f-141">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="9445f-142">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="9445f-142">Updated service side.</span></span>|
|<span data-ttu-id="9445f-143">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9445f-143">lastSyncDateTime</span></span>|<span data-ttu-id="9445f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9445f-144">DateTimeOffset</span></span>|<span data-ttu-id="9445f-145">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="9445f-145">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="9445f-146">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="9445f-146">Updated service side.</span></span>|
|<span data-ttu-id="9445f-147">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="9445f-147">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="9445f-148">String</span><span class="sxs-lookup"><span data-stu-id="9445f-148">String</span></span>|<span data-ttu-id="9445f-149">通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。</span><span class="sxs-lookup"><span data-stu-id="9445f-149">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="9445f-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="9445f-150">deviceName</span></span>|<span data-ttu-id="9445f-151">String</span><span class="sxs-lookup"><span data-stu-id="9445f-151">String</span></span>|<span data-ttu-id="9445f-152">订阅已的设备名称设置如桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="9445f-152">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="9445f-153">userName</span><span class="sxs-lookup"><span data-stu-id="9445f-153">userName</span></span>|<span data-ttu-id="9445f-154">String</span><span class="sxs-lookup"><span data-stu-id="9445f-154">String</span></span>|<span data-ttu-id="9445f-155">订阅已设置到例如 joe@contoso.com 用户名</span><span class="sxs-lookup"><span data-stu-id="9445f-155">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="9445f-156">state</span><span class="sxs-lookup"><span data-stu-id="9445f-156">state</span></span>|[<span data-ttu-id="9445f-157">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="9445f-157">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="9445f-158">应用于该设备配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9445f-158">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="9445f-159">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="9445f-159">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="9445f-160">stateDetails</span><span class="sxs-lookup"><span data-stu-id="9445f-160">stateDetails</span></span>|<span data-ttu-id="9445f-161">String</span><span class="sxs-lookup"><span data-stu-id="9445f-161">String</span></span>|<span data-ttu-id="9445f-162">字符串设置状态的说明。</span><span class="sxs-lookup"><span data-stu-id="9445f-162">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9445f-163">关系</span><span class="sxs-lookup"><span data-stu-id="9445f-163">Relationships</span></span>
<span data-ttu-id="9445f-164">无</span><span class="sxs-lookup"><span data-stu-id="9445f-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9445f-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9445f-165">JSON Representation</span></span>
<span data-ttu-id="9445f-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9445f-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```




