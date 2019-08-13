---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5ec33dc83ab0e6389fb45b09b2873b9290aa55ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337564"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="9fde8-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fde8-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="9fde8-110">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fde8-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fde8-111">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fde8-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fde8-112">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="9fde8-112">The Role Definition resource.</span></span> <span data-ttu-id="9fde8-113">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="9fde8-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="9fde8-114">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="9fde8-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="9fde8-115">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="9fde8-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="9fde8-116">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="9fde8-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="9fde8-117">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="9fde8-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="9fde8-118">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="9fde8-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="9fde8-119">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9fde8-120">方法</span><span class="sxs-lookup"><span data-stu-id="9fde8-120">Methods</span></span>
|<span data-ttu-id="9fde8-121">方法</span><span class="sxs-lookup"><span data-stu-id="9fde8-121">Method</span></span>|<span data-ttu-id="9fde8-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="9fde8-122">Return Type</span></span>|<span data-ttu-id="9fde8-123">说明</span><span class="sxs-lookup"><span data-stu-id="9fde8-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9fde8-124">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="9fde8-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="9fde8-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fde8-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="9fde8-126">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fde8-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="9fde8-127">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="9fde8-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="9fde8-129">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fde8-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="9fde8-130">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="9fde8-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="9fde8-132">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fde8-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="9fde8-133">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="9fde8-134">无</span><span class="sxs-lookup"><span data-stu-id="9fde8-134">None</span></span>|<span data-ttu-id="9fde8-135">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9fde8-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="9fde8-136">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="9fde8-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="9fde8-138">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9fde8-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fde8-139">属性</span><span class="sxs-lookup"><span data-stu-id="9fde8-139">Properties</span></span>
|<span data-ttu-id="9fde8-140">属性</span><span class="sxs-lookup"><span data-stu-id="9fde8-140">Property</span></span>|<span data-ttu-id="9fde8-141">类型</span><span class="sxs-lookup"><span data-stu-id="9fde8-141">Type</span></span>|<span data-ttu-id="9fde8-142">说明</span><span class="sxs-lookup"><span data-stu-id="9fde8-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fde8-143">id</span><span class="sxs-lookup"><span data-stu-id="9fde8-143">id</span></span>|<span data-ttu-id="9fde8-144">字符串</span><span class="sxs-lookup"><span data-stu-id="9fde8-144">String</span></span>|<span data-ttu-id="9fde8-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9fde8-145">Key of the entity.</span></span> <span data-ttu-id="9fde8-146">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="9fde8-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="9fde8-147">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-148">displayName</span><span class="sxs-lookup"><span data-stu-id="9fde8-148">displayName</span></span>|<span data-ttu-id="9fde8-149">String</span><span class="sxs-lookup"><span data-stu-id="9fde8-149">String</span></span>|<span data-ttu-id="9fde8-150">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9fde8-150">Display Name of the Role definition.</span></span> <span data-ttu-id="9fde8-151">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-152">说明</span><span class="sxs-lookup"><span data-stu-id="9fde8-152">description</span></span>|<span data-ttu-id="9fde8-153">String</span><span class="sxs-lookup"><span data-stu-id="9fde8-153">String</span></span>|<span data-ttu-id="9fde8-154">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="9fde8-154">Description of the Role definition.</span></span> <span data-ttu-id="9fde8-155">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-156">permissions</span><span class="sxs-lookup"><span data-stu-id="9fde8-156">permissions</span></span>|<span data-ttu-id="9fde8-157">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fde8-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="9fde8-158">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="9fde8-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="9fde8-159">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="9fde8-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="9fde8-160">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-161">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="9fde8-161">rolePermissions</span></span>|<span data-ttu-id="9fde8-162">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fde8-162">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="9fde8-163">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="9fde8-163">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="9fde8-164">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="9fde8-164">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="9fde8-165">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-166">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9fde8-166">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="9fde8-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fde8-167">Boolean</span></span>|<span data-ttu-id="9fde8-168">角色类型。</span><span class="sxs-lookup"><span data-stu-id="9fde8-168">Type of Role.</span></span> <span data-ttu-id="9fde8-169">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="9fde8-169">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="9fde8-170">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-170">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="9fde8-171">isBuiltIn</span></span>|<span data-ttu-id="9fde8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fde8-172">Boolean</span></span>|<span data-ttu-id="9fde8-173">角色类型。</span><span class="sxs-lookup"><span data-stu-id="9fde8-173">Type of Role.</span></span> <span data-ttu-id="9fde8-174">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="9fde8-174">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="9fde8-175">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-175">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="9fde8-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9fde8-176">roleScopeTagIds</span></span>|<span data-ttu-id="9fde8-177">String collection</span><span class="sxs-lookup"><span data-stu-id="9fde8-177">String collection</span></span>|<span data-ttu-id="9fde8-178">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9fde8-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9fde8-179">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-179">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fde8-180">关系</span><span class="sxs-lookup"><span data-stu-id="9fde8-180">Relationships</span></span>
|<span data-ttu-id="9fde8-181">关系</span><span class="sxs-lookup"><span data-stu-id="9fde8-181">Relationship</span></span>|<span data-ttu-id="9fde8-182">类型</span><span class="sxs-lookup"><span data-stu-id="9fde8-182">Type</span></span>|<span data-ttu-id="9fde8-183">说明</span><span class="sxs-lookup"><span data-stu-id="9fde8-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fde8-184">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="9fde8-184">roleAssignments</span></span>|<span data-ttu-id="9fde8-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9fde8-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="9fde8-186">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="9fde8-186">List of Role assignments for this role definition.</span></span> <span data-ttu-id="9fde8-187">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9fde8-187">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fde8-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fde8-188">JSON Representation</span></span>
<span data-ttu-id="9fde8-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fde8-189">Here is a JSON representation of the resource.</span></span>
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



