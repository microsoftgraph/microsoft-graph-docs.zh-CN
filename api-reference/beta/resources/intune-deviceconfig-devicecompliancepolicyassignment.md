---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb3bfaefa074a008ef84728476153791a42c250f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567408"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="5eb79-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eb79-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="5eb79-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5eb79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5eb79-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5eb79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eb79-106">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="5eb79-106">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="5eb79-107">方法</span><span class="sxs-lookup"><span data-stu-id="5eb79-107">Methods</span></span>
|<span data-ttu-id="5eb79-108">方法</span><span class="sxs-lookup"><span data-stu-id="5eb79-108">Method</span></span>|<span data-ttu-id="5eb79-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5eb79-109">Return Type</span></span>|<span data-ttu-id="5eb79-110">说明</span><span class="sxs-lookup"><span data-stu-id="5eb79-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5eb79-111">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="5eb79-111">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="5eb79-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5eb79-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="5eb79-113">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eb79-113">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="5eb79-114">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-114">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="5eb79-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="5eb79-116">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5eb79-116">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="5eb79-117">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-117">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="5eb79-118">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-118">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="5eb79-119">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5eb79-119">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="5eb79-120">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-120">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="5eb79-121">无</span><span class="sxs-lookup"><span data-stu-id="5eb79-121">None</span></span>|<span data-ttu-id="5eb79-122">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5eb79-122">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="5eb79-123">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-123">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="5eb79-124">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="5eb79-124">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="5eb79-125">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5eb79-125">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5eb79-126">属性</span><span class="sxs-lookup"><span data-stu-id="5eb79-126">Properties</span></span>
|<span data-ttu-id="5eb79-127">属性</span><span class="sxs-lookup"><span data-stu-id="5eb79-127">Property</span></span>|<span data-ttu-id="5eb79-128">类型</span><span class="sxs-lookup"><span data-stu-id="5eb79-128">Type</span></span>|<span data-ttu-id="5eb79-129">说明</span><span class="sxs-lookup"><span data-stu-id="5eb79-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb79-130">id</span><span class="sxs-lookup"><span data-stu-id="5eb79-130">id</span></span>|<span data-ttu-id="5eb79-131">String</span><span class="sxs-lookup"><span data-stu-id="5eb79-131">String</span></span>|<span data-ttu-id="5eb79-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5eb79-132">Key of the entity.</span></span>|
|<span data-ttu-id="5eb79-133">target</span><span class="sxs-lookup"><span data-stu-id="5eb79-133">target</span></span>|[<span data-ttu-id="5eb79-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5eb79-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5eb79-135">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="5eb79-135">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eb79-136">关系</span><span class="sxs-lookup"><span data-stu-id="5eb79-136">Relationships</span></span>
<span data-ttu-id="5eb79-137">无</span><span class="sxs-lookup"><span data-stu-id="5eb79-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5eb79-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eb79-138">JSON Representation</span></span>
<span data-ttu-id="5eb79-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eb79-139">Here is a JSON representation of the resource.</span></span>
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





