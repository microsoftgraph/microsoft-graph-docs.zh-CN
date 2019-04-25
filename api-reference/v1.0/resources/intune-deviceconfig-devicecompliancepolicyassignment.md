---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d327288ca08f43c36b20cefd8608b860529420
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534246"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="d0a3c-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0a3c-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="d0a3c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0a3c-105">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-105">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="d0a3c-106">方法</span><span class="sxs-lookup"><span data-stu-id="d0a3c-106">Methods</span></span>
|<span data-ttu-id="d0a3c-107">方法</span><span class="sxs-lookup"><span data-stu-id="d0a3c-107">Method</span></span>|<span data-ttu-id="d0a3c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0a3c-108">Return Type</span></span>|<span data-ttu-id="d0a3c-109">说明</span><span class="sxs-lookup"><span data-stu-id="d0a3c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0a3c-110">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="d0a3c-110">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="d0a3c-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0a3c-111">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="d0a3c-112">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-112">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="d0a3c-113">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-113">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="d0a3c-114">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-114">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d0a3c-115">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-115">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="d0a3c-116">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-116">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="d0a3c-117">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-117">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d0a3c-118">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-118">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="d0a3c-119">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-119">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="d0a3c-120">无</span><span class="sxs-lookup"><span data-stu-id="d0a3c-120">None</span></span>|<span data-ttu-id="d0a3c-121">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-121">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="d0a3c-122">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-122">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="d0a3c-123">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d0a3c-123">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d0a3c-124">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-124">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0a3c-125">属性</span><span class="sxs-lookup"><span data-stu-id="d0a3c-125">Properties</span></span>
|<span data-ttu-id="d0a3c-126">属性</span><span class="sxs-lookup"><span data-stu-id="d0a3c-126">Property</span></span>|<span data-ttu-id="d0a3c-127">类型</span><span class="sxs-lookup"><span data-stu-id="d0a3c-127">Type</span></span>|<span data-ttu-id="d0a3c-128">说明</span><span class="sxs-lookup"><span data-stu-id="d0a3c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0a3c-129">id</span><span class="sxs-lookup"><span data-stu-id="d0a3c-129">id</span></span>|<span data-ttu-id="d0a3c-130">String</span><span class="sxs-lookup"><span data-stu-id="d0a3c-130">String</span></span>|<span data-ttu-id="d0a3c-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-131">Key of the entity.</span></span>|
|<span data-ttu-id="d0a3c-132">target</span><span class="sxs-lookup"><span data-stu-id="d0a3c-132">target</span></span>|[<span data-ttu-id="d0a3c-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0a3c-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d0a3c-134">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-134">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0a3c-135">关系</span><span class="sxs-lookup"><span data-stu-id="d0a3c-135">Relationships</span></span>
<span data-ttu-id="d0a3c-136">无</span><span class="sxs-lookup"><span data-stu-id="d0a3c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0a3c-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0a3c-137">JSON Representation</span></span>
<span data-ttu-id="d0a3c-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0a3c-138">Here is a JSON representation of the resource.</span></span>
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
  }
}
```



