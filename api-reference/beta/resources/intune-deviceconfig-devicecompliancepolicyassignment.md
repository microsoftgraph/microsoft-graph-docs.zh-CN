---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7be0c5f321c6ea5cac125f3a0785a057ad216716
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538901"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="35fe5-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="35fe5-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="35fe5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35fe5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35fe5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35fe5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35fe5-106">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="35fe5-106">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="35fe5-107">方法</span><span class="sxs-lookup"><span data-stu-id="35fe5-107">Methods</span></span>
|<span data-ttu-id="35fe5-108">方法</span><span class="sxs-lookup"><span data-stu-id="35fe5-108">Method</span></span>|<span data-ttu-id="35fe5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="35fe5-109">Return Type</span></span>|<span data-ttu-id="35fe5-110">说明</span><span class="sxs-lookup"><span data-stu-id="35fe5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35fe5-111">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="35fe5-111">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="35fe5-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35fe5-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="35fe5-113">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35fe5-113">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="35fe5-114">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-114">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="35fe5-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="35fe5-116">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35fe5-116">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="35fe5-117">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-117">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="35fe5-118">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-118">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="35fe5-119">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35fe5-119">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="35fe5-120">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-120">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="35fe5-121">无</span><span class="sxs-lookup"><span data-stu-id="35fe5-121">None</span></span>|<span data-ttu-id="35fe5-122">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="35fe5-122">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="35fe5-123">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-123">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="35fe5-124">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="35fe5-124">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="35fe5-125">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35fe5-125">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35fe5-126">属性</span><span class="sxs-lookup"><span data-stu-id="35fe5-126">Properties</span></span>
|<span data-ttu-id="35fe5-127">属性</span><span class="sxs-lookup"><span data-stu-id="35fe5-127">Property</span></span>|<span data-ttu-id="35fe5-128">类型</span><span class="sxs-lookup"><span data-stu-id="35fe5-128">Type</span></span>|<span data-ttu-id="35fe5-129">说明</span><span class="sxs-lookup"><span data-stu-id="35fe5-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35fe5-130">id</span><span class="sxs-lookup"><span data-stu-id="35fe5-130">id</span></span>|<span data-ttu-id="35fe5-131">字符串</span><span class="sxs-lookup"><span data-stu-id="35fe5-131">String</span></span>|<span data-ttu-id="35fe5-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="35fe5-132">Key of the entity.</span></span>|
|<span data-ttu-id="35fe5-133">target</span><span class="sxs-lookup"><span data-stu-id="35fe5-133">target</span></span>|[<span data-ttu-id="35fe5-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="35fe5-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="35fe5-135">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="35fe5-135">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="35fe5-136">source</span><span class="sxs-lookup"><span data-stu-id="35fe5-136">source</span></span>|[<span data-ttu-id="35fe5-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="35fe5-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="35fe5-138">设备合规性策略、direct 或包裹/policySet 的分配源。</span><span class="sxs-lookup"><span data-stu-id="35fe5-138">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="35fe5-139">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="35fe5-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="35fe5-140">sourceId</span><span class="sxs-lookup"><span data-stu-id="35fe5-140">sourceId</span></span>|<span data-ttu-id="35fe5-141">字符串</span><span class="sxs-lookup"><span data-stu-id="35fe5-141">String</span></span>|<span data-ttu-id="35fe5-142">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="35fe5-142">The identifier of the source of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35fe5-143">关系</span><span class="sxs-lookup"><span data-stu-id="35fe5-143">Relationships</span></span>
<span data-ttu-id="35fe5-144">无</span><span class="sxs-lookup"><span data-stu-id="35fe5-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35fe5-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35fe5-145">JSON Representation</span></span>
<span data-ttu-id="35fe5-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35fe5-146">Here is a JSON representation of the resource.</span></span>
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



