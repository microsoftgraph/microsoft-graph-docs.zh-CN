---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 680fea1ccbe65405983baf37100b8ca7211852a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530824"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="81e4c-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="81e4c-103">deviceCompliancePolicyAssignment resource type</span></span>

<span data-ttu-id="81e4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81e4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81e4c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81e4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81e4c-106">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="81e4c-106">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="81e4c-107">Methods</span><span class="sxs-lookup"><span data-stu-id="81e4c-107">Methods</span></span>
|<span data-ttu-id="81e4c-108">方法</span><span class="sxs-lookup"><span data-stu-id="81e4c-108">Method</span></span>|<span data-ttu-id="81e4c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="81e4c-109">Return Type</span></span>|<span data-ttu-id="81e4c-110">说明</span><span class="sxs-lookup"><span data-stu-id="81e4c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81e4c-111">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="81e4c-111">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="81e4c-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81e4c-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="81e4c-113">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81e4c-113">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="81e4c-114">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-114">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="81e4c-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="81e4c-116">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81e4c-116">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="81e4c-117">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-117">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="81e4c-118">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-118">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="81e4c-119">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81e4c-119">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="81e4c-120">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-120">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="81e4c-121">无</span><span class="sxs-lookup"><span data-stu-id="81e4c-121">None</span></span>|<span data-ttu-id="81e4c-122">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="81e4c-122">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="81e4c-123">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-123">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="81e4c-124">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="81e4c-124">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="81e4c-125">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="81e4c-125">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81e4c-126">属性</span><span class="sxs-lookup"><span data-stu-id="81e4c-126">Properties</span></span>
|<span data-ttu-id="81e4c-127">属性</span><span class="sxs-lookup"><span data-stu-id="81e4c-127">Property</span></span>|<span data-ttu-id="81e4c-128">类型</span><span class="sxs-lookup"><span data-stu-id="81e4c-128">Type</span></span>|<span data-ttu-id="81e4c-129">说明</span><span class="sxs-lookup"><span data-stu-id="81e4c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e4c-130">id</span><span class="sxs-lookup"><span data-stu-id="81e4c-130">id</span></span>|<span data-ttu-id="81e4c-131">字符串</span><span class="sxs-lookup"><span data-stu-id="81e4c-131">String</span></span>|<span data-ttu-id="81e4c-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81e4c-132">Key of the entity.</span></span>|
|<span data-ttu-id="81e4c-133">target</span><span class="sxs-lookup"><span data-stu-id="81e4c-133">target</span></span>|[<span data-ttu-id="81e4c-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="81e4c-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="81e4c-135">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="81e4c-135">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81e4c-136">关系</span><span class="sxs-lookup"><span data-stu-id="81e4c-136">Relationships</span></span>
<span data-ttu-id="81e4c-137">无</span><span class="sxs-lookup"><span data-stu-id="81e4c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81e4c-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81e4c-138">JSON Representation</span></span>
<span data-ttu-id="81e4c-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81e4c-139">Here is a JSON representation of the resource.</span></span>
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




