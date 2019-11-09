---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6704afe5e105491e2be35bda1e68dd446f3c88
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088299"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="b6f41-103">deviceHealthScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6f41-103">deviceHealthScriptAssignment resource type</span></span>

> <span data-ttu-id="b6f41-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6f41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6f41-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6f41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f41-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="b6f41-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="b6f41-107">方法</span><span class="sxs-lookup"><span data-stu-id="b6f41-107">Methods</span></span>
|<span data-ttu-id="b6f41-108">方法</span><span class="sxs-lookup"><span data-stu-id="b6f41-108">Method</span></span>|<span data-ttu-id="b6f41-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6f41-109">Return Type</span></span>|<span data-ttu-id="b6f41-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6f41-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6f41-111">列出 deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="b6f41-111">List deviceHealthScriptAssignments</span></span>](../api/intune-devices-devicehealthscriptassignment-list.md)|<span data-ttu-id="b6f41-112">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6f41-112">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="b6f41-113">列出[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6f41-113">List properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="b6f41-114">获取 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-114">Get deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-get.md)|[<span data-ttu-id="b6f41-115">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-115">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="b6f41-116">读取[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6f41-116">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="b6f41-117">创建 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-117">Create deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-create.md)|[<span data-ttu-id="b6f41-118">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-118">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="b6f41-119">创建新的[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6f41-119">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="b6f41-120">删除 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-120">Delete deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-delete.md)|<span data-ttu-id="b6f41-121">无</span><span class="sxs-lookup"><span data-stu-id="b6f41-121">None</span></span>|<span data-ttu-id="b6f41-122">删除[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="b6f41-122">Deletes a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>|
|[<span data-ttu-id="b6f41-123">更新 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-123">Update deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-update.md)|[<span data-ttu-id="b6f41-124">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="b6f41-124">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="b6f41-125">更新[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6f41-125">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6f41-126">属性</span><span class="sxs-lookup"><span data-stu-id="b6f41-126">Properties</span></span>
|<span data-ttu-id="b6f41-127">属性</span><span class="sxs-lookup"><span data-stu-id="b6f41-127">Property</span></span>|<span data-ttu-id="b6f41-128">类型</span><span class="sxs-lookup"><span data-stu-id="b6f41-128">Type</span></span>|<span data-ttu-id="b6f41-129">说明</span><span class="sxs-lookup"><span data-stu-id="b6f41-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6f41-130">id</span><span class="sxs-lookup"><span data-stu-id="b6f41-130">id</span></span>|<span data-ttu-id="b6f41-131">String</span><span class="sxs-lookup"><span data-stu-id="b6f41-131">String</span></span>|<span data-ttu-id="b6f41-132">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6f41-132">Key of the device health script assignment entity.</span></span> <span data-ttu-id="b6f41-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b6f41-133">This property is read-only.</span></span>|
|<span data-ttu-id="b6f41-134">target</span><span class="sxs-lookup"><span data-stu-id="b6f41-134">target</span></span>|[<span data-ttu-id="b6f41-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b6f41-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b6f41-136">将脚本设定为的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="b6f41-136">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="b6f41-137">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="b6f41-137">runRemediationScript</span></span>|<span data-ttu-id="b6f41-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6f41-138">Boolean</span></span>|<span data-ttu-id="b6f41-139">确定是只运行检测脚本还是运行两个检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="b6f41-139">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="b6f41-140">runSchedule</span><span class="sxs-lookup"><span data-stu-id="b6f41-140">runSchedule</span></span>|[<span data-ttu-id="b6f41-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="b6f41-141">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="b6f41-142">目标组的脚本运行计划</span><span class="sxs-lookup"><span data-stu-id="b6f41-142">Script run schedule for the target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6f41-143">关系</span><span class="sxs-lookup"><span data-stu-id="b6f41-143">Relationships</span></span>
<span data-ttu-id="b6f41-144">无</span><span class="sxs-lookup"><span data-stu-id="b6f41-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6f41-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6f41-145">JSON Representation</span></span>
<span data-ttu-id="b6f41-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6f41-146">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



