---
title: embeddedSIMDeviceState 资源类型
description: 介绍与设备相关的嵌入的 SIM 激活代码部署状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b88fe5ada325e77b03bc83f2dcec5bb099c2f7d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442784"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="77f27-103">embeddedSIMDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="77f27-103">embeddedSIMDeviceState resource type</span></span>

<span data-ttu-id="77f27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77f27-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77f27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77f27-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77f27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f27-107">介绍与设备相关的嵌入的 SIM 激活代码部署状态。</span><span class="sxs-lookup"><span data-stu-id="77f27-107">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>

## <a name="methods"></a><span data-ttu-id="77f27-108">方法</span><span class="sxs-lookup"><span data-stu-id="77f27-108">Methods</span></span>
|<span data-ttu-id="77f27-109">方法</span><span class="sxs-lookup"><span data-stu-id="77f27-109">Method</span></span>|<span data-ttu-id="77f27-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="77f27-110">Return Type</span></span>|<span data-ttu-id="77f27-111">说明</span><span class="sxs-lookup"><span data-stu-id="77f27-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="77f27-112">列出 embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="77f27-112">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="77f27-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="77f27-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="77f27-114">列出[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77f27-114">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="77f27-115">获取 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-115">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="77f27-116">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-116">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="77f27-117">读取[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77f27-117">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="77f27-118">创建 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-118">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="77f27-119">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-119">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="77f27-120">创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="77f27-120">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="77f27-121">删除 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-121">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="77f27-122">无</span><span class="sxs-lookup"><span data-stu-id="77f27-122">None</span></span>|<span data-ttu-id="77f27-123">删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="77f27-123">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="77f27-124">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-124">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="77f27-125">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="77f27-125">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="77f27-126">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77f27-126">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="77f27-127">属性</span><span class="sxs-lookup"><span data-stu-id="77f27-127">Properties</span></span>
|<span data-ttu-id="77f27-128">属性</span><span class="sxs-lookup"><span data-stu-id="77f27-128">Property</span></span>|<span data-ttu-id="77f27-129">类型</span><span class="sxs-lookup"><span data-stu-id="77f27-129">Type</span></span>|<span data-ttu-id="77f27-130">说明</span><span class="sxs-lookup"><span data-stu-id="77f27-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f27-131">id</span><span class="sxs-lookup"><span data-stu-id="77f27-131">id</span></span>|<span data-ttu-id="77f27-132">String</span><span class="sxs-lookup"><span data-stu-id="77f27-132">String</span></span>|<span data-ttu-id="77f27-133">嵌入的 SIM 卡设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="77f27-133">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="77f27-134">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="77f27-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="77f27-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77f27-135">createdDateTime</span></span>|<span data-ttu-id="77f27-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f27-136">DateTimeOffset</span></span>|<span data-ttu-id="77f27-137">嵌入的 SIM 设备状态的创建时间。</span><span class="sxs-lookup"><span data-stu-id="77f27-137">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="77f27-138">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="77f27-138">Generated service side.</span></span>|
|<span data-ttu-id="77f27-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77f27-139">modifiedDateTime</span></span>|<span data-ttu-id="77f27-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f27-140">DateTimeOffset</span></span>|<span data-ttu-id="77f27-141">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="77f27-141">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="77f27-142">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="77f27-142">Updated service side.</span></span>|
|<span data-ttu-id="77f27-143">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="77f27-143">lastSyncDateTime</span></span>|<span data-ttu-id="77f27-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f27-144">DateTimeOffset</span></span>|<span data-ttu-id="77f27-145">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="77f27-145">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="77f27-146">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="77f27-146">Updated service side.</span></span>|
|<span data-ttu-id="77f27-147">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="77f27-147">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="77f27-148">String</span><span class="sxs-lookup"><span data-stu-id="77f27-148">String</span></span>|<span data-ttu-id="77f27-149">通用集成电路卡标识符（UICCID），用于标识要在其上部署配置文件的硬件。</span><span class="sxs-lookup"><span data-stu-id="77f27-149">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="77f27-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="77f27-150">deviceName</span></span>|<span data-ttu-id="77f27-151">String</span><span class="sxs-lookup"><span data-stu-id="77f27-151">String</span></span>|<span data-ttu-id="77f27-152">订阅预配到的设备名称，例如，桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="77f27-152">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="77f27-153">userName</span><span class="sxs-lookup"><span data-stu-id="77f27-153">userName</span></span>|<span data-ttu-id="77f27-154">String</span><span class="sxs-lookup"><span data-stu-id="77f27-154">String</span></span>|<span data-ttu-id="77f27-155">订阅预配到的用户名，例如 joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="77f27-155">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="77f27-156">state</span><span class="sxs-lookup"><span data-stu-id="77f27-156">state</span></span>|[<span data-ttu-id="77f27-157">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="77f27-157">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="77f27-158">应用于设备的配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="77f27-158">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="77f27-159">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="77f27-159">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="77f27-160">stateDetails</span><span class="sxs-lookup"><span data-stu-id="77f27-160">stateDetails</span></span>|<span data-ttu-id="77f27-161">String</span><span class="sxs-lookup"><span data-stu-id="77f27-161">String</span></span>|<span data-ttu-id="77f27-162">设置状态的字符串说明。</span><span class="sxs-lookup"><span data-stu-id="77f27-162">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f27-163">关系</span><span class="sxs-lookup"><span data-stu-id="77f27-163">Relationships</span></span>
<span data-ttu-id="77f27-164">无</span><span class="sxs-lookup"><span data-stu-id="77f27-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77f27-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77f27-165">JSON Representation</span></span>
<span data-ttu-id="77f27-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77f27-166">Here is a JSON representation of the resource.</span></span>
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



