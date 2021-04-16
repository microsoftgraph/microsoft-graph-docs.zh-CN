---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 276104e49a12ff64fcbc585b3a5ce07570377397
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867325"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="84090-103">deviceHealthScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="84090-103">deviceHealthScriptAssignment resource type</span></span>

<span data-ttu-id="84090-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84090-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84090-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84090-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84090-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84090-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84090-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="84090-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="84090-108">方法</span><span class="sxs-lookup"><span data-stu-id="84090-108">Methods</span></span>
|<span data-ttu-id="84090-109">方法</span><span class="sxs-lookup"><span data-stu-id="84090-109">Method</span></span>|<span data-ttu-id="84090-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="84090-110">Return Type</span></span>|<span data-ttu-id="84090-111">说明</span><span class="sxs-lookup"><span data-stu-id="84090-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84090-112">列出 deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="84090-112">List deviceHealthScriptAssignments</span></span>](../api/intune-devices-devicehealthscriptassignment-list.md)|<span data-ttu-id="84090-113">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84090-113">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="84090-114">列出 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84090-114">List properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="84090-115">获取 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-115">Get deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-get.md)|[<span data-ttu-id="84090-116">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-116">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="84090-117">读取 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84090-117">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="84090-118">创建 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-118">Create deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-create.md)|[<span data-ttu-id="84090-119">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-119">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="84090-120">创建新的 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84090-120">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="84090-121">删除 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-121">Delete deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-delete.md)|<span data-ttu-id="84090-122">无</span><span class="sxs-lookup"><span data-stu-id="84090-122">None</span></span>|<span data-ttu-id="84090-123">删除 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="84090-123">Deletes a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>|
|[<span data-ttu-id="84090-124">更新 deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-124">Update deviceHealthScriptAssignment</span></span>](../api/intune-devices-devicehealthscriptassignment-update.md)|[<span data-ttu-id="84090-125">deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="84090-125">deviceHealthScriptAssignment</span></span>](../resources/intune-devices-devicehealthscriptassignment.md)|<span data-ttu-id="84090-126">更新 [deviceHealthScriptAssignment 对象](../resources/intune-devices-devicehealthscriptassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="84090-126">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84090-127">属性</span><span class="sxs-lookup"><span data-stu-id="84090-127">Properties</span></span>
|<span data-ttu-id="84090-128">属性</span><span class="sxs-lookup"><span data-stu-id="84090-128">Property</span></span>|<span data-ttu-id="84090-129">类型</span><span class="sxs-lookup"><span data-stu-id="84090-129">Type</span></span>|<span data-ttu-id="84090-130">说明</span><span class="sxs-lookup"><span data-stu-id="84090-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84090-131">id</span><span class="sxs-lookup"><span data-stu-id="84090-131">id</span></span>|<span data-ttu-id="84090-132">String</span><span class="sxs-lookup"><span data-stu-id="84090-132">String</span></span>|<span data-ttu-id="84090-133">设备运行状况脚本分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="84090-133">Key of the device health script assignment entity.</span></span> <span data-ttu-id="84090-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="84090-134">This property is read-only.</span></span>|
|<span data-ttu-id="84090-135">target</span><span class="sxs-lookup"><span data-stu-id="84090-135">target</span></span>|[<span data-ttu-id="84090-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="84090-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="84090-137">我们将脚本定向到的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="84090-137">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="84090-138">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="84090-138">runRemediationScript</span></span>|<span data-ttu-id="84090-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="84090-139">Boolean</span></span>|<span data-ttu-id="84090-140">确定是仅运行检测脚本还是同时运行检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="84090-140">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|

## <a name="relationships"></a><span data-ttu-id="84090-141">关系</span><span class="sxs-lookup"><span data-stu-id="84090-141">Relationships</span></span>
<span data-ttu-id="84090-142">无</span><span class="sxs-lookup"><span data-stu-id="84090-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84090-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84090-143">JSON Representation</span></span>
<span data-ttu-id="84090-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84090-144">Here is a JSON representation of the resource.</span></span>
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
  "runRemediationScript": true
}
```




