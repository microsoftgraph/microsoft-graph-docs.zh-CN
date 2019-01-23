---
title: groupPolicyConfigurationAssignment 资源类型
description: 组策略配置工作分配实体将一个或多个 AAD 组分配给特定的组策略配置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 508581ba7b5ac689338c179f4f6b211928c9abaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429361"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="c5020-103">groupPolicyConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5020-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="c5020-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c5020-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5020-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5020-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5020-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5020-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5020-107">组策略配置工作分配实体将一个或多个 AAD 组分配给特定的组策略配置。</span><span class="sxs-lookup"><span data-stu-id="c5020-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c5020-108">方法</span><span class="sxs-lookup"><span data-stu-id="c5020-108">Methods</span></span>
|<span data-ttu-id="c5020-109">方法</span><span class="sxs-lookup"><span data-stu-id="c5020-109">Method</span></span>|<span data-ttu-id="c5020-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5020-110">Return Type</span></span>|<span data-ttu-id="c5020-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5020-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5020-112">列表 groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c5020-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="c5020-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5020-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c5020-114">列出属性和[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="c5020-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c5020-115">获取 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="c5020-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c5020-117">读取属性和[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c5020-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c5020-118">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="c5020-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c5020-120">创建新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5020-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c5020-121">删除 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="c5020-122">无</span><span class="sxs-lookup"><span data-stu-id="c5020-122">None</span></span>|<span data-ttu-id="c5020-123">删除[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c5020-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c5020-124">更新 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="c5020-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c5020-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c5020-126">更新[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5020-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5020-127">属性</span><span class="sxs-lookup"><span data-stu-id="c5020-127">Properties</span></span>
|<span data-ttu-id="c5020-128">属性</span><span class="sxs-lookup"><span data-stu-id="c5020-128">Property</span></span>|<span data-ttu-id="c5020-129">类型</span><span class="sxs-lookup"><span data-stu-id="c5020-129">Type</span></span>|<span data-ttu-id="c5020-130">说明</span><span class="sxs-lookup"><span data-stu-id="c5020-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5020-131">id</span><span class="sxs-lookup"><span data-stu-id="c5020-131">id</span></span>|<span data-ttu-id="c5020-132">String</span><span class="sxs-lookup"><span data-stu-id="c5020-132">String</span></span>|<span data-ttu-id="c5020-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5020-133">Key of the entity.</span></span>|
|<span data-ttu-id="c5020-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5020-134">lastModifiedDateTime</span></span>|<span data-ttu-id="c5020-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5020-135">DateTimeOffset</span></span>|<span data-ttu-id="c5020-136">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="c5020-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="c5020-137">target</span><span class="sxs-lookup"><span data-stu-id="c5020-137">target</span></span>|[<span data-ttu-id="c5020-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c5020-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c5020-139">组类型目标组策略配置。</span><span class="sxs-lookup"><span data-stu-id="c5020-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5020-140">关系</span><span class="sxs-lookup"><span data-stu-id="c5020-140">Relationships</span></span>
<span data-ttu-id="c5020-141">无</span><span class="sxs-lookup"><span data-stu-id="c5020-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5020-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5020-142">JSON Representation</span></span>
<span data-ttu-id="c5020-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5020-143">Here is a JSON representation of the resource.</span></span>
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




