---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b3a5204b766352436e1af3964b2f3f4baedc4efa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965185"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="7ab60-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ab60-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="7ab60-110">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ab60-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ab60-111">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="7ab60-111">The Role Definition resource.</span></span> <span data-ttu-id="7ab60-112">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="7ab60-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="7ab60-113">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="7ab60-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="7ab60-114">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="7ab60-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="7ab60-115">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="7ab60-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="7ab60-116">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="7ab60-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="7ab60-117">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="7ab60-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="7ab60-118">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7ab60-119">方法</span><span class="sxs-lookup"><span data-stu-id="7ab60-119">Methods</span></span>
|<span data-ttu-id="7ab60-120">方法</span><span class="sxs-lookup"><span data-stu-id="7ab60-120">Method</span></span>|<span data-ttu-id="7ab60-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ab60-121">Return Type</span></span>|<span data-ttu-id="7ab60-122">说明</span><span class="sxs-lookup"><span data-stu-id="7ab60-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ab60-123">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="7ab60-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="7ab60-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ab60-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="7ab60-125">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ab60-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="7ab60-126">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="7ab60-127">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-127">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7ab60-128">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ab60-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="7ab60-129">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="7ab60-130">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-130">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7ab60-131">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ab60-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="7ab60-132">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="7ab60-133">无</span><span class="sxs-lookup"><span data-stu-id="7ab60-133">None</span></span>|<span data-ttu-id="7ab60-134">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7ab60-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="7ab60-135">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="7ab60-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ab60-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="7ab60-137">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7ab60-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ab60-138">属性</span><span class="sxs-lookup"><span data-stu-id="7ab60-138">Properties</span></span>
|<span data-ttu-id="7ab60-139">属性</span><span class="sxs-lookup"><span data-stu-id="7ab60-139">Property</span></span>|<span data-ttu-id="7ab60-140">类型</span><span class="sxs-lookup"><span data-stu-id="7ab60-140">Type</span></span>|<span data-ttu-id="7ab60-141">说明</span><span class="sxs-lookup"><span data-stu-id="7ab60-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ab60-142">id</span><span class="sxs-lookup"><span data-stu-id="7ab60-142">id</span></span>|<span data-ttu-id="7ab60-143">String</span><span class="sxs-lookup"><span data-stu-id="7ab60-143">String</span></span>|<span data-ttu-id="7ab60-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ab60-144">Key of the entity.</span></span> <span data-ttu-id="7ab60-145">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="7ab60-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="7ab60-146">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ab60-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7ab60-147">displayName</span></span>|<span data-ttu-id="7ab60-148">String</span><span class="sxs-lookup"><span data-stu-id="7ab60-148">String</span></span>|<span data-ttu-id="7ab60-149">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7ab60-149">Display Name of the Role definition.</span></span> <span data-ttu-id="7ab60-150">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ab60-151">description</span><span class="sxs-lookup"><span data-stu-id="7ab60-151">description</span></span>|<span data-ttu-id="7ab60-152">String</span><span class="sxs-lookup"><span data-stu-id="7ab60-152">String</span></span>|<span data-ttu-id="7ab60-153">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="7ab60-153">Description of the Role definition.</span></span> <span data-ttu-id="7ab60-154">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ab60-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7ab60-155">rolePermissions</span></span>|<span data-ttu-id="7ab60-156">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ab60-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7ab60-157">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="7ab60-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7ab60-158">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="7ab60-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7ab60-159">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ab60-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7ab60-160">isBuiltIn</span></span>|<span data-ttu-id="7ab60-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ab60-161">Boolean</span></span>|<span data-ttu-id="7ab60-162">角色类型。</span><span class="sxs-lookup"><span data-stu-id="7ab60-162">Type of Role.</span></span> <span data-ttu-id="7ab60-163">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="7ab60-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7ab60-164">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ab60-165">关系</span><span class="sxs-lookup"><span data-stu-id="7ab60-165">Relationships</span></span>
|<span data-ttu-id="7ab60-166">关系</span><span class="sxs-lookup"><span data-stu-id="7ab60-166">Relationship</span></span>|<span data-ttu-id="7ab60-167">类型</span><span class="sxs-lookup"><span data-stu-id="7ab60-167">Type</span></span>|<span data-ttu-id="7ab60-168">说明</span><span class="sxs-lookup"><span data-stu-id="7ab60-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ab60-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="7ab60-169">roleAssignments</span></span>|<span data-ttu-id="7ab60-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ab60-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="7ab60-171">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="7ab60-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="7ab60-172">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7ab60-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ab60-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ab60-173">JSON Representation</span></span>
<span data-ttu-id="7ab60-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ab60-174">Here is a JSON representation of the resource.</span></span>
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```



