---
title: deviceManagementConfigurationPolicyAssignment 资源类型
description: DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e571983c36c2832aef5c43478d1cccca7361aca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157664"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a><span data-ttu-id="95bff-103">deviceManagementConfigurationPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="95bff-103">deviceManagementConfigurationPolicyAssignment resource type</span></span>

<span data-ttu-id="95bff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95bff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95bff-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95bff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95bff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95bff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95bff-107">DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="95bff-107">The DeviceManagementConfigurationPolicyAssignment entity assigns a specific DeviceManagementConfigurationPolicy to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="95bff-108">方法</span><span class="sxs-lookup"><span data-stu-id="95bff-108">Methods</span></span>
|<span data-ttu-id="95bff-109">方法</span><span class="sxs-lookup"><span data-stu-id="95bff-109">Method</span></span>|<span data-ttu-id="95bff-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="95bff-110">Return Type</span></span>|<span data-ttu-id="95bff-111">说明</span><span class="sxs-lookup"><span data-stu-id="95bff-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95bff-112">列出 deviceManagementConfigurationPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="95bff-112">List deviceManagementConfigurationPolicyAssignments</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|<span data-ttu-id="95bff-113">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95bff-113">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="95bff-114">列出 [deviceManagementConfigurationPolicyAssignment 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="95bff-114">List properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="95bff-115">获取 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-115">Get deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[<span data-ttu-id="95bff-116">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-116">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="95bff-117">读取 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95bff-117">Read properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="95bff-118">创建 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-118">Create deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[<span data-ttu-id="95bff-119">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-119">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="95bff-120">创建新的 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95bff-120">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="95bff-121">删除 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-121">Delete deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|<span data-ttu-id="95bff-122">无</span><span class="sxs-lookup"><span data-stu-id="95bff-122">None</span></span>|<span data-ttu-id="95bff-123">删除 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="95bff-123">Deletes a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>|
|[<span data-ttu-id="95bff-124">更新 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-124">Update deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[<span data-ttu-id="95bff-125">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95bff-125">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="95bff-126">更新 [deviceManagementConfigurationPolicyAssignment 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="95bff-126">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="95bff-127">属性</span><span class="sxs-lookup"><span data-stu-id="95bff-127">Properties</span></span>
|<span data-ttu-id="95bff-128">属性</span><span class="sxs-lookup"><span data-stu-id="95bff-128">Property</span></span>|<span data-ttu-id="95bff-129">类型</span><span class="sxs-lookup"><span data-stu-id="95bff-129">Type</span></span>|<span data-ttu-id="95bff-130">说明</span><span class="sxs-lookup"><span data-stu-id="95bff-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95bff-131">id</span><span class="sxs-lookup"><span data-stu-id="95bff-131">id</span></span>|<span data-ttu-id="95bff-132">String</span><span class="sxs-lookup"><span data-stu-id="95bff-132">String</span></span>|<span data-ttu-id="95bff-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="95bff-133">The key of the assignment.</span></span>|
|<span data-ttu-id="95bff-134">target</span><span class="sxs-lookup"><span data-stu-id="95bff-134">target</span></span>|[<span data-ttu-id="95bff-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="95bff-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="95bff-136">DeviceManagementConfigurationPolicy 的分配目标。</span><span class="sxs-lookup"><span data-stu-id="95bff-136">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95bff-137">关系</span><span class="sxs-lookup"><span data-stu-id="95bff-137">Relationships</span></span>
<span data-ttu-id="95bff-138">无</span><span class="sxs-lookup"><span data-stu-id="95bff-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95bff-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95bff-139">JSON Representation</span></span>
<span data-ttu-id="95bff-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95bff-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




