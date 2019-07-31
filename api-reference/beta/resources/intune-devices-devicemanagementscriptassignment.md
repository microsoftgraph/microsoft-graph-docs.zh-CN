---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ea203aa6b0e4714aed5f47530de8ca3be8bf50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999862"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="316eb-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="316eb-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="316eb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="316eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="316eb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="316eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="316eb-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="316eb-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="316eb-107">方法</span><span class="sxs-lookup"><span data-stu-id="316eb-107">Methods</span></span>
|<span data-ttu-id="316eb-108">方法</span><span class="sxs-lookup"><span data-stu-id="316eb-108">Method</span></span>|<span data-ttu-id="316eb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="316eb-109">Return Type</span></span>|<span data-ttu-id="316eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="316eb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="316eb-111">列出 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="316eb-111">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="316eb-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="316eb-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="316eb-113">列出[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="316eb-113">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="316eb-114">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-114">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="316eb-115">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-115">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="316eb-116">读取[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="316eb-116">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="316eb-117">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-117">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="316eb-118">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-118">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="316eb-119">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="316eb-119">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="316eb-120">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-120">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="316eb-121">无</span><span class="sxs-lookup"><span data-stu-id="316eb-121">None</span></span>|<span data-ttu-id="316eb-122">删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="316eb-122">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="316eb-123">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-123">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="316eb-124">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="316eb-124">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="316eb-125">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="316eb-125">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="316eb-126">属性</span><span class="sxs-lookup"><span data-stu-id="316eb-126">Properties</span></span>
|<span data-ttu-id="316eb-127">属性</span><span class="sxs-lookup"><span data-stu-id="316eb-127">Property</span></span>|<span data-ttu-id="316eb-128">类型</span><span class="sxs-lookup"><span data-stu-id="316eb-128">Type</span></span>|<span data-ttu-id="316eb-129">说明</span><span class="sxs-lookup"><span data-stu-id="316eb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="316eb-130">id</span><span class="sxs-lookup"><span data-stu-id="316eb-130">id</span></span>|<span data-ttu-id="316eb-131">String</span><span class="sxs-lookup"><span data-stu-id="316eb-131">String</span></span>|<span data-ttu-id="316eb-132">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="316eb-132">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="316eb-133">target</span><span class="sxs-lookup"><span data-stu-id="316eb-133">target</span></span>|[<span data-ttu-id="316eb-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="316eb-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="316eb-135">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="316eb-135">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="316eb-136">关系</span><span class="sxs-lookup"><span data-stu-id="316eb-136">Relationships</span></span>
<span data-ttu-id="316eb-137">无</span><span class="sxs-lookup"><span data-stu-id="316eb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="316eb-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="316eb-138">JSON Representation</span></span>
<span data-ttu-id="316eb-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="316eb-139">Here is a JSON representation of the resource.</span></span>
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





