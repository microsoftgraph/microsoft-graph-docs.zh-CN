---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f86b85cd63c619e5ee5447e3f19a66f2a6524767
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793280"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="1a90f-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a90f-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="1a90f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a90f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a90f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a90f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a90f-106">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="1a90f-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="1a90f-107">方法</span><span class="sxs-lookup"><span data-stu-id="1a90f-107">Methods</span></span>
|<span data-ttu-id="1a90f-108">方法</span><span class="sxs-lookup"><span data-stu-id="1a90f-108">Method</span></span>|<span data-ttu-id="1a90f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a90f-109">Return Type</span></span>|<span data-ttu-id="1a90f-110">说明</span><span class="sxs-lookup"><span data-stu-id="1a90f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a90f-111">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="1a90f-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="1a90f-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a90f-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1a90f-113">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a90f-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="1a90f-114">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="1a90f-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="1a90f-116">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a90f-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1a90f-117">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="1a90f-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="1a90f-119">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a90f-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1a90f-120">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="1a90f-121">无</span><span class="sxs-lookup"><span data-stu-id="1a90f-121">None</span></span>|<span data-ttu-id="1a90f-122">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1a90f-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="1a90f-123">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="1a90f-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1a90f-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="1a90f-125">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a90f-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a90f-126">属性</span><span class="sxs-lookup"><span data-stu-id="1a90f-126">Properties</span></span>
|<span data-ttu-id="1a90f-127">属性</span><span class="sxs-lookup"><span data-stu-id="1a90f-127">Property</span></span>|<span data-ttu-id="1a90f-128">类型</span><span class="sxs-lookup"><span data-stu-id="1a90f-128">Type</span></span>|<span data-ttu-id="1a90f-129">说明</span><span class="sxs-lookup"><span data-stu-id="1a90f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a90f-130">id</span><span class="sxs-lookup"><span data-stu-id="1a90f-130">id</span></span>|<span data-ttu-id="1a90f-131">String</span><span class="sxs-lookup"><span data-stu-id="1a90f-131">String</span></span>|<span data-ttu-id="1a90f-132">分配的键。</span><span class="sxs-lookup"><span data-stu-id="1a90f-132">The key of the assignment.</span></span>|
|<span data-ttu-id="1a90f-133">target</span><span class="sxs-lookup"><span data-stu-id="1a90f-133">target</span></span>|[<span data-ttu-id="1a90f-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1a90f-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1a90f-135">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="1a90f-135">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="1a90f-136">source</span><span class="sxs-lookup"><span data-stu-id="1a90f-136">source</span></span>|[<span data-ttu-id="1a90f-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="1a90f-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="1a90f-138">设备配置、direct 或包裹/policySet 的工作分配源。</span><span class="sxs-lookup"><span data-stu-id="1a90f-138">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="1a90f-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1a90f-139">This property is read-only.</span></span> <span data-ttu-id="1a90f-140">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="1a90f-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="1a90f-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="1a90f-141">sourceId</span></span>|<span data-ttu-id="1a90f-142">String</span><span class="sxs-lookup"><span data-stu-id="1a90f-142">String</span></span>|<span data-ttu-id="1a90f-143">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="1a90f-143">The identifier of the source of the assignment.</span></span> <span data-ttu-id="1a90f-144">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1a90f-144">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a90f-145">关系</span><span class="sxs-lookup"><span data-stu-id="1a90f-145">Relationships</span></span>
<span data-ttu-id="1a90f-146">无</span><span class="sxs-lookup"><span data-stu-id="1a90f-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a90f-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a90f-147">JSON Representation</span></span>
<span data-ttu-id="1a90f-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a90f-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



