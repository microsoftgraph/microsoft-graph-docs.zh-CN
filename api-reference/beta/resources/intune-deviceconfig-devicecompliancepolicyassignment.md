---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6042de740a5f8ddf30bad329fb293698423c73aa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199404"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="244be-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="244be-103">deviceCompliancePolicyAssignment resource type</span></span>

<span data-ttu-id="244be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="244be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="244be-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="244be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="244be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="244be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="244be-107">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="244be-107">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="244be-108">方法</span><span class="sxs-lookup"><span data-stu-id="244be-108">Methods</span></span>
|<span data-ttu-id="244be-109">方法</span><span class="sxs-lookup"><span data-stu-id="244be-109">Method</span></span>|<span data-ttu-id="244be-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="244be-110">Return Type</span></span>|<span data-ttu-id="244be-111">说明</span><span class="sxs-lookup"><span data-stu-id="244be-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="244be-112">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="244be-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="244be-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="244be-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="244be-114">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="244be-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="244be-115">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="244be-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="244be-117">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="244be-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="244be-118">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="244be-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="244be-120">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="244be-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="244be-121">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="244be-122">无</span><span class="sxs-lookup"><span data-stu-id="244be-122">None</span></span>|<span data-ttu-id="244be-123">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="244be-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="244be-124">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="244be-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="244be-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="244be-126">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="244be-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="244be-127">属性</span><span class="sxs-lookup"><span data-stu-id="244be-127">Properties</span></span>
|<span data-ttu-id="244be-128">属性</span><span class="sxs-lookup"><span data-stu-id="244be-128">Property</span></span>|<span data-ttu-id="244be-129">类型</span><span class="sxs-lookup"><span data-stu-id="244be-129">Type</span></span>|<span data-ttu-id="244be-130">说明</span><span class="sxs-lookup"><span data-stu-id="244be-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="244be-131">id</span><span class="sxs-lookup"><span data-stu-id="244be-131">id</span></span>|<span data-ttu-id="244be-132">String</span><span class="sxs-lookup"><span data-stu-id="244be-132">String</span></span>|<span data-ttu-id="244be-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="244be-133">Key of the entity.</span></span>|
|<span data-ttu-id="244be-134">target</span><span class="sxs-lookup"><span data-stu-id="244be-134">target</span></span>|[<span data-ttu-id="244be-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="244be-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="244be-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="244be-136">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="244be-137">source</span><span class="sxs-lookup"><span data-stu-id="244be-137">source</span></span>|[<span data-ttu-id="244be-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="244be-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="244be-139">设备合规性策略、direct 或包裹/policySet 的分配源。</span><span class="sxs-lookup"><span data-stu-id="244be-139">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="244be-140">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="244be-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="244be-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="244be-141">sourceId</span></span>|<span data-ttu-id="244be-142">String</span><span class="sxs-lookup"><span data-stu-id="244be-142">String</span></span>|<span data-ttu-id="244be-143">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="244be-143">The identifier of the source of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="244be-144">关系</span><span class="sxs-lookup"><span data-stu-id="244be-144">Relationships</span></span>
<span data-ttu-id="244be-145">无</span><span class="sxs-lookup"><span data-stu-id="244be-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="244be-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="244be-146">JSON Representation</span></span>
<span data-ttu-id="244be-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="244be-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




