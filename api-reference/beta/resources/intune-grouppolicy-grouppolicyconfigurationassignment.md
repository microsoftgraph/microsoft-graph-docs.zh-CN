---
title: groupPolicyConfigurationAssignment 资源类型
description: 组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe21e130a870225b7e0b96c3926f1115361bde0e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256132"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="af0d8-103">groupPolicyConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="af0d8-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="af0d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af0d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af0d8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af0d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af0d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af0d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af0d8-107">组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。</span><span class="sxs-lookup"><span data-stu-id="af0d8-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="af0d8-108">方法</span><span class="sxs-lookup"><span data-stu-id="af0d8-108">Methods</span></span>
|<span data-ttu-id="af0d8-109">方法</span><span class="sxs-lookup"><span data-stu-id="af0d8-109">Method</span></span>|<span data-ttu-id="af0d8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="af0d8-110">Return Type</span></span>|<span data-ttu-id="af0d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="af0d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af0d8-112">列出 groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="af0d8-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="af0d8-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af0d8-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="af0d8-114">列出 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af0d8-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="af0d8-115">获取 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="af0d8-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="af0d8-117">读取 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af0d8-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="af0d8-118">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="af0d8-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="af0d8-120">创建新的 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af0d8-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="af0d8-121">删除 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="af0d8-122">无</span><span class="sxs-lookup"><span data-stu-id="af0d8-122">None</span></span>|<span data-ttu-id="af0d8-123">删除 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="af0d8-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="af0d8-124">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="af0d8-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="af0d8-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="af0d8-126">更新 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="af0d8-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af0d8-127">属性</span><span class="sxs-lookup"><span data-stu-id="af0d8-127">Properties</span></span>
|<span data-ttu-id="af0d8-128">属性</span><span class="sxs-lookup"><span data-stu-id="af0d8-128">Property</span></span>|<span data-ttu-id="af0d8-129">类型</span><span class="sxs-lookup"><span data-stu-id="af0d8-129">Type</span></span>|<span data-ttu-id="af0d8-130">说明</span><span class="sxs-lookup"><span data-stu-id="af0d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af0d8-131">id</span><span class="sxs-lookup"><span data-stu-id="af0d8-131">id</span></span>|<span data-ttu-id="af0d8-132">String</span><span class="sxs-lookup"><span data-stu-id="af0d8-132">String</span></span>|<span data-ttu-id="af0d8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af0d8-133">Key of the entity.</span></span>|
|<span data-ttu-id="af0d8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af0d8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="af0d8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af0d8-135">DateTimeOffset</span></span>|<span data-ttu-id="af0d8-136">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af0d8-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="af0d8-137">target</span><span class="sxs-lookup"><span data-stu-id="af0d8-137">target</span></span>|[<span data-ttu-id="af0d8-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="af0d8-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="af0d8-139">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="af0d8-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af0d8-140">关系</span><span class="sxs-lookup"><span data-stu-id="af0d8-140">Relationships</span></span>
<span data-ttu-id="af0d8-141">无</span><span class="sxs-lookup"><span data-stu-id="af0d8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af0d8-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af0d8-142">JSON Representation</span></span>
<span data-ttu-id="af0d8-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af0d8-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




