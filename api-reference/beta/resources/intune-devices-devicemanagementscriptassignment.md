---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8eac4db0ce0bec29602b2b340e7d1604f4fa241d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158161"
---
# <a name="devicemanagementscriptassignment-resource-type"></a><span data-ttu-id="90921-103">deviceManagementScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="90921-103">deviceManagementScriptAssignment resource type</span></span>

<span data-ttu-id="90921-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90921-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90921-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90921-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90921-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90921-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90921-107">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="90921-107">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="90921-108">方法</span><span class="sxs-lookup"><span data-stu-id="90921-108">Methods</span></span>
|<span data-ttu-id="90921-109">方法</span><span class="sxs-lookup"><span data-stu-id="90921-109">Method</span></span>|<span data-ttu-id="90921-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="90921-110">Return Type</span></span>|<span data-ttu-id="90921-111">说明</span><span class="sxs-lookup"><span data-stu-id="90921-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90921-112">列出 deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="90921-112">List deviceManagementScriptAssignments</span></span>](../api/intune-devices-devicemanagementscriptassignment-list.md)|<span data-ttu-id="90921-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90921-113">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="90921-114">列出 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90921-114">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>|
|[<span data-ttu-id="90921-115">获取 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-115">Get deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-get.md)|[<span data-ttu-id="90921-116">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-116">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="90921-117">读取 [deviceManagementScriptAssignment 对象的属性和](../resources/intune-devices-devicemanagementscriptassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="90921-117">Read properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="90921-118">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-118">Create deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-create.md)|[<span data-ttu-id="90921-119">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-119">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="90921-120">创建新的 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90921-120">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|
|[<span data-ttu-id="90921-121">删除 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-121">Delete deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-delete.md)|<span data-ttu-id="90921-122">无</span><span class="sxs-lookup"><span data-stu-id="90921-122">None</span></span>|<span data-ttu-id="90921-123">删除 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="90921-123">Deletes a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>|
|[<span data-ttu-id="90921-124">更新 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-124">Update deviceManagementScriptAssignment</span></span>](../api/intune-devices-devicemanagementscriptassignment-update.md)|[<span data-ttu-id="90921-125">deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="90921-125">deviceManagementScriptAssignment</span></span>](../resources/intune-devices-devicemanagementscriptassignment.md)|<span data-ttu-id="90921-126">更新 [deviceManagementScriptAssignment 对象](../resources/intune-devices-devicemanagementscriptassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="90921-126">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90921-127">属性</span><span class="sxs-lookup"><span data-stu-id="90921-127">Properties</span></span>
|<span data-ttu-id="90921-128">属性</span><span class="sxs-lookup"><span data-stu-id="90921-128">Property</span></span>|<span data-ttu-id="90921-129">类型</span><span class="sxs-lookup"><span data-stu-id="90921-129">Type</span></span>|<span data-ttu-id="90921-130">说明</span><span class="sxs-lookup"><span data-stu-id="90921-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90921-131">id</span><span class="sxs-lookup"><span data-stu-id="90921-131">id</span></span>|<span data-ttu-id="90921-132">String</span><span class="sxs-lookup"><span data-stu-id="90921-132">String</span></span>|<span data-ttu-id="90921-133">设备管理脚本组分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="90921-133">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="90921-134">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="90921-134">This property is read-only.</span></span>|
|<span data-ttu-id="90921-135">target</span><span class="sxs-lookup"><span data-stu-id="90921-135">target</span></span>|[<span data-ttu-id="90921-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="90921-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="90921-137">我们将脚本定向到的 Azure Active Directory 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="90921-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90921-138">关系</span><span class="sxs-lookup"><span data-stu-id="90921-138">Relationships</span></span>
<span data-ttu-id="90921-139">无</span><span class="sxs-lookup"><span data-stu-id="90921-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90921-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90921-140">JSON Representation</span></span>
<span data-ttu-id="90921-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90921-141">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




