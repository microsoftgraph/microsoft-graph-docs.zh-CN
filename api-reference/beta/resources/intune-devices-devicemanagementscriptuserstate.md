---
title: deviceManagementScriptUserState 资源类型
description: 包含运行状态的设备管理脚本的用户的属性。
ms.openlocfilehash: 4e444c1eee438acba558a85e2a4ada14e44849bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049258"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="3085f-103">deviceManagementScriptUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="3085f-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="3085f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3085f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3085f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3085f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3085f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3085f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3085f-107">包含运行状态的设备管理脚本的用户的属性。</span><span class="sxs-lookup"><span data-stu-id="3085f-107">Contains properties for user run state of the device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="3085f-108">方法</span><span class="sxs-lookup"><span data-stu-id="3085f-108">Methods</span></span>
|<span data-ttu-id="3085f-109">方法</span><span class="sxs-lookup"><span data-stu-id="3085f-109">Method</span></span>|<span data-ttu-id="3085f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="3085f-110">Return Type</span></span>|<span data-ttu-id="3085f-111">说明</span><span class="sxs-lookup"><span data-stu-id="3085f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3085f-112">列表 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="3085f-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="3085f-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="3085f-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="3085f-114">列出属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="3085f-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="3085f-115">获取 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="3085f-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="3085f-117">读取属性和[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="3085f-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="3085f-118">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="3085f-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="3085f-120">创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3085f-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="3085f-121">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="3085f-122">无</span><span class="sxs-lookup"><span data-stu-id="3085f-122">None</span></span>|<span data-ttu-id="3085f-123">删除[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="3085f-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="3085f-124">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="3085f-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="3085f-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="3085f-126">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3085f-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3085f-127">属性</span><span class="sxs-lookup"><span data-stu-id="3085f-127">Properties</span></span>
|<span data-ttu-id="3085f-128">属性</span><span class="sxs-lookup"><span data-stu-id="3085f-128">Property</span></span>|<span data-ttu-id="3085f-129">类型</span><span class="sxs-lookup"><span data-stu-id="3085f-129">Type</span></span>|<span data-ttu-id="3085f-130">说明</span><span class="sxs-lookup"><span data-stu-id="3085f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3085f-131">id</span><span class="sxs-lookup"><span data-stu-id="3085f-131">id</span></span>|<span data-ttu-id="3085f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3085f-132">String</span></span>|<span data-ttu-id="3085f-133">设备管理脚本的用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="3085f-133">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="3085f-134">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3085f-134">successDeviceCount</span></span>|<span data-ttu-id="3085f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="3085f-135">Int32</span></span>|<span data-ttu-id="3085f-136">成功的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="3085f-136">Success device count for specific user.</span></span>|
|<span data-ttu-id="3085f-137">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3085f-137">errorDeviceCount</span></span>|<span data-ttu-id="3085f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3085f-138">Int32</span></span>|<span data-ttu-id="3085f-139">错误的特定用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="3085f-139">Error device count for specific user.</span></span>|
|<span data-ttu-id="3085f-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3085f-140">userPrincipalName</span></span>|<span data-ttu-id="3085f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3085f-141">String</span></span>|<span data-ttu-id="3085f-142">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="3085f-142">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3085f-143">Relationships</span><span class="sxs-lookup"><span data-stu-id="3085f-143">Relationships</span></span>
|<span data-ttu-id="3085f-144">关系</span><span class="sxs-lookup"><span data-stu-id="3085f-144">Relationship</span></span>|<span data-ttu-id="3085f-145">类型</span><span class="sxs-lookup"><span data-stu-id="3085f-145">Type</span></span>|<span data-ttu-id="3085f-146">说明</span><span class="sxs-lookup"><span data-stu-id="3085f-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3085f-147">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="3085f-147">deviceRunStates</span></span>|<span data-ttu-id="3085f-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="3085f-148">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="3085f-149">此脚本的特定用户的所有设备上的运行状态的列表。</span><span class="sxs-lookup"><span data-stu-id="3085f-149">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3085f-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3085f-150">JSON Representation</span></span>
<span data-ttu-id="3085f-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3085f-151">Here is a JSON representation of the resource.</span></span>
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





