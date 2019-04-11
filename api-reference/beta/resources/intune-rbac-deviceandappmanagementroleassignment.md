---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2cb748669a7475319f97bf72b341d247ed6e5c86
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801419"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="bb2e4-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb2e4-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="bb2e4-107">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb2e4-108">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb2e4-109">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-109">The Role Assignment resource.</span></span> <span data-ttu-id="bb2e4-110">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="bb2e4-111">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="bb2e4-112">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="bb2e4-113">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bb2e4-114">方法</span><span class="sxs-lookup"><span data-stu-id="bb2e4-114">Methods</span></span>
|<span data-ttu-id="bb2e4-115">方法</span><span class="sxs-lookup"><span data-stu-id="bb2e4-115">Method</span></span>|<span data-ttu-id="bb2e4-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb2e4-116">Return Type</span></span>|<span data-ttu-id="bb2e4-117">说明</span><span class="sxs-lookup"><span data-stu-id="bb2e4-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb2e4-118">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="bb2e4-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="bb2e4-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb2e4-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="bb2e4-120">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="bb2e4-121">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="bb2e4-122">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-122">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="bb2e4-123">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="bb2e4-124">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="bb2e4-125">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-125">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="bb2e4-126">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="bb2e4-127">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="bb2e4-128">无</span><span class="sxs-lookup"><span data-stu-id="bb2e4-128">None</span></span>|<span data-ttu-id="bb2e4-129">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="bb2e4-130">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="bb2e4-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb2e4-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="bb2e4-132">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb2e4-133">属性</span><span class="sxs-lookup"><span data-stu-id="bb2e4-133">Properties</span></span>
|<span data-ttu-id="bb2e4-134">属性</span><span class="sxs-lookup"><span data-stu-id="bb2e4-134">Property</span></span>|<span data-ttu-id="bb2e4-135">类型</span><span class="sxs-lookup"><span data-stu-id="bb2e4-135">Type</span></span>|<span data-ttu-id="bb2e4-136">说明</span><span class="sxs-lookup"><span data-stu-id="bb2e4-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb2e4-137">id</span><span class="sxs-lookup"><span data-stu-id="bb2e4-137">id</span></span>|<span data-ttu-id="bb2e4-138">String</span><span class="sxs-lookup"><span data-stu-id="bb2e4-138">String</span></span>|<span data-ttu-id="bb2e4-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-139">Key of the entity.</span></span> <span data-ttu-id="bb2e4-140">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="bb2e4-141">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bb2e4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="bb2e4-142">displayName</span></span>|<span data-ttu-id="bb2e4-143">String</span><span class="sxs-lookup"><span data-stu-id="bb2e4-143">String</span></span>|<span data-ttu-id="bb2e4-144">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="bb2e4-145">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bb2e4-146">description</span><span class="sxs-lookup"><span data-stu-id="bb2e4-146">description</span></span>|<span data-ttu-id="bb2e4-147">String</span><span class="sxs-lookup"><span data-stu-id="bb2e4-147">String</span></span>|<span data-ttu-id="bb2e4-148">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-148">Description of the Role Assignment.</span></span> <span data-ttu-id="bb2e4-149">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bb2e4-150">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="bb2e4-150">scopeMembers</span></span>|<span data-ttu-id="bb2e4-151">String 集合</span><span class="sxs-lookup"><span data-stu-id="bb2e4-151">String collection</span></span>|<span data-ttu-id="bb2e4-152">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="bb2e4-153">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="bb2e4-154">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bb2e4-155">scopeType</span><span class="sxs-lookup"><span data-stu-id="bb2e4-155">scopeType</span></span>|[<span data-ttu-id="bb2e4-156">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="bb2e4-156">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="bb2e4-157">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-157">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="bb2e4-158">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-158">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="bb2e4-159">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-159">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="bb2e4-160">继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-160">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="bb2e4-161">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-161">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="bb2e4-162">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="bb2e4-162">resourceScopes</span></span>|<span data-ttu-id="bb2e4-163">String 集合</span><span class="sxs-lookup"><span data-stu-id="bb2e4-163">String collection</span></span>|<span data-ttu-id="bb2e4-164">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-164">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="bb2e4-165">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-165">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="bb2e4-166">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bb2e4-167">members</span><span class="sxs-lookup"><span data-stu-id="bb2e4-167">members</span></span>|<span data-ttu-id="bb2e4-168">String collection</span><span class="sxs-lookup"><span data-stu-id="bb2e4-168">String collection</span></span>|<span data-ttu-id="bb2e4-169">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-169">The list of ids of role member security groups.</span></span> <span data-ttu-id="bb2e4-170">这些是来自 Azure Active Directory 的 ID。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-170">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb2e4-171">关系</span><span class="sxs-lookup"><span data-stu-id="bb2e4-171">Relationships</span></span>
|<span data-ttu-id="bb2e4-172">关系</span><span class="sxs-lookup"><span data-stu-id="bb2e4-172">Relationship</span></span>|<span data-ttu-id="bb2e4-173">类型</span><span class="sxs-lookup"><span data-stu-id="bb2e4-173">Type</span></span>|<span data-ttu-id="bb2e4-174">说明</span><span class="sxs-lookup"><span data-stu-id="bb2e4-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb2e4-175">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb2e4-175">roleDefinition</span></span>|[<span data-ttu-id="bb2e4-176">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb2e4-176">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="bb2e4-177">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-177">Role definition this assignment is part of.</span></span> <span data-ttu-id="bb2e4-178">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb2e4-178">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bb2e4-179">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb2e4-179">roleScopeTags</span></span>|<span data-ttu-id="bb2e4-180">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb2e4-180">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="bb2e4-181">在角色分配上定义的一组角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-181">The set of Role Scope Tags defined on the Role Assignment.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb2e4-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb2e4-182">JSON Representation</span></span>
<span data-ttu-id="bb2e4-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb2e4-183">Here is a JSON representation of the resource.</span></span>
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
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```





