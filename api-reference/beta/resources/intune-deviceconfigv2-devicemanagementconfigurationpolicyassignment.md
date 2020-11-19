---
title: deviceManagementConfigurationPolicyAssignment 资源类型
description: DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4247518598cc9094346814079be37fc5d6073286
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241286"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a><span data-ttu-id="214e3-103">deviceManagementConfigurationPolicyAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="214e3-103">deviceManagementConfigurationPolicyAssignment resource type</span></span>

<span data-ttu-id="214e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="214e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="214e3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="214e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="214e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="214e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="214e3-107">DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="214e3-107">The DeviceManagementConfigurationPolicyAssignment entity assigns a specific DeviceManagementConfigurationPolicy to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="214e3-108">方法</span><span class="sxs-lookup"><span data-stu-id="214e3-108">Methods</span></span>
|<span data-ttu-id="214e3-109">方法</span><span class="sxs-lookup"><span data-stu-id="214e3-109">Method</span></span>|<span data-ttu-id="214e3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="214e3-110">Return Type</span></span>|<span data-ttu-id="214e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="214e3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="214e3-112">列出 deviceManagementConfigurationPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="214e3-112">List deviceManagementConfigurationPolicyAssignments</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|<span data-ttu-id="214e3-113">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="214e3-113">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="214e3-114">列出 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="214e3-114">List properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="214e3-115">获取 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-115">Get deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[<span data-ttu-id="214e3-116">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-116">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="214e3-117">读取 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="214e3-117">Read properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="214e3-118">创建 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-118">Create deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[<span data-ttu-id="214e3-119">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-119">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="214e3-120">创建新的 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="214e3-120">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="214e3-121">删除 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-121">Delete deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|<span data-ttu-id="214e3-122">无</span><span class="sxs-lookup"><span data-stu-id="214e3-122">None</span></span>|<span data-ttu-id="214e3-123">删除 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="214e3-123">Deletes a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>|
|[<span data-ttu-id="214e3-124">更新 deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-124">Update deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[<span data-ttu-id="214e3-125">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="214e3-125">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="214e3-126">更新 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="214e3-126">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="214e3-127">属性</span><span class="sxs-lookup"><span data-stu-id="214e3-127">Properties</span></span>
|<span data-ttu-id="214e3-128">属性</span><span class="sxs-lookup"><span data-stu-id="214e3-128">Property</span></span>|<span data-ttu-id="214e3-129">类型</span><span class="sxs-lookup"><span data-stu-id="214e3-129">Type</span></span>|<span data-ttu-id="214e3-130">说明</span><span class="sxs-lookup"><span data-stu-id="214e3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="214e3-131">id</span><span class="sxs-lookup"><span data-stu-id="214e3-131">id</span></span>|<span data-ttu-id="214e3-132">String</span><span class="sxs-lookup"><span data-stu-id="214e3-132">String</span></span>|<span data-ttu-id="214e3-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="214e3-133">The key of the assignment.</span></span>|
|<span data-ttu-id="214e3-134">target</span><span class="sxs-lookup"><span data-stu-id="214e3-134">target</span></span>|[<span data-ttu-id="214e3-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="214e3-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="214e3-136">DeviceManagementConfigurationPolicy 的分配目标。</span><span class="sxs-lookup"><span data-stu-id="214e3-136">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="214e3-137">关系</span><span class="sxs-lookup"><span data-stu-id="214e3-137">Relationships</span></span>
<span data-ttu-id="214e3-138">无</span><span class="sxs-lookup"><span data-stu-id="214e3-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="214e3-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="214e3-139">JSON Representation</span></span>
<span data-ttu-id="214e3-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="214e3-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




