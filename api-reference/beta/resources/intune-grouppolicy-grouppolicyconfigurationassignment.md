---
title: groupPolicyConfigurationAssignment 资源类型
description: 组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b113b7570726efacd3c6dc2691ef0d11a4795784
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031058"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="66842-103">groupPolicyConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="66842-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="66842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66842-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66842-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66842-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66842-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66842-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66842-107">组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。</span><span class="sxs-lookup"><span data-stu-id="66842-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="66842-108">方法</span><span class="sxs-lookup"><span data-stu-id="66842-108">Methods</span></span>
|<span data-ttu-id="66842-109">方法</span><span class="sxs-lookup"><span data-stu-id="66842-109">Method</span></span>|<span data-ttu-id="66842-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="66842-110">Return Type</span></span>|<span data-ttu-id="66842-111">说明</span><span class="sxs-lookup"><span data-stu-id="66842-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66842-112">列出 groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="66842-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="66842-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66842-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="66842-114">列出 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66842-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="66842-115">获取 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="66842-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="66842-117">读取 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66842-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="66842-118">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="66842-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="66842-120">创建新的 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66842-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="66842-121">删除 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="66842-122">无</span><span class="sxs-lookup"><span data-stu-id="66842-122">None</span></span>|<span data-ttu-id="66842-123">删除 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="66842-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="66842-124">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="66842-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66842-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="66842-126">更新 [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="66842-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="66842-127">属性</span><span class="sxs-lookup"><span data-stu-id="66842-127">Properties</span></span>
|<span data-ttu-id="66842-128">属性</span><span class="sxs-lookup"><span data-stu-id="66842-128">Property</span></span>|<span data-ttu-id="66842-129">类型</span><span class="sxs-lookup"><span data-stu-id="66842-129">Type</span></span>|<span data-ttu-id="66842-130">说明</span><span class="sxs-lookup"><span data-stu-id="66842-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66842-131">id</span><span class="sxs-lookup"><span data-stu-id="66842-131">id</span></span>|<span data-ttu-id="66842-132">String</span><span class="sxs-lookup"><span data-stu-id="66842-132">String</span></span>|<span data-ttu-id="66842-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="66842-133">Key of the entity.</span></span>|
|<span data-ttu-id="66842-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66842-134">lastModifiedDateTime</span></span>|<span data-ttu-id="66842-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66842-135">DateTimeOffset</span></span>|<span data-ttu-id="66842-136">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66842-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="66842-137">target</span><span class="sxs-lookup"><span data-stu-id="66842-137">target</span></span>|[<span data-ttu-id="66842-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="66842-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="66842-139">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="66842-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66842-140">关系</span><span class="sxs-lookup"><span data-stu-id="66842-140">Relationships</span></span>
<span data-ttu-id="66842-141">无</span><span class="sxs-lookup"><span data-stu-id="66842-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66842-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66842-142">JSON Representation</span></span>
<span data-ttu-id="66842-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66842-143">Here is a JSON representation of the resource.</span></span>
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






