---
title: deviceCompliancePolicyAssignment 资源类型
description: 设备符合性策略分配。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d1482521f7de5b6cc64c1b467b16ed4a04158a8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947153"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="d2fa8-103">deviceCompliancePolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2fa8-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="d2fa8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2fa8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2fa8-106">设备符合性策略分配。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-106">Device compliance policy assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="d2fa8-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2fa8-107">Methods</span></span>
|<span data-ttu-id="d2fa8-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2fa8-108">Method</span></span>|<span data-ttu-id="d2fa8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2fa8-109">Return Type</span></span>|<span data-ttu-id="d2fa8-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2fa8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2fa8-111">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="d2fa8-111">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="d2fa8-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2fa8-112">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="d2fa8-113">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-113">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="d2fa8-114">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-114">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="d2fa8-115">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-115">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d2fa8-116">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-116">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="d2fa8-117">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-117">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="d2fa8-118">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-118">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d2fa8-119">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-119">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="d2fa8-120">删除 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-120">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="d2fa8-121">无</span><span class="sxs-lookup"><span data-stu-id="d2fa8-121">None</span></span>|<span data-ttu-id="d2fa8-122">删除 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-122">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="d2fa8-123">更新 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-123">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="d2fa8-124">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d2fa8-124">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="d2fa8-125">更新 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-125">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2fa8-126">属性</span><span class="sxs-lookup"><span data-stu-id="d2fa8-126">Properties</span></span>
|<span data-ttu-id="d2fa8-127">属性</span><span class="sxs-lookup"><span data-stu-id="d2fa8-127">Property</span></span>|<span data-ttu-id="d2fa8-128">类型</span><span class="sxs-lookup"><span data-stu-id="d2fa8-128">Type</span></span>|<span data-ttu-id="d2fa8-129">说明</span><span class="sxs-lookup"><span data-stu-id="d2fa8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2fa8-130">id</span><span class="sxs-lookup"><span data-stu-id="d2fa8-130">id</span></span>|<span data-ttu-id="d2fa8-131">String</span><span class="sxs-lookup"><span data-stu-id="d2fa8-131">String</span></span>|<span data-ttu-id="d2fa8-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-132">Key of the entity.</span></span>|
|<span data-ttu-id="d2fa8-133">target</span><span class="sxs-lookup"><span data-stu-id="d2fa8-133">target</span></span>|[<span data-ttu-id="d2fa8-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d2fa8-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d2fa8-135">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-135">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2fa8-136">关系</span><span class="sxs-lookup"><span data-stu-id="d2fa8-136">Relationships</span></span>
<span data-ttu-id="d2fa8-137">无</span><span class="sxs-lookup"><span data-stu-id="d2fa8-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2fa8-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2fa8-138">JSON Representation</span></span>
<span data-ttu-id="d2fa8-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2fa8-139">Here is a JSON representation of the resource.</span></span>
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




