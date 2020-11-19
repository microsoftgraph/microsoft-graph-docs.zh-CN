---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7862605715e8ad1f6ef1ddf12413a9fb53111180
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230987"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="76449-103">deviceHealthScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="76449-103">deviceHealthScriptAssignment resource type</span></span>

<span data-ttu-id="76449-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76449-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76449-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76449-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76449-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76449-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76449-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="76449-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="76449-108">方法</span><span class="sxs-lookup"><span data-stu-id="76449-108">Methods</span></span>
|<span data-ttu-id="76449-109">方法</span><span class="sxs-lookup"><span data-stu-id="76449-109">Method</span></span>|<span data-ttu-id="76449-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="76449-110">Return Type</span></span>|<span data-ttu-id="76449-111">说明</span><span class="sxs-lookup"><span data-stu-id="76449-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76449-112">列出 deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="76449-112">List deviceHealthScriptAssignments</span></span>](../api/intune-devices-devicehealthscriptassignment-list.md)|<span data-ttu-id="76449-113">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76449-113">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="76449-114">列出 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76449-114">List properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="76449-115">获取 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-115">Get deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-get.md)|[<span data-ttu-id="76449-116">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-116">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="76449-117">读取 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76449-117">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="76449-118">创建 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-118">Create deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-create.md)|[<span data-ttu-id="76449-119">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-119">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="76449-120">创建新的 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76449-120">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="76449-121">删除 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-121">Delete deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-delete.md)|<span data-ttu-id="76449-122">无</span><span class="sxs-lookup"><span data-stu-id="76449-122">None</span></span>|<span data-ttu-id="76449-123">删除 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="76449-123">Deletes a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>|
|[<span data-ttu-id="76449-124">更新 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-124">Update deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-update.md)|[<span data-ttu-id="76449-125">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="76449-125">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="76449-126">更新 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76449-126">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76449-127">属性</span><span class="sxs-lookup"><span data-stu-id="76449-127">Properties</span></span>
|<span data-ttu-id="76449-128">属性</span><span class="sxs-lookup"><span data-stu-id="76449-128">Property</span></span>|<span data-ttu-id="76449-129">类型</span><span class="sxs-lookup"><span data-stu-id="76449-129">Type</span></span>|<span data-ttu-id="76449-130">说明</span><span class="sxs-lookup"><span data-stu-id="76449-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76449-131">id</span><span class="sxs-lookup"><span data-stu-id="76449-131">id</span></span>|<span data-ttu-id="76449-132">String</span><span class="sxs-lookup"><span data-stu-id="76449-132">String</span></span>|<span data-ttu-id="76449-133">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="76449-133">Key of the device health script assignment entity.</span></span> <span data-ttu-id="76449-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="76449-134">This property is read-only.</span></span>|
|<span data-ttu-id="76449-135">target</span><span class="sxs-lookup"><span data-stu-id="76449-135">target</span></span>|[<span data-ttu-id="76449-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="76449-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="76449-137">将脚本设定为的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="76449-137">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="76449-138">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="76449-138">runRemediationScript</span></span>|<span data-ttu-id="76449-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="76449-139">Boolean</span></span>|<span data-ttu-id="76449-140">确定是只运行检测脚本还是运行两个检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="76449-140">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="76449-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="76449-141">runSchedule</span></span>|[<span data-ttu-id="76449-142">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="76449-142">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="76449-143">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="76449-143">Script run schedule for the target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="76449-144">关系</span><span class="sxs-lookup"><span data-stu-id="76449-144">Relationships</span></span>
<span data-ttu-id="76449-145">无</span><span class="sxs-lookup"><span data-stu-id="76449-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76449-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76449-146">JSON Representation</span></span>
<span data-ttu-id="76449-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76449-147">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
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




