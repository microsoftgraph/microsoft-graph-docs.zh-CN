---
title: deviceManagementScriptUserState 资源类型
description: 包含设备管理脚本的用户运行状态的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed4ffab0a8fc77bfb14814961aeacc1bfe4955b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528607"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="c97d5-103">deviceManagementScriptUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c97d5-103">deviceManagementScriptUserState resource type</span></span>

<span data-ttu-id="c97d5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c97d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c97d5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c97d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c97d5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c97d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c97d5-107">包含设备管理脚本的用户运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="c97d5-107">Contains properties for user run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="c97d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="c97d5-108">Methods</span></span>
|<span data-ttu-id="c97d5-109">方法</span><span class="sxs-lookup"><span data-stu-id="c97d5-109">Method</span></span>|<span data-ttu-id="c97d5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c97d5-110">Return Type</span></span>|<span data-ttu-id="c97d5-111">说明</span><span class="sxs-lookup"><span data-stu-id="c97d5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c97d5-112">列出 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="c97d5-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="c97d5-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c97d5-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="c97d5-114">列出[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c97d5-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="c97d5-115">获取 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="c97d5-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="c97d5-117">读取[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c97d5-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="c97d5-118">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="c97d5-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="c97d5-120">创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c97d5-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="c97d5-121">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="c97d5-122">无</span><span class="sxs-lookup"><span data-stu-id="c97d5-122">None</span></span>|<span data-ttu-id="c97d5-123">删除[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="c97d5-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="c97d5-124">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="c97d5-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="c97d5-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="c97d5-126">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c97d5-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c97d5-127">属性</span><span class="sxs-lookup"><span data-stu-id="c97d5-127">Properties</span></span>
|<span data-ttu-id="c97d5-128">属性</span><span class="sxs-lookup"><span data-stu-id="c97d5-128">Property</span></span>|<span data-ttu-id="c97d5-129">类型</span><span class="sxs-lookup"><span data-stu-id="c97d5-129">Type</span></span>|<span data-ttu-id="c97d5-130">说明</span><span class="sxs-lookup"><span data-stu-id="c97d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97d5-131">id</span><span class="sxs-lookup"><span data-stu-id="c97d5-131">id</span></span>|<span data-ttu-id="c97d5-132">String</span><span class="sxs-lookup"><span data-stu-id="c97d5-132">String</span></span>|<span data-ttu-id="c97d5-133">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="c97d5-133">Key of the device management script user state entity.</span></span> <span data-ttu-id="c97d5-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c97d5-134">This property is read-only.</span></span>|
|<span data-ttu-id="c97d5-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c97d5-135">successDeviceCount</span></span>|<span data-ttu-id="c97d5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c97d5-136">Int32</span></span>|<span data-ttu-id="c97d5-137">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="c97d5-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="c97d5-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c97d5-138">errorDeviceCount</span></span>|<span data-ttu-id="c97d5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c97d5-139">Int32</span></span>|<span data-ttu-id="c97d5-140">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="c97d5-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="c97d5-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c97d5-141">userPrincipalName</span></span>|<span data-ttu-id="c97d5-142">String</span><span class="sxs-lookup"><span data-stu-id="c97d5-142">String</span></span>|<span data-ttu-id="c97d5-143">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c97d5-143">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c97d5-144">关系</span><span class="sxs-lookup"><span data-stu-id="c97d5-144">Relationships</span></span>
|<span data-ttu-id="c97d5-145">关系</span><span class="sxs-lookup"><span data-stu-id="c97d5-145">Relationship</span></span>|<span data-ttu-id="c97d5-146">类型</span><span class="sxs-lookup"><span data-stu-id="c97d5-146">Type</span></span>|<span data-ttu-id="c97d5-147">说明</span><span class="sxs-lookup"><span data-stu-id="c97d5-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97d5-148">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="c97d5-148">deviceRunStates</span></span>|<span data-ttu-id="c97d5-149">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c97d5-149">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="c97d5-150">此脚本在特定用户的所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="c97d5-150">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c97d5-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c97d5-151">JSON Representation</span></span>
<span data-ttu-id="c97d5-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c97d5-152">Here is a JSON representation of the resource.</span></span>
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



