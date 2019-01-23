---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 854bf15869415c036a6daed574000b2513aca904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399967"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="388cb-109">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="388cb-109">roleDefinition resource type</span></span>

> <span data-ttu-id="388cb-110">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="388cb-110">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="388cb-111">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="388cb-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="388cb-112">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="388cb-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="388cb-113">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="388cb-113">The Role Definition resource.</span></span> <span data-ttu-id="388cb-114">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="388cb-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="388cb-115">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="388cb-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="388cb-116">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="388cb-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="388cb-117">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="388cb-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="388cb-118">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="388cb-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="388cb-119">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="388cb-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="388cb-120">方法</span><span class="sxs-lookup"><span data-stu-id="388cb-120">Methods</span></span>
|<span data-ttu-id="388cb-121">方法</span><span class="sxs-lookup"><span data-stu-id="388cb-121">Method</span></span>|<span data-ttu-id="388cb-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="388cb-122">Return Type</span></span>|<span data-ttu-id="388cb-123">说明</span><span class="sxs-lookup"><span data-stu-id="388cb-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="388cb-124">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="388cb-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="388cb-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cb-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="388cb-126">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="388cb-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="388cb-127">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="388cb-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="388cb-129">读取 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="388cb-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="388cb-130">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="388cb-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="388cb-132">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="388cb-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="388cb-133">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="388cb-134">无</span><span class="sxs-lookup"><span data-stu-id="388cb-134">None</span></span>|<span data-ttu-id="388cb-135">删除 [roleDefinition](../resources/intune-rbac-roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="388cb-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="388cb-136">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="388cb-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="388cb-138">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="388cb-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="388cb-139">属性</span><span class="sxs-lookup"><span data-stu-id="388cb-139">Properties</span></span>
|<span data-ttu-id="388cb-140">属性</span><span class="sxs-lookup"><span data-stu-id="388cb-140">Property</span></span>|<span data-ttu-id="388cb-141">类型</span><span class="sxs-lookup"><span data-stu-id="388cb-141">Type</span></span>|<span data-ttu-id="388cb-142">说明</span><span class="sxs-lookup"><span data-stu-id="388cb-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="388cb-143">id</span><span class="sxs-lookup"><span data-stu-id="388cb-143">id</span></span>|<span data-ttu-id="388cb-144">String</span><span class="sxs-lookup"><span data-stu-id="388cb-144">String</span></span>|<span data-ttu-id="388cb-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="388cb-145">Key of the entity.</span></span> <span data-ttu-id="388cb-146">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="388cb-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="388cb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="388cb-147">displayName</span></span>|<span data-ttu-id="388cb-148">String</span><span class="sxs-lookup"><span data-stu-id="388cb-148">String</span></span>|<span data-ttu-id="388cb-149">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="388cb-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="388cb-150">说明</span><span class="sxs-lookup"><span data-stu-id="388cb-150">description</span></span>|<span data-ttu-id="388cb-151">String</span><span class="sxs-lookup"><span data-stu-id="388cb-151">String</span></span>|<span data-ttu-id="388cb-152">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="388cb-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="388cb-153">permissions</span><span class="sxs-lookup"><span data-stu-id="388cb-153">permissions</span></span>|<span data-ttu-id="388cb-154">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cb-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="388cb-155">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="388cb-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="388cb-156">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="388cb-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="388cb-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="388cb-157">rolePermissions</span></span>|<span data-ttu-id="388cb-158">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cb-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="388cb-159">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="388cb-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="388cb-160">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="388cb-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="388cb-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="388cb-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="388cb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="388cb-162">Boolean</span></span>|<span data-ttu-id="388cb-163">角色类型。</span><span class="sxs-lookup"><span data-stu-id="388cb-163">Type of Role.</span></span> <span data-ttu-id="388cb-164">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="388cb-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="388cb-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="388cb-165">isBuiltIn</span></span>|<span data-ttu-id="388cb-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="388cb-166">Boolean</span></span>|<span data-ttu-id="388cb-167">角色类型。</span><span class="sxs-lookup"><span data-stu-id="388cb-167">Type of Role.</span></span> <span data-ttu-id="388cb-168">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="388cb-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="388cb-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="388cb-169">roleScopeTagIds</span></span>|<span data-ttu-id="388cb-170">String 集合</span><span class="sxs-lookup"><span data-stu-id="388cb-170">String collection</span></span>|<span data-ttu-id="388cb-171">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="388cb-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="388cb-172">关系</span><span class="sxs-lookup"><span data-stu-id="388cb-172">Relationships</span></span>
|<span data-ttu-id="388cb-173">关系</span><span class="sxs-lookup"><span data-stu-id="388cb-173">Relationship</span></span>|<span data-ttu-id="388cb-174">类型</span><span class="sxs-lookup"><span data-stu-id="388cb-174">Type</span></span>|<span data-ttu-id="388cb-175">说明</span><span class="sxs-lookup"><span data-stu-id="388cb-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="388cb-176">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="388cb-176">roleAssignments</span></span>|<span data-ttu-id="388cb-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cb-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="388cb-178">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="388cb-178">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="388cb-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="388cb-179">JSON Representation</span></span>
<span data-ttu-id="388cb-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="388cb-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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




