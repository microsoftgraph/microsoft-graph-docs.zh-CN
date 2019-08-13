---
title: groupPolicyConfigurationAssignment 资源类型
description: 组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82101853def989bad8b80794d176b7d2bca2582b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331516"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="edfb1-103">groupPolicyConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="edfb1-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="edfb1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edfb1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edfb1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edfb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfb1-106">组策略配置分配实体将一个或多个 AAD 组分配给特定的组策略配置。</span><span class="sxs-lookup"><span data-stu-id="edfb1-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="edfb1-107">方法</span><span class="sxs-lookup"><span data-stu-id="edfb1-107">Methods</span></span>
|<span data-ttu-id="edfb1-108">方法</span><span class="sxs-lookup"><span data-stu-id="edfb1-108">Method</span></span>|<span data-ttu-id="edfb1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="edfb1-109">Return Type</span></span>|<span data-ttu-id="edfb1-110">说明</span><span class="sxs-lookup"><span data-stu-id="edfb1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="edfb1-111">列出 groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="edfb1-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="edfb1-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="edfb1-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="edfb1-113">列出[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="edfb1-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="edfb1-114">获取 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="edfb1-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="edfb1-116">读取[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="edfb1-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="edfb1-117">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="edfb1-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="edfb1-119">创建新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="edfb1-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="edfb1-120">删除 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="edfb1-121">无</span><span class="sxs-lookup"><span data-stu-id="edfb1-121">None</span></span>|<span data-ttu-id="edfb1-122">删除[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="edfb1-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="edfb1-123">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="edfb1-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="edfb1-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="edfb1-125">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="edfb1-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="edfb1-126">属性</span><span class="sxs-lookup"><span data-stu-id="edfb1-126">Properties</span></span>
|<span data-ttu-id="edfb1-127">属性</span><span class="sxs-lookup"><span data-stu-id="edfb1-127">Property</span></span>|<span data-ttu-id="edfb1-128">类型</span><span class="sxs-lookup"><span data-stu-id="edfb1-128">Type</span></span>|<span data-ttu-id="edfb1-129">说明</span><span class="sxs-lookup"><span data-stu-id="edfb1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfb1-130">id</span><span class="sxs-lookup"><span data-stu-id="edfb1-130">id</span></span>|<span data-ttu-id="edfb1-131">String</span><span class="sxs-lookup"><span data-stu-id="edfb1-131">String</span></span>|<span data-ttu-id="edfb1-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="edfb1-132">Key of the entity.</span></span>|
|<span data-ttu-id="edfb1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edfb1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="edfb1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfb1-134">DateTimeOffset</span></span>|<span data-ttu-id="edfb1-135">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="edfb1-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="edfb1-136">target</span><span class="sxs-lookup"><span data-stu-id="edfb1-136">target</span></span>|[<span data-ttu-id="edfb1-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="edfb1-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="edfb1-138">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="edfb1-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edfb1-139">关系</span><span class="sxs-lookup"><span data-stu-id="edfb1-139">Relationships</span></span>
<span data-ttu-id="edfb1-140">无</span><span class="sxs-lookup"><span data-stu-id="edfb1-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edfb1-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edfb1-141">JSON Representation</span></span>
<span data-ttu-id="edfb1-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edfb1-142">Here is a JSON representation of the resource.</span></span>
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



