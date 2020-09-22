---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 869538f50d30460faa2cb8f43d7fd5f16666144c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095231"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="ff8a3-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff8a3-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="ff8a3-110">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff8a3-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff8a3-111">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff8a3-112">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff8a3-113">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-113">The Role Definition resource.</span></span> <span data-ttu-id="ff8a3-114">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="ff8a3-115">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="ff8a3-116">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="ff8a3-117">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="ff8a3-118">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="ff8a3-119">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="ff8a3-120">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ff8a3-121">方法</span><span class="sxs-lookup"><span data-stu-id="ff8a3-121">Methods</span></span>
|<span data-ttu-id="ff8a3-122">方法</span><span class="sxs-lookup"><span data-stu-id="ff8a3-122">Method</span></span>|<span data-ttu-id="ff8a3-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff8a3-123">Return Type</span></span>|<span data-ttu-id="ff8a3-124">说明</span><span class="sxs-lookup"><span data-stu-id="ff8a3-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff8a3-125">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ff8a3-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="ff8a3-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff8a3-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="ff8a3-127">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="ff8a3-128">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="ff8a3-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="ff8a3-130">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="ff8a3-131">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="ff8a3-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="ff8a3-133">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="ff8a3-134">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="ff8a3-135">无</span><span class="sxs-lookup"><span data-stu-id="ff8a3-135">None</span></span>|<span data-ttu-id="ff8a3-136">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="ff8a3-137">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="ff8a3-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="ff8a3-139">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff8a3-140">属性</span><span class="sxs-lookup"><span data-stu-id="ff8a3-140">Properties</span></span>
|<span data-ttu-id="ff8a3-141">属性</span><span class="sxs-lookup"><span data-stu-id="ff8a3-141">Property</span></span>|<span data-ttu-id="ff8a3-142">类型</span><span class="sxs-lookup"><span data-stu-id="ff8a3-142">Type</span></span>|<span data-ttu-id="ff8a3-143">说明</span><span class="sxs-lookup"><span data-stu-id="ff8a3-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff8a3-144">id</span><span class="sxs-lookup"><span data-stu-id="ff8a3-144">id</span></span>|<span data-ttu-id="ff8a3-145">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8a3-145">String</span></span>|<span data-ttu-id="ff8a3-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-146">Key of the entity.</span></span> <span data-ttu-id="ff8a3-147">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="ff8a3-148">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="ff8a3-149">displayName</span></span>|<span data-ttu-id="ff8a3-150">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8a3-150">String</span></span>|<span data-ttu-id="ff8a3-151">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-151">Display Name of the Role definition.</span></span> <span data-ttu-id="ff8a3-152">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-153">说明</span><span class="sxs-lookup"><span data-stu-id="ff8a3-153">description</span></span>|<span data-ttu-id="ff8a3-154">字符串</span><span class="sxs-lookup"><span data-stu-id="ff8a3-154">String</span></span>|<span data-ttu-id="ff8a3-155">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-155">Description of the Role definition.</span></span> <span data-ttu-id="ff8a3-156">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-157">permissions</span><span class="sxs-lookup"><span data-stu-id="ff8a3-157">permissions</span></span>|<span data-ttu-id="ff8a3-158">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff8a3-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ff8a3-159">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ff8a3-160">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ff8a3-161">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ff8a3-162">rolePermissions</span></span>|<span data-ttu-id="ff8a3-163">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff8a3-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ff8a3-164">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ff8a3-165">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ff8a3-166">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff8a3-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="ff8a3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff8a3-168">Boolean</span></span>|<span data-ttu-id="ff8a3-169">角色类型。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-169">Type of Role.</span></span> <span data-ttu-id="ff8a3-170">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ff8a3-171">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ff8a3-172">isBuiltIn</span></span>|<span data-ttu-id="ff8a3-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff8a3-173">Boolean</span></span>|<span data-ttu-id="ff8a3-174">角色类型。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-174">Type of Role.</span></span> <span data-ttu-id="ff8a3-175">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ff8a3-176">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ff8a3-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff8a3-177">roleScopeTagIds</span></span>|<span data-ttu-id="ff8a3-178">字符串集合</span><span class="sxs-lookup"><span data-stu-id="ff8a3-178">String collection</span></span>|<span data-ttu-id="ff8a3-179">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ff8a3-180">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-180">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff8a3-181">关系</span><span class="sxs-lookup"><span data-stu-id="ff8a3-181">Relationships</span></span>
|<span data-ttu-id="ff8a3-182">关系</span><span class="sxs-lookup"><span data-stu-id="ff8a3-182">Relationship</span></span>|<span data-ttu-id="ff8a3-183">类型</span><span class="sxs-lookup"><span data-stu-id="ff8a3-183">Type</span></span>|<span data-ttu-id="ff8a3-184">说明</span><span class="sxs-lookup"><span data-stu-id="ff8a3-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff8a3-185">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="ff8a3-185">roleAssignments</span></span>|<span data-ttu-id="ff8a3-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff8a3-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="ff8a3-187">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-187">List of Role assignments for this role definition.</span></span> <span data-ttu-id="ff8a3-188">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ff8a3-188">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff8a3-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff8a3-189">JSON Representation</span></span>
<span data-ttu-id="ff8a3-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff8a3-190">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```






