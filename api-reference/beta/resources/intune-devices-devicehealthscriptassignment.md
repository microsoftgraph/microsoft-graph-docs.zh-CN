---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6849c3d8adb7ff10a8322d83707af0aeb328ddd0
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612075"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="101a5-103">deviceHealthScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="101a5-103">deviceHealthScriptAssignment resource type</span></span>

<span data-ttu-id="101a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="101a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="101a5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="101a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="101a5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="101a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="101a5-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="101a5-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="101a5-108">方法</span><span class="sxs-lookup"><span data-stu-id="101a5-108">Methods</span></span>
|<span data-ttu-id="101a5-109">方法</span><span class="sxs-lookup"><span data-stu-id="101a5-109">Method</span></span>|<span data-ttu-id="101a5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="101a5-110">Return Type</span></span>|<span data-ttu-id="101a5-111">Description</span><span class="sxs-lookup"><span data-stu-id="101a5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="101a5-112">列出 deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="101a5-112">List deviceHealthScriptAssignments</span></span>](../api/intune-devices-devicehealthscriptassignment-list.md)|<span data-ttu-id="101a5-113">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="101a5-113">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="101a5-114">列出 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="101a5-114">List properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="101a5-115">获取 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-115">Get deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-get.md)|[<span data-ttu-id="101a5-116">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-116">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="101a5-117">读取 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="101a5-117">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="101a5-118">创建 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-118">Create deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-create.md)|[<span data-ttu-id="101a5-119">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-119">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="101a5-120">创建新的 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="101a5-120">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="101a5-121">删除 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-121">Delete deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-delete.md)|<span data-ttu-id="101a5-122">无</span><span class="sxs-lookup"><span data-stu-id="101a5-122">None</span></span>|<span data-ttu-id="101a5-123">删除 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="101a5-123">Deletes a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>|
|[<span data-ttu-id="101a5-124">更新 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-124">Update deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-update.md)|[<span data-ttu-id="101a5-125">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="101a5-125">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="101a5-126">更新 [deviceHealthScriptAssignment 对象](../resources/intune-devices-devicehealthscriptassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="101a5-126">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="101a5-127">属性</span><span class="sxs-lookup"><span data-stu-id="101a5-127">Properties</span></span>
|<span data-ttu-id="101a5-128">属性</span><span class="sxs-lookup"><span data-stu-id="101a5-128">Property</span></span>|<span data-ttu-id="101a5-129">类型</span><span class="sxs-lookup"><span data-stu-id="101a5-129">Type</span></span>|<span data-ttu-id="101a5-130">说明</span><span class="sxs-lookup"><span data-stu-id="101a5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="101a5-131">id</span><span class="sxs-lookup"><span data-stu-id="101a5-131">id</span></span>|<span data-ttu-id="101a5-132">String</span><span class="sxs-lookup"><span data-stu-id="101a5-132">String</span></span>|<span data-ttu-id="101a5-133">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="101a5-133">Key of the device health script assignment entity.</span></span> <span data-ttu-id="101a5-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="101a5-134">This property is read-only.</span></span>|
|<span data-ttu-id="101a5-135">target</span><span class="sxs-lookup"><span data-stu-id="101a5-135">target</span></span>|[<span data-ttu-id="101a5-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="101a5-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="101a5-137">我们将脚本定向到的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="101a5-137">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="101a5-138">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="101a5-138">runRemediationScript</span></span>|<span data-ttu-id="101a5-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="101a5-139">Boolean</span></span>|<span data-ttu-id="101a5-140">确定是仅运行检测脚本还是同时运行检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="101a5-140">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="101a5-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="101a5-141">runSchedule</span></span>|[<span data-ttu-id="101a5-142">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="101a5-142">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="101a5-143">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="101a5-143">Script run schedule for the target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="101a5-144">关系</span><span class="sxs-lookup"><span data-stu-id="101a5-144">Relationships</span></span>
<span data-ttu-id="101a5-145">无</span><span class="sxs-lookup"><span data-stu-id="101a5-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="101a5-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="101a5-146">JSON Representation</span></span>
<span data-ttu-id="101a5-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="101a5-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
    "interval": 1024,
    "useUtc": true,
    "time": "String (time of day)"
  }
}
```




