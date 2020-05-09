---
title: deviceConfigurationAssignment 资源类型
description: 设备配置分配实体将 AAD 组分配到特定设备配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a391c926b077b32e48c5afc5efb6ac67fa8cc5ad
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179226"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="8ba1b-103">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ba1b-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="8ba1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ba1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ba1b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ba1b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ba1b-107">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8ba1b-108">方法</span><span class="sxs-lookup"><span data-stu-id="8ba1b-108">Methods</span></span>
|<span data-ttu-id="8ba1b-109">方法</span><span class="sxs-lookup"><span data-stu-id="8ba1b-109">Method</span></span>|<span data-ttu-id="8ba1b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8ba1b-110">Return Type</span></span>|<span data-ttu-id="8ba1b-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ba1b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ba1b-112">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="8ba1b-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="8ba1b-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ba1b-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8ba1b-114">列出 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="8ba1b-115">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="8ba1b-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8ba1b-117">读取 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8ba1b-118">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="8ba1b-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8ba1b-120">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8ba1b-121">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="8ba1b-122">无</span><span class="sxs-lookup"><span data-stu-id="8ba1b-122">None</span></span>|<span data-ttu-id="8ba1b-123">删除 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="8ba1b-124">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="8ba1b-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ba1b-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8ba1b-126">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ba1b-127">属性</span><span class="sxs-lookup"><span data-stu-id="8ba1b-127">Properties</span></span>
|<span data-ttu-id="8ba1b-128">属性</span><span class="sxs-lookup"><span data-stu-id="8ba1b-128">Property</span></span>|<span data-ttu-id="8ba1b-129">类型</span><span class="sxs-lookup"><span data-stu-id="8ba1b-129">Type</span></span>|<span data-ttu-id="8ba1b-130">说明</span><span class="sxs-lookup"><span data-stu-id="8ba1b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba1b-131">id</span><span class="sxs-lookup"><span data-stu-id="8ba1b-131">id</span></span>|<span data-ttu-id="8ba1b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="8ba1b-132">String</span></span>|<span data-ttu-id="8ba1b-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-133">The key of the assignment.</span></span>|
|<span data-ttu-id="8ba1b-134">target</span><span class="sxs-lookup"><span data-stu-id="8ba1b-134">target</span></span>|[<span data-ttu-id="8ba1b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8ba1b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8ba1b-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="8ba1b-137">source</span><span class="sxs-lookup"><span data-stu-id="8ba1b-137">source</span></span>|[<span data-ttu-id="8ba1b-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8ba1b-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8ba1b-139">设备配置、direct 或包裹/policySet 的工作分配源。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="8ba1b-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-140">This property is read-only.</span></span> <span data-ttu-id="8ba1b-141">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8ba1b-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="8ba1b-142">sourceId</span></span>|<span data-ttu-id="8ba1b-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8ba1b-143">String</span></span>|<span data-ttu-id="8ba1b-144">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="8ba1b-145">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ba1b-146">关系</span><span class="sxs-lookup"><span data-stu-id="8ba1b-146">Relationships</span></span>
<span data-ttu-id="8ba1b-147">无</span><span class="sxs-lookup"><span data-stu-id="8ba1b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ba1b-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ba1b-148">JSON Representation</span></span>
<span data-ttu-id="8ba1b-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ba1b-149">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



