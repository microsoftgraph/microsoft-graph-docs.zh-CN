---
title: embeddedSIMDeviceState 资源类型
description: 介绍与设备相关的嵌入的 SIM 激活代码部署状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358fb343282bdb30b43226a02fe127c73613dcc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151056"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="5e42b-103">embeddedSIMDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e42b-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="5e42b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e42b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e42b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e42b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e42b-106">介绍与设备相关的嵌入的 SIM 激活代码部署状态。</span><span class="sxs-lookup"><span data-stu-id="5e42b-106">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>

## <a name="methods"></a><span data-ttu-id="5e42b-107">方法</span><span class="sxs-lookup"><span data-stu-id="5e42b-107">Methods</span></span>
|<span data-ttu-id="5e42b-108">方法</span><span class="sxs-lookup"><span data-stu-id="5e42b-108">Method</span></span>|<span data-ttu-id="5e42b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e42b-109">Return Type</span></span>|<span data-ttu-id="5e42b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5e42b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e42b-111">列出 embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="5e42b-111">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="5e42b-112">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="5e42b-112">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="5e42b-113">列出[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e42b-113">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="5e42b-114">获取 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-114">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="5e42b-115">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-115">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="5e42b-116">读取[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e42b-116">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="5e42b-117">创建 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-117">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="5e42b-118">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-118">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="5e42b-119">创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e42b-119">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="5e42b-120">删除 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-120">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="5e42b-121">无</span><span class="sxs-lookup"><span data-stu-id="5e42b-121">None</span></span>|<span data-ttu-id="5e42b-122">删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="5e42b-122">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="5e42b-123">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-123">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="5e42b-124">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="5e42b-124">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="5e42b-125">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e42b-125">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e42b-126">属性</span><span class="sxs-lookup"><span data-stu-id="5e42b-126">Properties</span></span>
|<span data-ttu-id="5e42b-127">属性</span><span class="sxs-lookup"><span data-stu-id="5e42b-127">Property</span></span>|<span data-ttu-id="5e42b-128">类型</span><span class="sxs-lookup"><span data-stu-id="5e42b-128">Type</span></span>|<span data-ttu-id="5e42b-129">说明</span><span class="sxs-lookup"><span data-stu-id="5e42b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e42b-130">id</span><span class="sxs-lookup"><span data-stu-id="5e42b-130">id</span></span>|<span data-ttu-id="5e42b-131">字符串</span><span class="sxs-lookup"><span data-stu-id="5e42b-131">String</span></span>|<span data-ttu-id="5e42b-132">嵌入的 SIM 卡设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5e42b-132">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="5e42b-133">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="5e42b-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="5e42b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e42b-134">createdDateTime</span></span>|<span data-ttu-id="5e42b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e42b-135">DateTimeOffset</span></span>|<span data-ttu-id="5e42b-136">嵌入的 SIM 设备状态的创建时间。</span><span class="sxs-lookup"><span data-stu-id="5e42b-136">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="5e42b-137">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="5e42b-137">Generated service side.</span></span>|
|<span data-ttu-id="5e42b-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e42b-138">modifiedDateTime</span></span>|<span data-ttu-id="5e42b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e42b-139">DateTimeOffset</span></span>|<span data-ttu-id="5e42b-140">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="5e42b-140">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="5e42b-141">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="5e42b-141">Updated service side.</span></span>|
|<span data-ttu-id="5e42b-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5e42b-142">lastSyncDateTime</span></span>|<span data-ttu-id="5e42b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e42b-143">DateTimeOffset</span></span>|<span data-ttu-id="5e42b-144">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="5e42b-144">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="5e42b-145">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="5e42b-145">Updated service side.</span></span>|
|<span data-ttu-id="5e42b-146">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="5e42b-146">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="5e42b-147">字符串</span><span class="sxs-lookup"><span data-stu-id="5e42b-147">String</span></span>|<span data-ttu-id="5e42b-148">通用集成电路卡标识符 (UICCID), 用于标识要在其上部署配置文件的硬件。</span><span class="sxs-lookup"><span data-stu-id="5e42b-148">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="5e42b-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="5e42b-149">deviceName</span></span>|<span data-ttu-id="5e42b-150">String</span><span class="sxs-lookup"><span data-stu-id="5e42b-150">String</span></span>|<span data-ttu-id="5e42b-151">订阅预配到的设备名称, 例如, 桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="5e42b-151">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="5e42b-152">userName</span><span class="sxs-lookup"><span data-stu-id="5e42b-152">userName</span></span>|<span data-ttu-id="5e42b-153">字符串</span><span class="sxs-lookup"><span data-stu-id="5e42b-153">String</span></span>|<span data-ttu-id="5e42b-154">订阅预配到的用户名, 例如 joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="5e42b-154">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="5e42b-155">state</span><span class="sxs-lookup"><span data-stu-id="5e42b-155">state</span></span>|[<span data-ttu-id="5e42b-156">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="5e42b-156">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="5e42b-157">应用于设备的配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="5e42b-157">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="5e42b-158">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="5e42b-158">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="5e42b-159">stateDetails</span><span class="sxs-lookup"><span data-stu-id="5e42b-159">stateDetails</span></span>|<span data-ttu-id="5e42b-160">字符串</span><span class="sxs-lookup"><span data-stu-id="5e42b-160">String</span></span>|<span data-ttu-id="5e42b-161">设置状态的字符串说明。</span><span class="sxs-lookup"><span data-stu-id="5e42b-161">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e42b-162">关系</span><span class="sxs-lookup"><span data-stu-id="5e42b-162">Relationships</span></span>
<span data-ttu-id="5e42b-163">无</span><span class="sxs-lookup"><span data-stu-id="5e42b-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e42b-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e42b-164">JSON Representation</span></span>
<span data-ttu-id="5e42b-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e42b-165">Here is a JSON representation of the resource.</span></span>
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




