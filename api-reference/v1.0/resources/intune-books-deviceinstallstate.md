---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a7396adc2f6d39421b357a0fa409a52f6bc014c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468794"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="9dac4-103">deviceInstallState 资源类型</span><span class="sxs-lookup"><span data-stu-id="9dac4-103">deviceInstallState resource type</span></span>

<span data-ttu-id="9dac4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dac4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9dac4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9dac4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dac4-106">包含某个设备的安装状态的属性。</span><span class="sxs-lookup"><span data-stu-id="9dac4-106">Contains properties for the installation state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="9dac4-107">方法</span><span class="sxs-lookup"><span data-stu-id="9dac4-107">Methods</span></span>
|<span data-ttu-id="9dac4-108">方法</span><span class="sxs-lookup"><span data-stu-id="9dac4-108">Method</span></span>|<span data-ttu-id="9dac4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9dac4-109">Return Type</span></span>|<span data-ttu-id="9dac4-110">说明</span><span class="sxs-lookup"><span data-stu-id="9dac4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9dac4-111">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="9dac4-111">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="9dac4-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dac4-112">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9dac4-113">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9dac4-113">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="9dac4-114">获取 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-114">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="9dac4-115">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-115">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9dac4-116">读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9dac4-116">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="9dac4-117">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-117">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="9dac4-118">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-118">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9dac4-119">创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9dac4-119">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="9dac4-120">删除 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-120">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="9dac4-121">无</span><span class="sxs-lookup"><span data-stu-id="9dac4-121">None</span></span>|<span data-ttu-id="9dac4-122">删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。</span><span class="sxs-lookup"><span data-stu-id="9dac4-122">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="9dac4-123">更新 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-123">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="9dac4-124">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="9dac4-124">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="9dac4-125">更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9dac4-125">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9dac4-126">属性</span><span class="sxs-lookup"><span data-stu-id="9dac4-126">Properties</span></span>
|<span data-ttu-id="9dac4-127">属性</span><span class="sxs-lookup"><span data-stu-id="9dac4-127">Property</span></span>|<span data-ttu-id="9dac4-128">类型</span><span class="sxs-lookup"><span data-stu-id="9dac4-128">Type</span></span>|<span data-ttu-id="9dac4-129">说明</span><span class="sxs-lookup"><span data-stu-id="9dac4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dac4-130">id</span><span class="sxs-lookup"><span data-stu-id="9dac4-130">id</span></span>|<span data-ttu-id="9dac4-131">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-131">String</span></span>|<span data-ttu-id="9dac4-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9dac4-132">Key of the entity.</span></span>|
|<span data-ttu-id="9dac4-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="9dac4-133">deviceName</span></span>|<span data-ttu-id="9dac4-134">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-134">String</span></span>|<span data-ttu-id="9dac4-135">设备名称。</span><span class="sxs-lookup"><span data-stu-id="9dac4-135">Device name.</span></span>|
|<span data-ttu-id="9dac4-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="9dac4-136">deviceId</span></span>|<span data-ttu-id="9dac4-137">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-137">String</span></span>|<span data-ttu-id="9dac4-138">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="9dac4-138">Device Id.</span></span>|
|<span data-ttu-id="9dac4-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9dac4-139">lastSyncDateTime</span></span>|<span data-ttu-id="9dac4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dac4-140">DateTimeOffset</span></span>|<span data-ttu-id="9dac4-141">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9dac4-141">Last sync date and time.</span></span>|
|<span data-ttu-id="9dac4-142">installState</span><span class="sxs-lookup"><span data-stu-id="9dac4-142">installState</span></span>|[<span data-ttu-id="9dac4-143">installState</span><span class="sxs-lookup"><span data-stu-id="9dac4-143">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="9dac4-144">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="9dac4-144">The install state of the eBook.</span></span> <span data-ttu-id="9dac4-145">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="9dac4-145">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="9dac4-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="9dac4-146">errorCode</span></span>|<span data-ttu-id="9dac4-147">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-147">String</span></span>|<span data-ttu-id="9dac4-148">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9dac4-148">The error code for install failures.</span></span>|
|<span data-ttu-id="9dac4-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="9dac4-149">osVersion</span></span>|<span data-ttu-id="9dac4-150">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-150">String</span></span>|<span data-ttu-id="9dac4-151">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9dac4-151">OS Version.</span></span>|
|<span data-ttu-id="9dac4-152">osDescription</span><span class="sxs-lookup"><span data-stu-id="9dac4-152">osDescription</span></span>|<span data-ttu-id="9dac4-153">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-153">String</span></span>|<span data-ttu-id="9dac4-154">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="9dac4-154">OS Description.</span></span>|
|<span data-ttu-id="9dac4-155">userName</span><span class="sxs-lookup"><span data-stu-id="9dac4-155">userName</span></span>|<span data-ttu-id="9dac4-156">String</span><span class="sxs-lookup"><span data-stu-id="9dac4-156">String</span></span>|<span data-ttu-id="9dac4-157">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="9dac4-157">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dac4-158">关系</span><span class="sxs-lookup"><span data-stu-id="9dac4-158">Relationships</span></span>
<span data-ttu-id="9dac4-159">无</span><span class="sxs-lookup"><span data-stu-id="9dac4-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dac4-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9dac4-160">JSON Representation</span></span>
<span data-ttu-id="9dac4-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dac4-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```







