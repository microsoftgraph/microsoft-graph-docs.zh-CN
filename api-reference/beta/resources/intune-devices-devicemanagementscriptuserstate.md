---
title: deviceManagementScriptUserState 资源类型
description: 包含设备管理脚本的用户运行状态的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2476329a402e0d6a50594ab110e88da4b5f5ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522403"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a><span data-ttu-id="b5748-103">deviceManagementScriptUserState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5748-103">deviceManagementScriptUserState resource type</span></span>

> <span data-ttu-id="b5748-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5748-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5748-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5748-106">包含设备管理脚本的用户运行状态的属性。</span><span class="sxs-lookup"><span data-stu-id="b5748-106">Contains properties for user run state of the device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="b5748-107">方法</span><span class="sxs-lookup"><span data-stu-id="b5748-107">Methods</span></span>
|<span data-ttu-id="b5748-108">方法</span><span class="sxs-lookup"><span data-stu-id="b5748-108">Method</span></span>|<span data-ttu-id="b5748-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5748-109">Return Type</span></span>|<span data-ttu-id="b5748-110">说明</span><span class="sxs-lookup"><span data-stu-id="b5748-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5748-111">列出 deviceManagementScriptUserStates</span><span class="sxs-lookup"><span data-stu-id="b5748-111">List deviceManagementScriptUserStates</span></span>](../api/intune-devices-devicemanagementscriptuserstate-list.md)|<span data-ttu-id="b5748-112">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="b5748-112">[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) collection</span></span>|<span data-ttu-id="b5748-113">列出[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5748-113">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>|
|[<span data-ttu-id="b5748-114">获取 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-114">Get deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[<span data-ttu-id="b5748-115">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-115">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="b5748-116">读取[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5748-116">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="b5748-117">创建 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-117">Create deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[<span data-ttu-id="b5748-118">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-118">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="b5748-119">创建新的[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b5748-119">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|
|[<span data-ttu-id="b5748-120">删除 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-120">Delete deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|<span data-ttu-id="b5748-121">无</span><span class="sxs-lookup"><span data-stu-id="b5748-121">None</span></span>|<span data-ttu-id="b5748-122">删除[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)。</span><span class="sxs-lookup"><span data-stu-id="b5748-122">Deletes a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>|
|[<span data-ttu-id="b5748-123">更新 deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-123">Update deviceManagementScriptUserState</span></span>](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[<span data-ttu-id="b5748-124">deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b5748-124">deviceManagementScriptUserState</span></span>](../resources/intune-devices-devicemanagementscriptuserstate.md)|<span data-ttu-id="b5748-125">更新[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5748-125">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5748-126">属性</span><span class="sxs-lookup"><span data-stu-id="b5748-126">Properties</span></span>
|<span data-ttu-id="b5748-127">属性</span><span class="sxs-lookup"><span data-stu-id="b5748-127">Property</span></span>|<span data-ttu-id="b5748-128">类型</span><span class="sxs-lookup"><span data-stu-id="b5748-128">Type</span></span>|<span data-ttu-id="b5748-129">说明</span><span class="sxs-lookup"><span data-stu-id="b5748-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5748-130">id</span><span class="sxs-lookup"><span data-stu-id="b5748-130">id</span></span>|<span data-ttu-id="b5748-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b5748-131">String</span></span>|<span data-ttu-id="b5748-132">设备管理脚本用户状态实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5748-132">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="b5748-133">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5748-133">successDeviceCount</span></span>|<span data-ttu-id="b5748-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b5748-134">Int32</span></span>|<span data-ttu-id="b5748-135">特定用户的成功设备计数。</span><span class="sxs-lookup"><span data-stu-id="b5748-135">Success device count for specific user.</span></span>|
|<span data-ttu-id="b5748-136">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5748-136">errorDeviceCount</span></span>|<span data-ttu-id="b5748-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b5748-137">Int32</span></span>|<span data-ttu-id="b5748-138">特定用户的错误设备计数。</span><span class="sxs-lookup"><span data-stu-id="b5748-138">Error device count for specific user.</span></span>|
|<span data-ttu-id="b5748-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5748-139">userPrincipalName</span></span>|<span data-ttu-id="b5748-140">String</span><span class="sxs-lookup"><span data-stu-id="b5748-140">String</span></span>|<span data-ttu-id="b5748-141">特定用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b5748-141">User principle name of specific user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5748-142">关系</span><span class="sxs-lookup"><span data-stu-id="b5748-142">Relationships</span></span>
|<span data-ttu-id="b5748-143">关系</span><span class="sxs-lookup"><span data-stu-id="b5748-143">Relationship</span></span>|<span data-ttu-id="b5748-144">类型</span><span class="sxs-lookup"><span data-stu-id="b5748-144">Type</span></span>|<span data-ttu-id="b5748-145">说明</span><span class="sxs-lookup"><span data-stu-id="b5748-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5748-146">deviceRunStates</span><span class="sxs-lookup"><span data-stu-id="b5748-146">deviceRunStates</span></span>|<span data-ttu-id="b5748-147">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="b5748-147">[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) collection</span></span>|<span data-ttu-id="b5748-148">此脚本在特定用户的所有设备上的运行状态列表。</span><span class="sxs-lookup"><span data-stu-id="b5748-148">List of run states for this script across all devices of specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5748-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5748-149">JSON Representation</span></span>
<span data-ttu-id="b5748-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5748-150">Here is a JSON representation of the resource.</span></span>
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





