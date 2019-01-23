---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于分配给组的设备管理脚本的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6e153842e0b820a845260bc125154df7cef0cb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413848"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="d8975-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8975-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="d8975-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d8975-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8975-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8975-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8975-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8975-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8975-107">包含用于分配给组的设备管理脚本的属性。</span><span class="sxs-lookup"><span data-stu-id="d8975-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="d8975-108">方法</span><span class="sxs-lookup"><span data-stu-id="d8975-108">Methods</span></span>
|<span data-ttu-id="d8975-109">方法</span><span class="sxs-lookup"><span data-stu-id="d8975-109">Method</span></span>|<span data-ttu-id="d8975-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8975-110">Return Type</span></span>|<span data-ttu-id="d8975-111">说明</span><span class="sxs-lookup"><span data-stu-id="d8975-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8975-112">列表 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="d8975-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="d8975-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d8975-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d8975-114">列出属性和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d8975-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="d8975-115">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="d8975-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d8975-117">读取属性和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d8975-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="d8975-118">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="d8975-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d8975-120">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8975-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="d8975-121">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="d8975-122">无</span><span class="sxs-lookup"><span data-stu-id="d8975-122">None</span></span>|<span data-ttu-id="d8975-123">删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d8975-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="d8975-124">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="d8975-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d8975-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="d8975-126">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8975-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8975-127">属性</span><span class="sxs-lookup"><span data-stu-id="d8975-127">Properties</span></span>
|<span data-ttu-id="d8975-128">属性</span><span class="sxs-lookup"><span data-stu-id="d8975-128">Property</span></span>|<span data-ttu-id="d8975-129">类型</span><span class="sxs-lookup"><span data-stu-id="d8975-129">Type</span></span>|<span data-ttu-id="d8975-130">说明</span><span class="sxs-lookup"><span data-stu-id="d8975-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8975-131">id</span><span class="sxs-lookup"><span data-stu-id="d8975-131">id</span></span>|<span data-ttu-id="d8975-132">String</span><span class="sxs-lookup"><span data-stu-id="d8975-132">String</span></span>|<span data-ttu-id="d8975-133">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8975-133">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="d8975-134">target</span><span class="sxs-lookup"><span data-stu-id="d8975-134">target</span></span>|[<span data-ttu-id="d8975-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d8975-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d8975-136">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="d8975-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8975-137">关系</span><span class="sxs-lookup"><span data-stu-id="d8975-137">Relationships</span></span>
<span data-ttu-id="d8975-138">无</span><span class="sxs-lookup"><span data-stu-id="d8975-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8975-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8975-139">JSON Representation</span></span>
<span data-ttu-id="d8975-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8975-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




