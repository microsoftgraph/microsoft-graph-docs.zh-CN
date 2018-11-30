---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
ms.openlocfilehash: 90c701afc33a16cfb2747c40d53d47e74c3cedde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044744"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="7f678-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f678-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="7f678-110">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7f678-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f678-111">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7f678-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f678-112">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7f678-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f678-113">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="7f678-113">The Role Definition resource.</span></span> <span data-ttu-id="7f678-114">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="7f678-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="7f678-115">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="7f678-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="7f678-116">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="7f678-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="7f678-117">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="7f678-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="7f678-118">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="7f678-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="7f678-119">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="7f678-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="7f678-120">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7f678-121">方法</span><span class="sxs-lookup"><span data-stu-id="7f678-121">Methods</span></span>
|<span data-ttu-id="7f678-122">方法</span><span class="sxs-lookup"><span data-stu-id="7f678-122">Method</span></span>|<span data-ttu-id="7f678-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="7f678-123">Return Type</span></span>|<span data-ttu-id="7f678-124">说明</span><span class="sxs-lookup"><span data-stu-id="7f678-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f678-125">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="7f678-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="7f678-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f678-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="7f678-127">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f678-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="7f678-128">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="7f678-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7f678-130">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f678-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="7f678-131">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="7f678-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7f678-133">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f678-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="7f678-134">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="7f678-135">无</span><span class="sxs-lookup"><span data-stu-id="7f678-135">None</span></span>|<span data-ttu-id="7f678-136">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7f678-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="7f678-137">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="7f678-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7f678-139">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7f678-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f678-140">属性</span><span class="sxs-lookup"><span data-stu-id="7f678-140">Properties</span></span>
|<span data-ttu-id="7f678-141">属性</span><span class="sxs-lookup"><span data-stu-id="7f678-141">Property</span></span>|<span data-ttu-id="7f678-142">类型</span><span class="sxs-lookup"><span data-stu-id="7f678-142">Type</span></span>|<span data-ttu-id="7f678-143">说明</span><span class="sxs-lookup"><span data-stu-id="7f678-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f678-144">id</span><span class="sxs-lookup"><span data-stu-id="7f678-144">id</span></span>|<span data-ttu-id="7f678-145">String</span><span class="sxs-lookup"><span data-stu-id="7f678-145">String</span></span>|<span data-ttu-id="7f678-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7f678-146">Key of the entity.</span></span> <span data-ttu-id="7f678-147">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="7f678-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="7f678-148">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7f678-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7f678-149">displayName</span></span>|<span data-ttu-id="7f678-150">String</span><span class="sxs-lookup"><span data-stu-id="7f678-150">String</span></span>|<span data-ttu-id="7f678-151">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7f678-151">Display Name of the Role definition.</span></span> <span data-ttu-id="7f678-152">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7f678-153">description</span><span class="sxs-lookup"><span data-stu-id="7f678-153">description</span></span>|<span data-ttu-id="7f678-154">String</span><span class="sxs-lookup"><span data-stu-id="7f678-154">String</span></span>|<span data-ttu-id="7f678-155">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="7f678-155">Description of the Role definition.</span></span> <span data-ttu-id="7f678-156">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7f678-157">permissions</span><span class="sxs-lookup"><span data-stu-id="7f678-157">permissions</span></span>|<span data-ttu-id="7f678-158">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f678-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7f678-159">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="7f678-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7f678-160">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="7f678-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7f678-161">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7f678-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7f678-162">rolePermissions</span></span>|<span data-ttu-id="7f678-163">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f678-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7f678-164">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="7f678-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7f678-165">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="7f678-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7f678-166">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7f678-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7f678-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="7f678-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="7f678-168">Boolean</span></span>|<span data-ttu-id="7f678-169">角色类型。</span><span class="sxs-lookup"><span data-stu-id="7f678-169">Type of Role.</span></span> <span data-ttu-id="7f678-170">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="7f678-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7f678-171">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7f678-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7f678-172">isBuiltIn</span></span>|<span data-ttu-id="7f678-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="7f678-173">Boolean</span></span>|<span data-ttu-id="7f678-174">角色类型。</span><span class="sxs-lookup"><span data-stu-id="7f678-174">Type of Role.</span></span> <span data-ttu-id="7f678-175">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="7f678-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7f678-176">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f678-177">关系</span><span class="sxs-lookup"><span data-stu-id="7f678-177">Relationships</span></span>
|<span data-ttu-id="7f678-178">关系</span><span class="sxs-lookup"><span data-stu-id="7f678-178">Relationship</span></span>|<span data-ttu-id="7f678-179">类型</span><span class="sxs-lookup"><span data-stu-id="7f678-179">Type</span></span>|<span data-ttu-id="7f678-180">说明</span><span class="sxs-lookup"><span data-stu-id="7f678-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f678-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="7f678-181">roleAssignments</span></span>|<span data-ttu-id="7f678-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f678-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="7f678-183">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="7f678-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="7f678-184">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7f678-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f678-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f678-185">JSON Representation</span></span>
<span data-ttu-id="7f678-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f678-186">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





