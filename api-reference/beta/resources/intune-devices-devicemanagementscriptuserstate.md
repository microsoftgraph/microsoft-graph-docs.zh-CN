---
title: deviceManagementScriptUserState 资源类型
description: 包含运行状态的设备管理脚本的用户的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1884967707be8e126724148afa5d04b07f80a48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407282"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="e36da-103">deviceManagementScriptUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e36da-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="e36da-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e36da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e36da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e36da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e36da-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e36da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e36da-107">包含运行状态的设备管理脚本的用户的属性。</span><span class="sxs-lookup"><span data-stu-id="e36da-107">Contains properties for user run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="e36da-108">方法</span><span class="sxs-lookup"><span data-stu-id="e36da-108">Methods</span></span>
|<span data-ttu-id="e36da-109">方法</span><span class="sxs-lookup"><span data-stu-id="e36da-109">Method</span></span>|<span data-ttu-id="e36da-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e36da-110">Return Type</span></span>|<span data-ttu-id="e36da-111">说明</span><span class="sxs-lookup"><span data-stu-id="e36da-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e36da-112">列表 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="e36da-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="e36da-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e36da-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="e36da-114">列出属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e36da-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="e36da-115">获取 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="e36da-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="e36da-117">读取属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e36da-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="e36da-118">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="e36da-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="e36da-120">创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e36da-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="e36da-121">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="e36da-122">无</span><span class="sxs-lookup"><span data-stu-id="e36da-122">None</span></span>|<span data-ttu-id="e36da-123">删除[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="e36da-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="e36da-124">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="e36da-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="e36da-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="e36da-126">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e36da-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e36da-127">属性</span><span class="sxs-lookup"><span data-stu-id="e36da-127">Properties</span></span>
|<span data-ttu-id="e36da-128">属性</span><span class="sxs-lookup"><span data-stu-id="e36da-128">Property</span></span>|<span data-ttu-id="e36da-129">类型</span><span class="sxs-lookup"><span data-stu-id="e36da-129">Type</span></span>|<span data-ttu-id="e36da-130">说明</span><span class="sxs-lookup"><span data-stu-id="e36da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e36da-131">id</span><span class="sxs-lookup"><span data-stu-id="e36da-131">id</span></span>|<span data-ttu-id="e36da-132">String</span><span class="sxs-lookup"><span data-stu-id="e36da-132">String</span></span>|<span data-ttu-id="e36da-133">设备管理脚本的用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="e36da-133">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="e36da-134">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e36da-134">successDeviceCount</span></span>|<span data-ttu-id="e36da-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e36da-135">Int32</span></span>|<span data-ttu-id="e36da-136">成功的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="e36da-136">Success device count for specific user.</span></span>|
|<span data-ttu-id="e36da-137">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e36da-137">errorDeviceCount</span></span>|<span data-ttu-id="e36da-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e36da-138">Int32</span></span>|<span data-ttu-id="e36da-139">错误的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="e36da-139">Error device count for specific user.</span></span>|
|<span data-ttu-id="e36da-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e36da-140">userPrincipalName</span></span>|<span data-ttu-id="e36da-141">String</span><span class="sxs-lookup"><span data-stu-id="e36da-141">String</span></span>|<span data-ttu-id="e36da-142">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e36da-142">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e36da-143">关系</span><span class="sxs-lookup"><span data-stu-id="e36da-143">Relationships</span></span>
|<span data-ttu-id="e36da-144">关系</span><span class="sxs-lookup"><span data-stu-id="e36da-144">Relationship</span></span>|<span data-ttu-id="e36da-145">类型</span><span class="sxs-lookup"><span data-stu-id="e36da-145">Type</span></span>|<span data-ttu-id="e36da-146">说明</span><span class="sxs-lookup"><span data-stu-id="e36da-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e36da-147">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="e36da-147">deviceRunStates</span></span>|<span data-ttu-id="e36da-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e36da-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="e36da-149">此脚本的特定用户的所有设备上的运行状态的列表。</span><span class="sxs-lookup"><span data-stu-id="e36da-149">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e36da-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e36da-150">JSON Representation</span></span>
<span data-ttu-id="e36da-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e36da-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```




