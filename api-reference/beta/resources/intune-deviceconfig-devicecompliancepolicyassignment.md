---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb90240e83bb3e811b0eff09966346f801a1637
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415605"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="dca09-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="dca09-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="dca09-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="dca09-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dca09-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dca09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dca09-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dca09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca09-107">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="dca09-107">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="dca09-108">方法</span><span class="sxs-lookup"><span data-stu-id="dca09-108">Methods</span></span>
|<span data-ttu-id="dca09-109">方法</span><span class="sxs-lookup"><span data-stu-id="dca09-109">Method</span></span>|<span data-ttu-id="dca09-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dca09-110">Return Type</span></span>|<span data-ttu-id="dca09-111">说明</span><span class="sxs-lookup"><span data-stu-id="dca09-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dca09-112">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="dca09-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="dca09-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dca09-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="dca09-114">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dca09-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="dca09-115">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="dca09-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="dca09-117">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dca09-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="dca09-118">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="dca09-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="dca09-120">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dca09-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="dca09-121">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="dca09-122">无</span><span class="sxs-lookup"><span data-stu-id="dca09-122">None</span></span>|<span data-ttu-id="dca09-123">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="dca09-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="dca09-124">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="dca09-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="dca09-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="dca09-126">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dca09-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dca09-127">属性</span><span class="sxs-lookup"><span data-stu-id="dca09-127">Properties</span></span>
|<span data-ttu-id="dca09-128">属性</span><span class="sxs-lookup"><span data-stu-id="dca09-128">Property</span></span>|<span data-ttu-id="dca09-129">类型</span><span class="sxs-lookup"><span data-stu-id="dca09-129">Type</span></span>|<span data-ttu-id="dca09-130">说明</span><span class="sxs-lookup"><span data-stu-id="dca09-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca09-131">id</span><span class="sxs-lookup"><span data-stu-id="dca09-131">id</span></span>|<span data-ttu-id="dca09-132">String</span><span class="sxs-lookup"><span data-stu-id="dca09-132">String</span></span>|<span data-ttu-id="dca09-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dca09-133">Key of the entity.</span></span>|
|<span data-ttu-id="dca09-134">target</span><span class="sxs-lookup"><span data-stu-id="dca09-134">target</span></span>|[<span data-ttu-id="dca09-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dca09-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dca09-136">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="dca09-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca09-137">关系</span><span class="sxs-lookup"><span data-stu-id="dca09-137">Relationships</span></span>
<span data-ttu-id="dca09-138">无</span><span class="sxs-lookup"><span data-stu-id="dca09-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dca09-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dca09-139">JSON Representation</span></span>
<span data-ttu-id="dca09-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dca09-140">Here is a JSON representation of the resource.</span></span>
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




