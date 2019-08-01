---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4293b5e7efc29ccf25a2b4c72b6b8ceb1a377a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037182"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="41a56-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="41a56-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="41a56-107">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41a56-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41a56-108">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="41a56-108">The Role Assignment resource.</span></span> <span data-ttu-id="41a56-109">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="41a56-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="41a56-110">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="41a56-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="41a56-111">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="41a56-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="41a56-112">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41a56-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="41a56-113">方法</span><span class="sxs-lookup"><span data-stu-id="41a56-113">Methods</span></span>
|<span data-ttu-id="41a56-114">方法</span><span class="sxs-lookup"><span data-stu-id="41a56-114">Method</span></span>|<span data-ttu-id="41a56-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="41a56-115">Return Type</span></span>|<span data-ttu-id="41a56-116">说明</span><span class="sxs-lookup"><span data-stu-id="41a56-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="41a56-117">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="41a56-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="41a56-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41a56-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="41a56-119">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41a56-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="41a56-120">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="41a56-121">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-121">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="41a56-122">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41a56-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="41a56-123">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="41a56-124">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-124">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="41a56-125">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41a56-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="41a56-126">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="41a56-127">无</span><span class="sxs-lookup"><span data-stu-id="41a56-127">None</span></span>|<span data-ttu-id="41a56-128">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="41a56-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="41a56-129">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="41a56-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="41a56-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="41a56-131">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41a56-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="41a56-132">属性</span><span class="sxs-lookup"><span data-stu-id="41a56-132">Properties</span></span>
|<span data-ttu-id="41a56-133">属性</span><span class="sxs-lookup"><span data-stu-id="41a56-133">Property</span></span>|<span data-ttu-id="41a56-134">类型</span><span class="sxs-lookup"><span data-stu-id="41a56-134">Type</span></span>|<span data-ttu-id="41a56-135">说明</span><span class="sxs-lookup"><span data-stu-id="41a56-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41a56-136">id</span><span class="sxs-lookup"><span data-stu-id="41a56-136">id</span></span>|<span data-ttu-id="41a56-137">字符串</span><span class="sxs-lookup"><span data-stu-id="41a56-137">String</span></span>|<span data-ttu-id="41a56-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41a56-138">Key of the entity.</span></span> <span data-ttu-id="41a56-139">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="41a56-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="41a56-140">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41a56-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="41a56-141">displayName</span><span class="sxs-lookup"><span data-stu-id="41a56-141">displayName</span></span>|<span data-ttu-id="41a56-142">String</span><span class="sxs-lookup"><span data-stu-id="41a56-142">String</span></span>|<span data-ttu-id="41a56-143">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="41a56-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="41a56-144">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41a56-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="41a56-145">说明</span><span class="sxs-lookup"><span data-stu-id="41a56-145">description</span></span>|<span data-ttu-id="41a56-146">String</span><span class="sxs-lookup"><span data-stu-id="41a56-146">String</span></span>|<span data-ttu-id="41a56-147">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="41a56-147">Description of the Role Assignment.</span></span> <span data-ttu-id="41a56-148">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41a56-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="41a56-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="41a56-149">resourceScopes</span></span>|<span data-ttu-id="41a56-150">String collection</span><span class="sxs-lookup"><span data-stu-id="41a56-150">String collection</span></span>|<span data-ttu-id="41a56-151">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="41a56-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="41a56-152">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="41a56-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="41a56-153">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41a56-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="41a56-154">members</span><span class="sxs-lookup"><span data-stu-id="41a56-154">members</span></span>|<span data-ttu-id="41a56-155">String collection</span><span class="sxs-lookup"><span data-stu-id="41a56-155">String collection</span></span>|<span data-ttu-id="41a56-156">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="41a56-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="41a56-157">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="41a56-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41a56-158">关系</span><span class="sxs-lookup"><span data-stu-id="41a56-158">Relationships</span></span>
|<span data-ttu-id="41a56-159">关系</span><span class="sxs-lookup"><span data-stu-id="41a56-159">Relationship</span></span>|<span data-ttu-id="41a56-160">类型</span><span class="sxs-lookup"><span data-stu-id="41a56-160">Type</span></span>|<span data-ttu-id="41a56-161">说明</span><span class="sxs-lookup"><span data-stu-id="41a56-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41a56-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41a56-162">roleDefinition</span></span>|[<span data-ttu-id="41a56-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="41a56-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="41a56-164">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="41a56-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="41a56-165">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="41a56-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41a56-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41a56-166">JSON Representation</span></span>
<span data-ttu-id="41a56-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41a56-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



