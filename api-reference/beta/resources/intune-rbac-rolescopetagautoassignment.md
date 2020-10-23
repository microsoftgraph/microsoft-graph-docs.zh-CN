---
title: roleScopeTagAutoAssignment 资源类型
description: 包含用于将角色作用域标记自动分配给要应用于设备的组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d33e6aca4b0c788995bae2aa169be347856104c3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723804"
---
# <a name="rolescopetagautoassignment-resource-type"></a><span data-ttu-id="d6966-103">roleScopeTagAutoAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6966-103">roleScopeTagAutoAssignment resource type</span></span>

<span data-ttu-id="d6966-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6966-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6966-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6966-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6966-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6966-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6966-107">包含用于将角色作用域标记自动分配给要应用于设备的组的属性。</span><span class="sxs-lookup"><span data-stu-id="d6966-107">Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.</span></span>

## <a name="methods"></a><span data-ttu-id="d6966-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d6966-108">Methods</span></span>
|<span data-ttu-id="d6966-109">方法</span><span class="sxs-lookup"><span data-stu-id="d6966-109">Method</span></span>|<span data-ttu-id="d6966-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6966-110">Return Type</span></span>|<span data-ttu-id="d6966-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6966-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6966-112">列出 roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="d6966-112">List roleScopeTagAutoAssignments</span></span>](../api/intune-rbac-rolescopetagautoassignment-list.md)|<span data-ttu-id="d6966-113">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6966-113">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="d6966-114">列出 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6966-114">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>|
|[<span data-ttu-id="d6966-115">获取 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-115">Get roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-get.md)|[<span data-ttu-id="d6966-116">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-116">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="d6966-117">读取 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6966-117">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="d6966-118">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-118">Create roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-create.md)|[<span data-ttu-id="d6966-119">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-119">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="d6966-120">创建新的 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6966-120">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="d6966-121">删除 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-121">Delete roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-delete.md)|<span data-ttu-id="d6966-122">无</span><span class="sxs-lookup"><span data-stu-id="d6966-122">None</span></span>|<span data-ttu-id="d6966-123">删除 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d6966-123">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>|
|[<span data-ttu-id="d6966-124">更新 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-124">Update roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-update.md)|[<span data-ttu-id="d6966-125">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6966-125">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="d6966-126">更新 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6966-126">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6966-127">属性</span><span class="sxs-lookup"><span data-stu-id="d6966-127">Properties</span></span>
|<span data-ttu-id="d6966-128">属性</span><span class="sxs-lookup"><span data-stu-id="d6966-128">Property</span></span>|<span data-ttu-id="d6966-129">类型</span><span class="sxs-lookup"><span data-stu-id="d6966-129">Type</span></span>|<span data-ttu-id="d6966-130">说明</span><span class="sxs-lookup"><span data-stu-id="d6966-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6966-131">id</span><span class="sxs-lookup"><span data-stu-id="d6966-131">id</span></span>|<span data-ttu-id="d6966-132">String</span><span class="sxs-lookup"><span data-stu-id="d6966-132">String</span></span>|<span data-ttu-id="d6966-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d6966-133">Key of the entity.</span></span>|
|<span data-ttu-id="d6966-134">target</span><span class="sxs-lookup"><span data-stu-id="d6966-134">target</span></span>|[<span data-ttu-id="d6966-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d6966-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d6966-136">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="d6966-136">The auto-assignment target for the specific Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6966-137">关系</span><span class="sxs-lookup"><span data-stu-id="d6966-137">Relationships</span></span>
<span data-ttu-id="d6966-138">无</span><span class="sxs-lookup"><span data-stu-id="d6966-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6966-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6966-139">JSON Representation</span></span>
<span data-ttu-id="d6966-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6966-140">Here is a JSON representation of the resource.</span></span>
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





