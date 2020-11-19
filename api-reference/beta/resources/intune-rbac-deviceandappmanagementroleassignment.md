---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3094c3ad5693193f56c25a5f9b24badb25e56ac9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272064"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="1d362-106">deviceAndAppManagementRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d362-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="1d362-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d362-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d362-108">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d362-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d362-109">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d362-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d362-110">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="1d362-110">The Role Assignment resource.</span></span> <span data-ttu-id="1d362-111">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="1d362-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="1d362-112">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="1d362-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="1d362-113">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="1d362-113">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="1d362-114">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-114">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1d362-115">方法</span><span class="sxs-lookup"><span data-stu-id="1d362-115">Methods</span></span>
|<span data-ttu-id="1d362-116">方法</span><span class="sxs-lookup"><span data-stu-id="1d362-116">Method</span></span>|<span data-ttu-id="1d362-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d362-117">Return Type</span></span>|<span data-ttu-id="1d362-118">说明</span><span class="sxs-lookup"><span data-stu-id="1d362-118">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d362-119">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="1d362-119">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="1d362-120">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d362-120">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="1d362-121">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d362-121">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="1d362-122">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-122">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="1d362-123">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-123">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="1d362-124">读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d362-124">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="1d362-125">创建 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-125">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="1d362-126">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-126">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="1d362-127">创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d362-127">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="1d362-128">删除 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-128">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="1d362-129">无</span><span class="sxs-lookup"><span data-stu-id="1d362-129">None</span></span>|<span data-ttu-id="1d362-130">删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1d362-130">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="1d362-131">更新 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-131">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="1d362-132">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1d362-132">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="1d362-133">更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1d362-133">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d362-134">属性</span><span class="sxs-lookup"><span data-stu-id="1d362-134">Properties</span></span>
|<span data-ttu-id="1d362-135">属性</span><span class="sxs-lookup"><span data-stu-id="1d362-135">Property</span></span>|<span data-ttu-id="1d362-136">类型</span><span class="sxs-lookup"><span data-stu-id="1d362-136">Type</span></span>|<span data-ttu-id="1d362-137">说明</span><span class="sxs-lookup"><span data-stu-id="1d362-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d362-138">id</span><span class="sxs-lookup"><span data-stu-id="1d362-138">id</span></span>|<span data-ttu-id="1d362-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1d362-139">String</span></span>|<span data-ttu-id="1d362-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1d362-140">Key of the entity.</span></span> <span data-ttu-id="1d362-141">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="1d362-141">This is read-only and automatically generated.</span></span> <span data-ttu-id="1d362-142">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-142">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1d362-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1d362-143">displayName</span></span>|<span data-ttu-id="1d362-144">字符串</span><span class="sxs-lookup"><span data-stu-id="1d362-144">String</span></span>|<span data-ttu-id="1d362-145">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="1d362-145">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="1d362-146">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-146">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1d362-147">description</span><span class="sxs-lookup"><span data-stu-id="1d362-147">description</span></span>|<span data-ttu-id="1d362-148">字符串</span><span class="sxs-lookup"><span data-stu-id="1d362-148">String</span></span>|<span data-ttu-id="1d362-149">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="1d362-149">Description of the Role Assignment.</span></span> <span data-ttu-id="1d362-150">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1d362-151">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="1d362-151">scopeMembers</span></span>|<span data-ttu-id="1d362-152">String collection</span><span class="sxs-lookup"><span data-stu-id="1d362-152">String collection</span></span>|<span data-ttu-id="1d362-153">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1d362-153">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1d362-154">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d362-154">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="1d362-155">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1d362-156">scopeType</span><span class="sxs-lookup"><span data-stu-id="1d362-156">scopeType</span></span>|[<span data-ttu-id="1d362-157">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="1d362-157">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="1d362-158">指定角色分配的作用域的类型。</span><span class="sxs-lookup"><span data-stu-id="1d362-158">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="1d362-159">默认类型 "ResourceScope" 允许分配 ResourceScopes。</span><span class="sxs-lookup"><span data-stu-id="1d362-159">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="1d362-160">对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers"，ResourceScopes 属性应保留为空。</span><span class="sxs-lookup"><span data-stu-id="1d362-160">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="1d362-161">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1d362-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="1d362-162">可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。</span><span class="sxs-lookup"><span data-stu-id="1d362-162">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="1d362-163">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1d362-163">resourceScopes</span></span>|<span data-ttu-id="1d362-164">String collection</span><span class="sxs-lookup"><span data-stu-id="1d362-164">String collection</span></span>|<span data-ttu-id="1d362-165">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1d362-165">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1d362-166">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d362-166">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="1d362-167">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-167">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1d362-168">members</span><span class="sxs-lookup"><span data-stu-id="1d362-168">members</span></span>|<span data-ttu-id="1d362-169">String collection</span><span class="sxs-lookup"><span data-stu-id="1d362-169">String collection</span></span>|<span data-ttu-id="1d362-170">角色成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="1d362-170">The list of ids of role member security groups.</span></span> <span data-ttu-id="1d362-171">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d362-171">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d362-172">关系</span><span class="sxs-lookup"><span data-stu-id="1d362-172">Relationships</span></span>
|<span data-ttu-id="1d362-173">关系</span><span class="sxs-lookup"><span data-stu-id="1d362-173">Relationship</span></span>|<span data-ttu-id="1d362-174">类型</span><span class="sxs-lookup"><span data-stu-id="1d362-174">Type</span></span>|<span data-ttu-id="1d362-175">说明</span><span class="sxs-lookup"><span data-stu-id="1d362-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d362-176">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1d362-176">roleDefinition</span></span>|[<span data-ttu-id="1d362-177">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1d362-177">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="1d362-178">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="1d362-178">Role definition this assignment is part of.</span></span> <span data-ttu-id="1d362-179">继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1d362-179">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1d362-180">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="1d362-180">roleScopeTags</span></span>|<span data-ttu-id="1d362-181">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d362-181">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="1d362-182">在角色分配上定义的一组角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="1d362-182">The set of Role Scope Tags defined on the Role Assignment.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d362-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d362-183">JSON Representation</span></span>
<span data-ttu-id="1d362-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d362-184">Here is a JSON representation of the resource.</span></span>
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




