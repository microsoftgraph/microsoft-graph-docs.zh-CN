---
title: embeddedSIMDeviceState 资源类型
description: 描述与设备相关的嵌入的 SIM 激活代码部署状态。
author: tfitzmac
ms.openlocfilehash: ef7611e96b1b6f3bba0a3c59dead85ede41b2eda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308454"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="0b2ce-103">embeddedSIMDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b2ce-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="0b2ce-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b2ce-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b2ce-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b2ce-107">描述与设备相关的嵌入的 SIM 激活代码部署状态。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-107">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>
## <a name="methods"></a><span data-ttu-id="0b2ce-108">方法</span><span class="sxs-lookup"><span data-stu-id="0b2ce-108">Methods</span></span>
|<span data-ttu-id="0b2ce-109">方法</span><span class="sxs-lookup"><span data-stu-id="0b2ce-109">Method</span></span>|<span data-ttu-id="0b2ce-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b2ce-110">Return Type</span></span>|<span data-ttu-id="0b2ce-111">说明</span><span class="sxs-lookup"><span data-stu-id="0b2ce-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b2ce-112">列表 embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="0b2ce-112">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="0b2ce-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b2ce-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="0b2ce-114">列出属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-114">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="0b2ce-115">获取 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-115">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="0b2ce-116">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-116">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="0b2ce-117">读取属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-117">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0b2ce-118">创建 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-118">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="0b2ce-119">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-119">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="0b2ce-120">创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-120">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="0b2ce-121">删除 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-121">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="0b2ce-122">无</span><span class="sxs-lookup"><span data-stu-id="0b2ce-122">None</span></span>|<span data-ttu-id="0b2ce-123">删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-123">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="0b2ce-124">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-124">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="0b2ce-125">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0b2ce-125">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="0b2ce-126">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-126">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b2ce-127">属性</span><span class="sxs-lookup"><span data-stu-id="0b2ce-127">Properties</span></span>
|<span data-ttu-id="0b2ce-128">属性</span><span class="sxs-lookup"><span data-stu-id="0b2ce-128">Property</span></span>|<span data-ttu-id="0b2ce-129">类型</span><span class="sxs-lookup"><span data-stu-id="0b2ce-129">Type</span></span>|<span data-ttu-id="0b2ce-130">说明</span><span class="sxs-lookup"><span data-stu-id="0b2ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b2ce-131">id</span><span class="sxs-lookup"><span data-stu-id="0b2ce-131">id</span></span>|<span data-ttu-id="0b2ce-132">字符串</span><span class="sxs-lookup"><span data-stu-id="0b2ce-132">String</span></span>|<span data-ttu-id="0b2ce-133">嵌入 SIM 设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-133">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="0b2ce-134">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0b2ce-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b2ce-135">createdDateTime</span></span>|<span data-ttu-id="0b2ce-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b2ce-136">DateTimeOffset</span></span>|<span data-ttu-id="0b2ce-137">创建嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-137">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="0b2ce-138">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-138">Generated service side.</span></span>|
|<span data-ttu-id="0b2ce-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b2ce-139">modifiedDateTime</span></span>|<span data-ttu-id="0b2ce-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b2ce-140">DateTimeOffset</span></span>|<span data-ttu-id="0b2ce-141">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-141">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="0b2ce-142">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-142">Updated service side.</span></span>|
|<span data-ttu-id="0b2ce-143">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0b2ce-143">lastSyncDateTime</span></span>|<span data-ttu-id="0b2ce-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b2ce-144">DateTimeOffset</span></span>|<span data-ttu-id="0b2ce-145">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-145">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="0b2ce-146">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-146">Updated service side.</span></span>|
|<span data-ttu-id="0b2ce-147">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="0b2ce-147">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="0b2ce-148">字符串</span><span class="sxs-lookup"><span data-stu-id="0b2ce-148">String</span></span>|<span data-ttu-id="0b2ce-149">通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-149">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="0b2ce-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="0b2ce-150">deviceName</span></span>|<span data-ttu-id="0b2ce-151">String</span><span class="sxs-lookup"><span data-stu-id="0b2ce-151">String</span></span>|<span data-ttu-id="0b2ce-152">订阅已的设备名称设置如桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="0b2ce-152">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="0b2ce-153">userName</span><span class="sxs-lookup"><span data-stu-id="0b2ce-153">userName</span></span>|<span data-ttu-id="0b2ce-154">String</span><span class="sxs-lookup"><span data-stu-id="0b2ce-154">String</span></span>|<span data-ttu-id="0b2ce-155">订阅已设置到例如 joe@contoso.com 用户名</span><span class="sxs-lookup"><span data-stu-id="0b2ce-155">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="0b2ce-156">状态</span><span class="sxs-lookup"><span data-stu-id="0b2ce-156">state</span></span>|[<span data-ttu-id="0b2ce-157">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="0b2ce-157">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="0b2ce-158">应用于该设备配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-158">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="0b2ce-159">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-159">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="0b2ce-160">stateDetails</span><span class="sxs-lookup"><span data-stu-id="0b2ce-160">stateDetails</span></span>|<span data-ttu-id="0b2ce-161">字符串</span><span class="sxs-lookup"><span data-stu-id="0b2ce-161">String</span></span>|<span data-ttu-id="0b2ce-162">字符串设置状态的说明。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-162">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b2ce-163">Relationships</span><span class="sxs-lookup"><span data-stu-id="0b2ce-163">Relationships</span></span>
<span data-ttu-id="0b2ce-164">无</span><span class="sxs-lookup"><span data-stu-id="0b2ce-164">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b2ce-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b2ce-165">JSON Representation</span></span>
<span data-ttu-id="0b2ce-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b2ce-166">Here is a JSON representation of the resource.</span></span>
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





