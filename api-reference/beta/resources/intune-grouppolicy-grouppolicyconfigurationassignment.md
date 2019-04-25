---
title: groupPolicyConfigurationAssignment 资源类型
description: 组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6fcd7ace912075189ec3e9b5a817181dd392a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575819"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="49f88-103">groupPolicyConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="49f88-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="49f88-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49f88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49f88-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49f88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49f88-106">组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。</span><span class="sxs-lookup"><span data-stu-id="49f88-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="49f88-107">方法</span><span class="sxs-lookup"><span data-stu-id="49f88-107">Methods</span></span>
|<span data-ttu-id="49f88-108">方法</span><span class="sxs-lookup"><span data-stu-id="49f88-108">Method</span></span>|<span data-ttu-id="49f88-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="49f88-109">Return Type</span></span>|<span data-ttu-id="49f88-110">说明</span><span class="sxs-lookup"><span data-stu-id="49f88-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49f88-111">列出 groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="49f88-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="49f88-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="49f88-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="49f88-113">列出[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49f88-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="49f88-114">获取 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="49f88-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="49f88-116">读取[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49f88-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="49f88-117">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="49f88-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="49f88-119">创建新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49f88-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="49f88-120">删除 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="49f88-121">无</span><span class="sxs-lookup"><span data-stu-id="49f88-121">None</span></span>|<span data-ttu-id="49f88-122">删除[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="49f88-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="49f88-123">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="49f88-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="49f88-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="49f88-125">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="49f88-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="49f88-126">属性</span><span class="sxs-lookup"><span data-stu-id="49f88-126">Properties</span></span>
|<span data-ttu-id="49f88-127">属性</span><span class="sxs-lookup"><span data-stu-id="49f88-127">Property</span></span>|<span data-ttu-id="49f88-128">类型</span><span class="sxs-lookup"><span data-stu-id="49f88-128">Type</span></span>|<span data-ttu-id="49f88-129">说明</span><span class="sxs-lookup"><span data-stu-id="49f88-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f88-130">id</span><span class="sxs-lookup"><span data-stu-id="49f88-130">id</span></span>|<span data-ttu-id="49f88-131">String</span><span class="sxs-lookup"><span data-stu-id="49f88-131">String</span></span>|<span data-ttu-id="49f88-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="49f88-132">Key of the entity.</span></span>|
|<span data-ttu-id="49f88-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49f88-133">lastModifiedDateTime</span></span>|<span data-ttu-id="49f88-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49f88-134">DateTimeOffset</span></span>|<span data-ttu-id="49f88-135">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="49f88-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="49f88-136">target</span><span class="sxs-lookup"><span data-stu-id="49f88-136">target</span></span>|[<span data-ttu-id="49f88-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="49f88-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="49f88-138">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="49f88-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49f88-139">关系</span><span class="sxs-lookup"><span data-stu-id="49f88-139">Relationships</span></span>
<span data-ttu-id="49f88-140">无</span><span class="sxs-lookup"><span data-stu-id="49f88-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49f88-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49f88-141">JSON Representation</span></span>
<span data-ttu-id="49f88-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49f88-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





