---
title: roleScopeTagAutoAssignment 资源类型
description: 包含用于将角色作用域标记自动分配给要应用于设备的组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a308c91eb2a78c50012c348a19b613335915af47
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369183"
---
# <a name="rolescopetagautoassignment-resource-type"></a><span data-ttu-id="5e54d-103">roleScopeTagAutoAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e54d-103">roleScopeTagAutoAssignment resource type</span></span>

> <span data-ttu-id="5e54d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e54d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e54d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e54d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e54d-106">包含用于将角色作用域标记自动分配给要应用于设备的组的属性。</span><span class="sxs-lookup"><span data-stu-id="5e54d-106">Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.</span></span>

## <a name="methods"></a><span data-ttu-id="5e54d-107">方法</span><span class="sxs-lookup"><span data-stu-id="5e54d-107">Methods</span></span>
|<span data-ttu-id="5e54d-108">方法</span><span class="sxs-lookup"><span data-stu-id="5e54d-108">Method</span></span>|<span data-ttu-id="5e54d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e54d-109">Return Type</span></span>|<span data-ttu-id="5e54d-110">说明</span><span class="sxs-lookup"><span data-stu-id="5e54d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e54d-111">列出 roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="5e54d-111">List roleScopeTagAutoAssignments</span></span>](../api/intune-rbac-rolescopetagautoassignment-list.md)|<span data-ttu-id="5e54d-112">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5e54d-112">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="5e54d-113">列出[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e54d-113">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>|
|[<span data-ttu-id="5e54d-114">获取 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-114">Get roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-get.md)|[<span data-ttu-id="5e54d-115">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-115">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="5e54d-116">读取[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e54d-116">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="5e54d-117">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-117">Create roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-create.md)|[<span data-ttu-id="5e54d-118">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-118">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="5e54d-119">创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e54d-119">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="5e54d-120">删除 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-120">Delete roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-delete.md)|<span data-ttu-id="5e54d-121">无</span><span class="sxs-lookup"><span data-stu-id="5e54d-121">None</span></span>|<span data-ttu-id="5e54d-122">删除[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5e54d-122">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>|
|[<span data-ttu-id="5e54d-123">更新 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-123">Update roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-update.md)|[<span data-ttu-id="5e54d-124">roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="5e54d-124">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="5e54d-125">更新[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5e54d-125">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e54d-126">属性</span><span class="sxs-lookup"><span data-stu-id="5e54d-126">Properties</span></span>
|<span data-ttu-id="5e54d-127">属性</span><span class="sxs-lookup"><span data-stu-id="5e54d-127">Property</span></span>|<span data-ttu-id="5e54d-128">类型</span><span class="sxs-lookup"><span data-stu-id="5e54d-128">Type</span></span>|<span data-ttu-id="5e54d-129">说明</span><span class="sxs-lookup"><span data-stu-id="5e54d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e54d-130">id</span><span class="sxs-lookup"><span data-stu-id="5e54d-130">id</span></span>|<span data-ttu-id="5e54d-131">String</span><span class="sxs-lookup"><span data-stu-id="5e54d-131">String</span></span>|<span data-ttu-id="5e54d-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5e54d-132">Key of the entity.</span></span>|
|<span data-ttu-id="5e54d-133">target</span><span class="sxs-lookup"><span data-stu-id="5e54d-133">target</span></span>|[<span data-ttu-id="5e54d-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5e54d-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5e54d-135">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="5e54d-135">The auto-assignment target for the specific Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e54d-136">关系</span><span class="sxs-lookup"><span data-stu-id="5e54d-136">Relationships</span></span>
<span data-ttu-id="5e54d-137">无</span><span class="sxs-lookup"><span data-stu-id="5e54d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e54d-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e54d-138">JSON Representation</span></span>
<span data-ttu-id="5e54d-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e54d-139">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



