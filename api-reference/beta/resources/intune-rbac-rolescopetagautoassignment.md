---
title: roleScopeTagAutoAssignment 资源类型
description: 包含用于将角色作用域标记自动分配给要应用于设备的组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffde4aeb5b1389255c694bbbbfef969f91c3e026
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307134"
---
# <a name="rolescopetagautoassignment-resource-type"></a><span data-ttu-id="c421b-103">roleScopeTagAutoAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c421b-103">roleScopeTagAutoAssignment resource type</span></span>

<span data-ttu-id="c421b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c421b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c421b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c421b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c421b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c421b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c421b-107">包含用于将角色作用域标记自动分配给要应用于设备的组的属性。</span><span class="sxs-lookup"><span data-stu-id="c421b-107">Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.</span></span>

## <a name="methods"></a><span data-ttu-id="c421b-108">Methods</span><span class="sxs-lookup"><span data-stu-id="c421b-108">Methods</span></span>
|<span data-ttu-id="c421b-109">方法</span><span class="sxs-lookup"><span data-stu-id="c421b-109">Method</span></span>|<span data-ttu-id="c421b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c421b-110">Return Type</span></span>|<span data-ttu-id="c421b-111">Description</span><span class="sxs-lookup"><span data-stu-id="c421b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c421b-112">列出 roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="c421b-112">List roleScopeTagAutoAssignments</span></span>](../api/intune-rbac-rolescopetagautoassignment-list.md)|<span data-ttu-id="c421b-113">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c421b-113">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="c421b-114">列出 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c421b-114">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>|
|[<span data-ttu-id="c421b-115">获取 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-115">Get roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-get.md)|[<span data-ttu-id="c421b-116">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-116">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="c421b-117">读取 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c421b-117">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="c421b-118">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-118">Create roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-create.md)|[<span data-ttu-id="c421b-119">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-119">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="c421b-120">创建新的 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c421b-120">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="c421b-121">删除 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-121">Delete roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-delete.md)|<span data-ttu-id="c421b-122">无</span><span class="sxs-lookup"><span data-stu-id="c421b-122">None</span></span>|<span data-ttu-id="c421b-123">删除 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c421b-123">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>|
|[<span data-ttu-id="c421b-124">更新 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-124">Update roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-update.md)|[<span data-ttu-id="c421b-125">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="c421b-125">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="c421b-126">更新 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c421b-126">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c421b-127">属性</span><span class="sxs-lookup"><span data-stu-id="c421b-127">Properties</span></span>
|<span data-ttu-id="c421b-128">属性</span><span class="sxs-lookup"><span data-stu-id="c421b-128">Property</span></span>|<span data-ttu-id="c421b-129">类型</span><span class="sxs-lookup"><span data-stu-id="c421b-129">Type</span></span>|<span data-ttu-id="c421b-130">说明</span><span class="sxs-lookup"><span data-stu-id="c421b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c421b-131">id</span><span class="sxs-lookup"><span data-stu-id="c421b-131">id</span></span>|<span data-ttu-id="c421b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c421b-132">String</span></span>|<span data-ttu-id="c421b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c421b-133">Key of the entity.</span></span>|
|<span data-ttu-id="c421b-134">target</span><span class="sxs-lookup"><span data-stu-id="c421b-134">target</span></span>|[<span data-ttu-id="c421b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c421b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c421b-136">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="c421b-136">The auto-assignment target for the specific Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c421b-137">关系</span><span class="sxs-lookup"><span data-stu-id="c421b-137">Relationships</span></span>
<span data-ttu-id="c421b-138">无</span><span class="sxs-lookup"><span data-stu-id="c421b-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c421b-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c421b-139">JSON Representation</span></span>
<span data-ttu-id="c421b-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c421b-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




