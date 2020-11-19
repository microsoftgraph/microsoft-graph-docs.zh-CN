---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 072d11542b186459ca57dfa9fc575e05f8189766
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299203"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="7432d-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7432d-103">deviceManagementScriptAssignment resource type</span></span>

<span data-ttu-id="7432d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7432d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7432d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7432d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7432d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7432d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7432d-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="7432d-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="7432d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="7432d-108">Methods</span></span>
|<span data-ttu-id="7432d-109">方法</span><span class="sxs-lookup"><span data-stu-id="7432d-109">Method</span></span>|<span data-ttu-id="7432d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7432d-110">Return Type</span></span>|<span data-ttu-id="7432d-111">Description</span><span class="sxs-lookup"><span data-stu-id="7432d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7432d-112">列出 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="7432d-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="7432d-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7432d-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="7432d-114">列出 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7432d-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="7432d-115">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="7432d-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="7432d-117">读取 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7432d-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="7432d-118">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="7432d-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="7432d-120">创建新的 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7432d-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="7432d-121">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="7432d-122">无</span><span class="sxs-lookup"><span data-stu-id="7432d-122">None</span></span>|<span data-ttu-id="7432d-123">删除 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7432d-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="7432d-124">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="7432d-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7432d-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="7432d-126">更新 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7432d-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7432d-127">属性</span><span class="sxs-lookup"><span data-stu-id="7432d-127">Properties</span></span>
|<span data-ttu-id="7432d-128">属性</span><span class="sxs-lookup"><span data-stu-id="7432d-128">Property</span></span>|<span data-ttu-id="7432d-129">类型</span><span class="sxs-lookup"><span data-stu-id="7432d-129">Type</span></span>|<span data-ttu-id="7432d-130">说明</span><span class="sxs-lookup"><span data-stu-id="7432d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7432d-131">id</span><span class="sxs-lookup"><span data-stu-id="7432d-131">id</span></span>|<span data-ttu-id="7432d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="7432d-132">String</span></span>|<span data-ttu-id="7432d-133">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="7432d-133">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="7432d-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7432d-134">This property is read-only.</span></span>|
|<span data-ttu-id="7432d-135">target</span><span class="sxs-lookup"><span data-stu-id="7432d-135">target</span></span>|[<span data-ttu-id="7432d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7432d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7432d-137">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="7432d-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7432d-138">关系</span><span class="sxs-lookup"><span data-stu-id="7432d-138">Relationships</span></span>
<span data-ttu-id="7432d-139">无</span><span class="sxs-lookup"><span data-stu-id="7432d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7432d-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7432d-140">JSON Representation</span></span>
<span data-ttu-id="7432d-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7432d-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




