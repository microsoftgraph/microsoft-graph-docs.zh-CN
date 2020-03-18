---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e1fd9bd3ed5ee2e1e86b3dffa2cf152dab60e60
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793343"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="4fc52-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4fc52-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="4fc52-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4fc52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fc52-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fc52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc52-106">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="4fc52-106">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="4fc52-107">方法</span><span class="sxs-lookup"><span data-stu-id="4fc52-107">Methods</span></span>
|<span data-ttu-id="4fc52-108">方法</span><span class="sxs-lookup"><span data-stu-id="4fc52-108">Method</span></span>|<span data-ttu-id="4fc52-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4fc52-109">Return Type</span></span>|<span data-ttu-id="4fc52-110">说明</span><span class="sxs-lookup"><span data-stu-id="4fc52-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fc52-111">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="4fc52-111">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="4fc52-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fc52-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="4fc52-113">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fc52-113">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="4fc52-114">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-114">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="4fc52-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="4fc52-116">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fc52-116">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="4fc52-117">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-117">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="4fc52-118">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-118">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="4fc52-119">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fc52-119">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="4fc52-120">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-120">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="4fc52-121">无</span><span class="sxs-lookup"><span data-stu-id="4fc52-121">None</span></span>|<span data-ttu-id="4fc52-122">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4fc52-122">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="4fc52-123">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-123">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="4fc52-124">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc52-124">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="4fc52-125">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4fc52-125">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4fc52-126">属性</span><span class="sxs-lookup"><span data-stu-id="4fc52-126">Properties</span></span>
|<span data-ttu-id="4fc52-127">属性</span><span class="sxs-lookup"><span data-stu-id="4fc52-127">Property</span></span>|<span data-ttu-id="4fc52-128">类型</span><span class="sxs-lookup"><span data-stu-id="4fc52-128">Type</span></span>|<span data-ttu-id="4fc52-129">说明</span><span class="sxs-lookup"><span data-stu-id="4fc52-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc52-130">id</span><span class="sxs-lookup"><span data-stu-id="4fc52-130">id</span></span>|<span data-ttu-id="4fc52-131">String</span><span class="sxs-lookup"><span data-stu-id="4fc52-131">String</span></span>|<span data-ttu-id="4fc52-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4fc52-132">Key of the entity.</span></span>|
|<span data-ttu-id="4fc52-133">target</span><span class="sxs-lookup"><span data-stu-id="4fc52-133">target</span></span>|[<span data-ttu-id="4fc52-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4fc52-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4fc52-135">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="4fc52-135">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="4fc52-136">source</span><span class="sxs-lookup"><span data-stu-id="4fc52-136">source</span></span>|[<span data-ttu-id="4fc52-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="4fc52-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="4fc52-138">设备合规性策略、direct 或包裹/policySet 的分配源。</span><span class="sxs-lookup"><span data-stu-id="4fc52-138">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="4fc52-139">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="4fc52-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="4fc52-140">sourceId</span><span class="sxs-lookup"><span data-stu-id="4fc52-140">sourceId</span></span>|<span data-ttu-id="4fc52-141">String</span><span class="sxs-lookup"><span data-stu-id="4fc52-141">String</span></span>|<span data-ttu-id="4fc52-142">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="4fc52-142">The identifier of the source of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fc52-143">关系</span><span class="sxs-lookup"><span data-stu-id="4fc52-143">Relationships</span></span>
<span data-ttu-id="4fc52-144">无</span><span class="sxs-lookup"><span data-stu-id="4fc52-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fc52-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4fc52-145">JSON Representation</span></span>
<span data-ttu-id="4fc52-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fc52-146">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



