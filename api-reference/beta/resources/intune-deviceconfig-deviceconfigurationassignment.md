---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd2dad2bfb846a876e369a3b8fc1a36c846a8276
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154871"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="5e080-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e080-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="5e080-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e080-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e080-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e080-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e080-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e080-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e080-107">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="5e080-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="5e080-108">方法</span><span class="sxs-lookup"><span data-stu-id="5e080-108">Methods</span></span>
|<span data-ttu-id="5e080-109">方法</span><span class="sxs-lookup"><span data-stu-id="5e080-109">Method</span></span>|<span data-ttu-id="5e080-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e080-110">Return Type</span></span>|<span data-ttu-id="5e080-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e080-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e080-112">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="5e080-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="5e080-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e080-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5e080-114">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e080-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="5e080-115">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="5e080-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="5e080-117">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e080-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="5e080-118">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="5e080-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="5e080-120">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e080-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="5e080-121">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="5e080-122">无</span><span class="sxs-lookup"><span data-stu-id="5e080-122">None</span></span>|<span data-ttu-id="5e080-123">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5e080-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="5e080-124">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="5e080-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e080-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="5e080-126">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e080-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e080-127">属性</span><span class="sxs-lookup"><span data-stu-id="5e080-127">Properties</span></span>
|<span data-ttu-id="5e080-128">属性</span><span class="sxs-lookup"><span data-stu-id="5e080-128">Property</span></span>|<span data-ttu-id="5e080-129">类型</span><span class="sxs-lookup"><span data-stu-id="5e080-129">Type</span></span>|<span data-ttu-id="5e080-130">说明</span><span class="sxs-lookup"><span data-stu-id="5e080-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e080-131">id</span><span class="sxs-lookup"><span data-stu-id="5e080-131">id</span></span>|<span data-ttu-id="5e080-132">String</span><span class="sxs-lookup"><span data-stu-id="5e080-132">String</span></span>|<span data-ttu-id="5e080-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="5e080-133">The key of the assignment.</span></span>|
|<span data-ttu-id="5e080-134">target</span><span class="sxs-lookup"><span data-stu-id="5e080-134">target</span></span>|[<span data-ttu-id="5e080-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5e080-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5e080-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="5e080-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="5e080-137">source</span><span class="sxs-lookup"><span data-stu-id="5e080-137">source</span></span>|[<span data-ttu-id="5e080-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="5e080-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="5e080-139">设备配置分配源：direct 或/policySet。</span><span class="sxs-lookup"><span data-stu-id="5e080-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="5e080-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e080-140">This property is read-only.</span></span> <span data-ttu-id="5e080-141">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="5e080-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="5e080-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="5e080-142">sourceId</span></span>|<span data-ttu-id="5e080-143">String</span><span class="sxs-lookup"><span data-stu-id="5e080-143">String</span></span>|<span data-ttu-id="5e080-144">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="5e080-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="5e080-145">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e080-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e080-146">关系</span><span class="sxs-lookup"><span data-stu-id="5e080-146">Relationships</span></span>
<span data-ttu-id="5e080-147">无</span><span class="sxs-lookup"><span data-stu-id="5e080-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e080-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e080-148">JSON Representation</span></span>
<span data-ttu-id="5e080-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e080-149">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




