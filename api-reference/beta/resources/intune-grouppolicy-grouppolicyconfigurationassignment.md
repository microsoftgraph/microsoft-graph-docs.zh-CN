---
title: groupPolicyConfigurationAssignment 资源类型
description: 组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcc3b313ca13c830c4924fa73b1ae09537069301
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793876"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="a974e-103">groupPolicyConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a974e-103">groupPolicyConfigurationAssignment resource type</span></span>

<span data-ttu-id="a974e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a974e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a974e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a974e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a974e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a974e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a974e-107">组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。</span><span class="sxs-lookup"><span data-stu-id="a974e-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="a974e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="a974e-108">Methods</span></span>
|<span data-ttu-id="a974e-109">方法</span><span class="sxs-lookup"><span data-stu-id="a974e-109">Method</span></span>|<span data-ttu-id="a974e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a974e-110">Return Type</span></span>|<span data-ttu-id="a974e-111">说明</span><span class="sxs-lookup"><span data-stu-id="a974e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a974e-112">列出 groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="a974e-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="a974e-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a974e-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a974e-114">列出[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a974e-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="a974e-115">获取 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="a974e-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="a974e-117">读取[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a974e-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a974e-118">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="a974e-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="a974e-120">创建新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a974e-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a974e-121">删除 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="a974e-122">无</span><span class="sxs-lookup"><span data-stu-id="a974e-122">None</span></span>|<span data-ttu-id="a974e-123">删除[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a974e-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="a974e-124">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="a974e-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a974e-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="a974e-126">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a974e-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a974e-127">属性</span><span class="sxs-lookup"><span data-stu-id="a974e-127">Properties</span></span>
|<span data-ttu-id="a974e-128">属性</span><span class="sxs-lookup"><span data-stu-id="a974e-128">Property</span></span>|<span data-ttu-id="a974e-129">类型</span><span class="sxs-lookup"><span data-stu-id="a974e-129">Type</span></span>|<span data-ttu-id="a974e-130">说明</span><span class="sxs-lookup"><span data-stu-id="a974e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a974e-131">id</span><span class="sxs-lookup"><span data-stu-id="a974e-131">id</span></span>|<span data-ttu-id="a974e-132">String</span><span class="sxs-lookup"><span data-stu-id="a974e-132">String</span></span>|<span data-ttu-id="a974e-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a974e-133">Key of the entity.</span></span>|
|<span data-ttu-id="a974e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a974e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="a974e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a974e-135">DateTimeOffset</span></span>|<span data-ttu-id="a974e-136">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a974e-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="a974e-137">target</span><span class="sxs-lookup"><span data-stu-id="a974e-137">target</span></span>|[<span data-ttu-id="a974e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a974e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a974e-139">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="a974e-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a974e-140">关系</span><span class="sxs-lookup"><span data-stu-id="a974e-140">Relationships</span></span>
<span data-ttu-id="a974e-141">无</span><span class="sxs-lookup"><span data-stu-id="a974e-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a974e-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a974e-142">JSON Representation</span></span>
<span data-ttu-id="a974e-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a974e-143">Here is a JSON representation of the resource.</span></span>
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



