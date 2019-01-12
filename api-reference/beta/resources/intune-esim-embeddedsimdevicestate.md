---
title: embeddedSIMDeviceState 资源类型
description: 描述与设备相关的嵌入的 SIM 激活代码部署状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce96250b8c64fc97171ee7721ca44b4cd4579072
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912622"
---
# <a name="embeddedsimdevicestate-resource-type"></a><span data-ttu-id="912d2-103">embeddedSIMDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="912d2-103">embeddedSIMDeviceState resource type</span></span>

> <span data-ttu-id="912d2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="912d2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="912d2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="912d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="912d2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="912d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="912d2-107">描述与设备相关的嵌入的 SIM 激活代码部署状态。</span><span class="sxs-lookup"><span data-stu-id="912d2-107">Describes the embedded SIM activation code deployment state in relation to a device.</span></span>
## <a name="methods"></a><span data-ttu-id="912d2-108">方法</span><span class="sxs-lookup"><span data-stu-id="912d2-108">Methods</span></span>
|<span data-ttu-id="912d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="912d2-109">Method</span></span>|<span data-ttu-id="912d2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="912d2-110">Return Type</span></span>|<span data-ttu-id="912d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="912d2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="912d2-112">列表 embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="912d2-112">List embeddedSIMDeviceStates</span></span>](../api/intune-esim-embeddedsimdevicestate-list.md)|<span data-ttu-id="912d2-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="912d2-113">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) collection</span></span>|<span data-ttu-id="912d2-114">列出属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="912d2-114">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="912d2-115">获取 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-115">Get embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-get.md)|[<span data-ttu-id="912d2-116">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-116">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="912d2-117">读取属性和[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="912d2-117">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="912d2-118">创建 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-118">Create embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-create.md)|[<span data-ttu-id="912d2-119">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-119">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="912d2-120">创建新的[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="912d2-120">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|
|[<span data-ttu-id="912d2-121">删除 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-121">Delete embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-delete.md)|<span data-ttu-id="912d2-122">无</span><span class="sxs-lookup"><span data-stu-id="912d2-122">None</span></span>|<span data-ttu-id="912d2-123">删除[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="912d2-123">Deletes a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>|
|[<span data-ttu-id="912d2-124">更新 embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-124">Update embeddedSIMDeviceState</span></span>](../api/intune-esim-embeddedsimdevicestate-update.md)|[<span data-ttu-id="912d2-125">embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="912d2-125">embeddedSIMDeviceState</span></span>](../resources/intune-esim-embeddedsimdevicestate.md)|<span data-ttu-id="912d2-126">更新[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="912d2-126">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="912d2-127">属性</span><span class="sxs-lookup"><span data-stu-id="912d2-127">Properties</span></span>
|<span data-ttu-id="912d2-128">属性</span><span class="sxs-lookup"><span data-stu-id="912d2-128">Property</span></span>|<span data-ttu-id="912d2-129">类型</span><span class="sxs-lookup"><span data-stu-id="912d2-129">Type</span></span>|<span data-ttu-id="912d2-130">说明</span><span class="sxs-lookup"><span data-stu-id="912d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="912d2-131">id</span><span class="sxs-lookup"><span data-stu-id="912d2-131">id</span></span>|<span data-ttu-id="912d2-132">字符串</span><span class="sxs-lookup"><span data-stu-id="912d2-132">String</span></span>|<span data-ttu-id="912d2-133">嵌入 SIM 设备状态的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="912d2-133">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="912d2-134">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="912d2-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="912d2-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="912d2-135">createdDateTime</span></span>|<span data-ttu-id="912d2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="912d2-136">DateTimeOffset</span></span>|<span data-ttu-id="912d2-137">创建嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="912d2-137">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="912d2-138">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="912d2-138">Generated service side.</span></span>|
|<span data-ttu-id="912d2-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="912d2-139">modifiedDateTime</span></span>|<span data-ttu-id="912d2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="912d2-140">DateTimeOffset</span></span>|<span data-ttu-id="912d2-141">上次修改嵌入的 SIM 设备状态的时间。</span><span class="sxs-lookup"><span data-stu-id="912d2-141">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="912d2-142">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="912d2-142">Updated service side.</span></span>|
|<span data-ttu-id="912d2-143">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="912d2-143">lastSyncDateTime</span></span>|<span data-ttu-id="912d2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="912d2-144">DateTimeOffset</span></span>|<span data-ttu-id="912d2-145">嵌入的 SIM 设备上次签入的时间。</span><span class="sxs-lookup"><span data-stu-id="912d2-145">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="912d2-146">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="912d2-146">Updated service side.</span></span>|
|<span data-ttu-id="912d2-147">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="912d2-147">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="912d2-148">字符串</span><span class="sxs-lookup"><span data-stu-id="912d2-148">String</span></span>|<span data-ttu-id="912d2-149">通用集成电路卡标识符 (UICCID) 标识到配置文件是要部署的硬件。</span><span class="sxs-lookup"><span data-stu-id="912d2-149">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="912d2-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="912d2-150">deviceName</span></span>|<span data-ttu-id="912d2-151">String</span><span class="sxs-lookup"><span data-stu-id="912d2-151">String</span></span>|<span data-ttu-id="912d2-152">订阅已的设备名称设置如桌面 JOE</span><span class="sxs-lookup"><span data-stu-id="912d2-152">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="912d2-153">userName</span><span class="sxs-lookup"><span data-stu-id="912d2-153">userName</span></span>|<span data-ttu-id="912d2-154">String</span><span class="sxs-lookup"><span data-stu-id="912d2-154">String</span></span>|<span data-ttu-id="912d2-155">订阅已设置到例如 joe@contoso.com 用户名</span><span class="sxs-lookup"><span data-stu-id="912d2-155">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="912d2-156">state</span><span class="sxs-lookup"><span data-stu-id="912d2-156">state</span></span>|[<span data-ttu-id="912d2-157">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="912d2-157">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="912d2-158">应用于该设备配置文件操作的状态。</span><span class="sxs-lookup"><span data-stu-id="912d2-158">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="912d2-159">可取值为：`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser`。</span><span class="sxs-lookup"><span data-stu-id="912d2-159">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="912d2-160">stateDetails</span><span class="sxs-lookup"><span data-stu-id="912d2-160">stateDetails</span></span>|<span data-ttu-id="912d2-161">字符串</span><span class="sxs-lookup"><span data-stu-id="912d2-161">String</span></span>|<span data-ttu-id="912d2-162">字符串设置状态的说明。</span><span class="sxs-lookup"><span data-stu-id="912d2-162">String description of the provisioning state.</span></span>|

## <a name="relationships"></a><span data-ttu-id="912d2-163">Relationships</span><span class="sxs-lookup"><span data-stu-id="912d2-163">Relationships</span></span>
<span data-ttu-id="912d2-164">无</span><span class="sxs-lookup"><span data-stu-id="912d2-164">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="912d2-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="912d2-165">JSON Representation</span></span>
<span data-ttu-id="912d2-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="912d2-166">Here is a JSON representation of the resource.</span></span>
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





