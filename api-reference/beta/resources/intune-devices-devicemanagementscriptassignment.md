---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1eb5092de59dbe9b6f83916a082aaa5e2a9879bc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784914"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="ef04f-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-103">deviceManagementScriptAssignment resource type</span></span>

> <span data-ttu-id="ef04f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ef04f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef04f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef04f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef04f-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="ef04f-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="ef04f-107">方法</span><span class="sxs-lookup"><span data-stu-id="ef04f-107">Methods</span></span>
|<span data-ttu-id="ef04f-108">方法</span><span class="sxs-lookup"><span data-stu-id="ef04f-108">Method</span></span>|<span data-ttu-id="ef04f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-109">Return Type</span></span>|<span data-ttu-id="ef04f-110">说明</span><span class="sxs-lookup"><span data-stu-id="ef04f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ef04f-111">列出 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="ef04f-111">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="ef04f-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ef04f-112">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="ef04f-113">列出[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ef04f-113">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="ef04f-114">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-114">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="ef04f-115">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-115">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="ef04f-116">读取[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ef04f-116">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="ef04f-117">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-117">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="ef04f-118">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-118">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="ef04f-119">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef04f-119">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="ef04f-120">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-120">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="ef04f-121">None</span><span class="sxs-lookup"><span data-stu-id="ef04f-121">None</span></span>|<span data-ttu-id="ef04f-122">删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="ef04f-122">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="ef04f-123">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-123">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="ef04f-124">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="ef04f-124">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="ef04f-125">更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ef04f-125">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef04f-126">属性</span><span class="sxs-lookup"><span data-stu-id="ef04f-126">Properties</span></span>
|<span data-ttu-id="ef04f-127">属性</span><span class="sxs-lookup"><span data-stu-id="ef04f-127">Property</span></span>|<span data-ttu-id="ef04f-128">类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-128">Type</span></span>|<span data-ttu-id="ef04f-129">说明</span><span class="sxs-lookup"><span data-stu-id="ef04f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef04f-130">id</span><span class="sxs-lookup"><span data-stu-id="ef04f-130">id</span></span>|<span data-ttu-id="ef04f-131">String</span><span class="sxs-lookup"><span data-stu-id="ef04f-131">String</span></span>|<span data-ttu-id="ef04f-132">Device management script group 分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef04f-132">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="ef04f-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ef04f-133">This property is read-only.</span></span>|
|<span data-ttu-id="ef04f-134">target</span><span class="sxs-lookup"><span data-stu-id="ef04f-134">target</span></span>|[<span data-ttu-id="ef04f-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ef04f-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ef04f-136">要作为脚本目标的 Azure Active Directory 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="ef04f-136">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef04f-137">关系</span><span class="sxs-lookup"><span data-stu-id="ef04f-137">Relationships</span></span>
<span data-ttu-id="ef04f-138">无</span><span class="sxs-lookup"><span data-stu-id="ef04f-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef04f-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef04f-139">JSON Representation</span></span>
<span data-ttu-id="ef04f-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef04f-140">Here is a JSON representation of the resource.</span></span>
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



