---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f7664b660952b2e70b7337ea5313834ca7d009c9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158245"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="e30b1-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e30b1-103">deviceCompliancePolicyAssignment resource type</span></span>

<span data-ttu-id="e30b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e30b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e30b1-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e30b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e30b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e30b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e30b1-107">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="e30b1-107">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="e30b1-108">方法</span><span class="sxs-lookup"><span data-stu-id="e30b1-108">Methods</span></span>
|<span data-ttu-id="e30b1-109">方法</span><span class="sxs-lookup"><span data-stu-id="e30b1-109">Method</span></span>|<span data-ttu-id="e30b1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e30b1-110">Return Type</span></span>|<span data-ttu-id="e30b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="e30b1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e30b1-112">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="e30b1-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="e30b1-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e30b1-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="e30b1-114">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e30b1-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="e30b1-115">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="e30b1-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="e30b1-117">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e30b1-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="e30b1-118">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="e30b1-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="e30b1-120">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e30b1-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="e30b1-121">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="e30b1-122">无</span><span class="sxs-lookup"><span data-stu-id="e30b1-122">None</span></span>|<span data-ttu-id="e30b1-123">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="e30b1-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="e30b1-124">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="e30b1-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e30b1-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="e30b1-126">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e30b1-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e30b1-127">属性</span><span class="sxs-lookup"><span data-stu-id="e30b1-127">Properties</span></span>
|<span data-ttu-id="e30b1-128">属性</span><span class="sxs-lookup"><span data-stu-id="e30b1-128">Property</span></span>|<span data-ttu-id="e30b1-129">类型</span><span class="sxs-lookup"><span data-stu-id="e30b1-129">Type</span></span>|<span data-ttu-id="e30b1-130">说明</span><span class="sxs-lookup"><span data-stu-id="e30b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e30b1-131">id</span><span class="sxs-lookup"><span data-stu-id="e30b1-131">id</span></span>|<span data-ttu-id="e30b1-132">String</span><span class="sxs-lookup"><span data-stu-id="e30b1-132">String</span></span>|<span data-ttu-id="e30b1-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e30b1-133">Key of the entity.</span></span>|
|<span data-ttu-id="e30b1-134">target</span><span class="sxs-lookup"><span data-stu-id="e30b1-134">target</span></span>|[<span data-ttu-id="e30b1-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e30b1-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e30b1-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="e30b1-136">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="e30b1-137">source</span><span class="sxs-lookup"><span data-stu-id="e30b1-137">source</span></span>|[<span data-ttu-id="e30b1-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="e30b1-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="e30b1-139">设备合规性策略的分配源：direct 或/policySet。</span><span class="sxs-lookup"><span data-stu-id="e30b1-139">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="e30b1-140">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="e30b1-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="e30b1-141">sourceId</span><span class="sxs-lookup"><span data-stu-id="e30b1-141">sourceId</span></span>|<span data-ttu-id="e30b1-142">String</span><span class="sxs-lookup"><span data-stu-id="e30b1-142">String</span></span>|<span data-ttu-id="e30b1-143">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="e30b1-143">The identifier of the source of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e30b1-144">关系</span><span class="sxs-lookup"><span data-stu-id="e30b1-144">Relationships</span></span>
<span data-ttu-id="e30b1-145">无</span><span class="sxs-lookup"><span data-stu-id="e30b1-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e30b1-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e30b1-146">JSON Representation</span></span>
<span data-ttu-id="e30b1-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e30b1-147">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




