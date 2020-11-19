---
title: deviceManagementScriptUserState 资源类型
description: 包含设备管理脚本的用户运行状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fdf91765d6387a735439ad4bcf66f568f3944ab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267598"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="f33fb-103">deviceManagementScriptUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f33fb-103">deviceManagementScriptUserState resource type</span></span>

<span data-ttu-id="f33fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f33fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f33fb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f33fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f33fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f33fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f33fb-107">包含设备管理脚本的用户运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="f33fb-107">Contains properties for user run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="f33fb-108">方法</span><span class="sxs-lookup"><span data-stu-id="f33fb-108">Methods</span></span>
|<span data-ttu-id="f33fb-109">方法</span><span class="sxs-lookup"><span data-stu-id="f33fb-109">Method</span></span>|<span data-ttu-id="f33fb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f33fb-110">Return Type</span></span>|<span data-ttu-id="f33fb-111">说明</span><span class="sxs-lookup"><span data-stu-id="f33fb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f33fb-112">列出 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="f33fb-112">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="f33fb-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f33fb-113">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="f33fb-114">列出 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f33fb-114">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="f33fb-115">获取 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-115">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="f33fb-116">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-116">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="f33fb-117">读取 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f33fb-117">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="f33fb-118">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-118">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="f33fb-119">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-119">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="f33fb-120">创建新的 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f33fb-120">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="f33fb-121">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-121">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="f33fb-122">无</span><span class="sxs-lookup"><span data-stu-id="f33fb-122">None</span></span>|<span data-ttu-id="f33fb-123">删除 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="f33fb-123">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="f33fb-124">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-124">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="f33fb-125">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="f33fb-125">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="f33fb-126">更新 [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f33fb-126">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f33fb-127">属性</span><span class="sxs-lookup"><span data-stu-id="f33fb-127">Properties</span></span>
|<span data-ttu-id="f33fb-128">属性</span><span class="sxs-lookup"><span data-stu-id="f33fb-128">Property</span></span>|<span data-ttu-id="f33fb-129">类型</span><span class="sxs-lookup"><span data-stu-id="f33fb-129">Type</span></span>|<span data-ttu-id="f33fb-130">说明</span><span class="sxs-lookup"><span data-stu-id="f33fb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f33fb-131">id</span><span class="sxs-lookup"><span data-stu-id="f33fb-131">id</span></span>|<span data-ttu-id="f33fb-132">字符串</span><span class="sxs-lookup"><span data-stu-id="f33fb-132">String</span></span>|<span data-ttu-id="f33fb-133">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="f33fb-133">Key of the device management script user state entity.</span></span> <span data-ttu-id="f33fb-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f33fb-134">This property is read-only.</span></span>|
|<span data-ttu-id="f33fb-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f33fb-135">successDeviceCount</span></span>|<span data-ttu-id="f33fb-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f33fb-136">Int32</span></span>|<span data-ttu-id="f33fb-137">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="f33fb-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="f33fb-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f33fb-138">errorDeviceCount</span></span>|<span data-ttu-id="f33fb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f33fb-139">Int32</span></span>|<span data-ttu-id="f33fb-140">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="f33fb-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="f33fb-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f33fb-141">userPrincipalName</span></span>|<span data-ttu-id="f33fb-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f33fb-142">String</span></span>|<span data-ttu-id="f33fb-143">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="f33fb-143">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f33fb-144">关系</span><span class="sxs-lookup"><span data-stu-id="f33fb-144">Relationships</span></span>
|<span data-ttu-id="f33fb-145">关系</span><span class="sxs-lookup"><span data-stu-id="f33fb-145">Relationship</span></span>|<span data-ttu-id="f33fb-146">类型</span><span class="sxs-lookup"><span data-stu-id="f33fb-146">Type</span></span>|<span data-ttu-id="f33fb-147">说明</span><span class="sxs-lookup"><span data-stu-id="f33fb-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f33fb-148">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="f33fb-148">deviceRunStates</span></span>|<span data-ttu-id="f33fb-149">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f33fb-149">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="f33fb-150">此脚本在特定用户的所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="f33fb-150">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f33fb-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f33fb-151">JSON Representation</span></span>
<span data-ttu-id="f33fb-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f33fb-152">Here is a JSON representation of the resource.</span></span>
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




