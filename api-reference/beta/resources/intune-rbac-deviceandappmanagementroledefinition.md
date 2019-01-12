---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: abe28e4b36c62df049e5f85b910e27f787bce2bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922891"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="31440-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="31440-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="31440-110">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="31440-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31440-111">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="31440-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31440-112">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="31440-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31440-113">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="31440-113">The Role Definition resource.</span></span> <span data-ttu-id="31440-114">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="31440-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="31440-115">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="31440-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="31440-116">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="31440-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="31440-117">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="31440-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="31440-118">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="31440-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="31440-119">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="31440-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="31440-120">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="31440-121">方法</span><span class="sxs-lookup"><span data-stu-id="31440-121">Methods</span></span>
|<span data-ttu-id="31440-122">方法</span><span class="sxs-lookup"><span data-stu-id="31440-122">Method</span></span>|<span data-ttu-id="31440-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="31440-123">Return Type</span></span>|<span data-ttu-id="31440-124">说明</span><span class="sxs-lookup"><span data-stu-id="31440-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31440-125">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="31440-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="31440-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31440-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="31440-127">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31440-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="31440-128">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="31440-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="31440-130">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31440-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="31440-131">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="31440-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="31440-133">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31440-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="31440-134">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="31440-135">无</span><span class="sxs-lookup"><span data-stu-id="31440-135">None</span></span>|<span data-ttu-id="31440-136">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="31440-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="31440-137">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="31440-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="31440-139">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="31440-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31440-140">属性</span><span class="sxs-lookup"><span data-stu-id="31440-140">Properties</span></span>
|<span data-ttu-id="31440-141">属性</span><span class="sxs-lookup"><span data-stu-id="31440-141">Property</span></span>|<span data-ttu-id="31440-142">类型</span><span class="sxs-lookup"><span data-stu-id="31440-142">Type</span></span>|<span data-ttu-id="31440-143">说明</span><span class="sxs-lookup"><span data-stu-id="31440-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31440-144">id</span><span class="sxs-lookup"><span data-stu-id="31440-144">id</span></span>|<span data-ttu-id="31440-145">String</span><span class="sxs-lookup"><span data-stu-id="31440-145">String</span></span>|<span data-ttu-id="31440-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="31440-146">Key of the entity.</span></span> <span data-ttu-id="31440-147">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="31440-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="31440-148">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="31440-149">displayName</span><span class="sxs-lookup"><span data-stu-id="31440-149">displayName</span></span>|<span data-ttu-id="31440-150">String</span><span class="sxs-lookup"><span data-stu-id="31440-150">String</span></span>|<span data-ttu-id="31440-151">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="31440-151">Display Name of the Role definition.</span></span> <span data-ttu-id="31440-152">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="31440-153">description</span><span class="sxs-lookup"><span data-stu-id="31440-153">description</span></span>|<span data-ttu-id="31440-154">String</span><span class="sxs-lookup"><span data-stu-id="31440-154">String</span></span>|<span data-ttu-id="31440-155">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="31440-155">Description of the Role definition.</span></span> <span data-ttu-id="31440-156">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="31440-157">permissions</span><span class="sxs-lookup"><span data-stu-id="31440-157">permissions</span></span>|<span data-ttu-id="31440-158">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31440-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="31440-159">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="31440-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="31440-160">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="31440-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="31440-161">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="31440-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="31440-162">rolePermissions</span></span>|<span data-ttu-id="31440-163">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31440-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="31440-164">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="31440-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="31440-165">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="31440-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="31440-166">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="31440-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="31440-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="31440-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="31440-168">Boolean</span></span>|<span data-ttu-id="31440-169">角色类型。</span><span class="sxs-lookup"><span data-stu-id="31440-169">Type of Role.</span></span> <span data-ttu-id="31440-170">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="31440-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="31440-171">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="31440-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="31440-172">isBuiltIn</span></span>|<span data-ttu-id="31440-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="31440-173">Boolean</span></span>|<span data-ttu-id="31440-174">角色类型。</span><span class="sxs-lookup"><span data-stu-id="31440-174">Type of Role.</span></span> <span data-ttu-id="31440-175">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="31440-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="31440-176">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="31440-177">关系</span><span class="sxs-lookup"><span data-stu-id="31440-177">Relationships</span></span>
|<span data-ttu-id="31440-178">关系</span><span class="sxs-lookup"><span data-stu-id="31440-178">Relationship</span></span>|<span data-ttu-id="31440-179">类型</span><span class="sxs-lookup"><span data-stu-id="31440-179">Type</span></span>|<span data-ttu-id="31440-180">说明</span><span class="sxs-lookup"><span data-stu-id="31440-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31440-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="31440-181">roleAssignments</span></span>|<span data-ttu-id="31440-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31440-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="31440-183">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="31440-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="31440-184">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31440-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31440-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31440-185">JSON Representation</span></span>
<span data-ttu-id="31440-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31440-186">Here is a JSON representation of the resource.</span></span>
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





