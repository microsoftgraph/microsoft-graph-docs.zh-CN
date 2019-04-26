---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e703909f818535eac7ae00284d15620bce55ba80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567464"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="d5431-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5431-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="d5431-110">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5431-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5431-111">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="d5431-111">The Role Definition resource.</span></span> <span data-ttu-id="d5431-112">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="d5431-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="d5431-113">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="d5431-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="d5431-114">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="d5431-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="d5431-115">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="d5431-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="d5431-116">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="d5431-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="d5431-117">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="d5431-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="d5431-118">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d5431-119">方法</span><span class="sxs-lookup"><span data-stu-id="d5431-119">Methods</span></span>
|<span data-ttu-id="d5431-120">方法</span><span class="sxs-lookup"><span data-stu-id="d5431-120">Method</span></span>|<span data-ttu-id="d5431-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5431-121">Return Type</span></span>|<span data-ttu-id="d5431-122">说明</span><span class="sxs-lookup"><span data-stu-id="d5431-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5431-123">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="d5431-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="d5431-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5431-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="d5431-125">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5431-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="d5431-126">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="d5431-127">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-127">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="d5431-128">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5431-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="d5431-129">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="d5431-130">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-130">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="d5431-131">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5431-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="d5431-132">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="d5431-133">无</span><span class="sxs-lookup"><span data-stu-id="d5431-133">None</span></span>|<span data-ttu-id="d5431-134">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="d5431-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="d5431-135">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="d5431-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d5431-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="d5431-137">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d5431-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5431-138">属性</span><span class="sxs-lookup"><span data-stu-id="d5431-138">Properties</span></span>
|<span data-ttu-id="d5431-139">属性</span><span class="sxs-lookup"><span data-stu-id="d5431-139">Property</span></span>|<span data-ttu-id="d5431-140">类型</span><span class="sxs-lookup"><span data-stu-id="d5431-140">Type</span></span>|<span data-ttu-id="d5431-141">说明</span><span class="sxs-lookup"><span data-stu-id="d5431-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5431-142">id</span><span class="sxs-lookup"><span data-stu-id="d5431-142">id</span></span>|<span data-ttu-id="d5431-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d5431-143">String</span></span>|<span data-ttu-id="d5431-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d5431-144">Key of the entity.</span></span> <span data-ttu-id="d5431-145">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="d5431-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="d5431-146">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d5431-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d5431-147">displayName</span></span>|<span data-ttu-id="d5431-148">String</span><span class="sxs-lookup"><span data-stu-id="d5431-148">String</span></span>|<span data-ttu-id="d5431-149">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d5431-149">Display Name of the Role definition.</span></span> <span data-ttu-id="d5431-150">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d5431-151">说明</span><span class="sxs-lookup"><span data-stu-id="d5431-151">description</span></span>|<span data-ttu-id="d5431-152">String</span><span class="sxs-lookup"><span data-stu-id="d5431-152">String</span></span>|<span data-ttu-id="d5431-153">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="d5431-153">Description of the Role definition.</span></span> <span data-ttu-id="d5431-154">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d5431-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d5431-155">rolePermissions</span></span>|<span data-ttu-id="d5431-156">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5431-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d5431-157">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="d5431-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d5431-158">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="d5431-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="d5431-159">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d5431-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d5431-160">isBuiltIn</span></span>|<span data-ttu-id="d5431-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5431-161">Boolean</span></span>|<span data-ttu-id="d5431-162">角色类型。</span><span class="sxs-lookup"><span data-stu-id="d5431-162">Type of Role.</span></span> <span data-ttu-id="d5431-163">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="d5431-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="d5431-164">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5431-165">关系</span><span class="sxs-lookup"><span data-stu-id="d5431-165">Relationships</span></span>
|<span data-ttu-id="d5431-166">关系</span><span class="sxs-lookup"><span data-stu-id="d5431-166">Relationship</span></span>|<span data-ttu-id="d5431-167">类型</span><span class="sxs-lookup"><span data-stu-id="d5431-167">Type</span></span>|<span data-ttu-id="d5431-168">说明</span><span class="sxs-lookup"><span data-stu-id="d5431-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5431-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="d5431-169">roleAssignments</span></span>|<span data-ttu-id="d5431-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5431-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="d5431-171">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="d5431-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="d5431-172">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5431-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5431-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5431-173">JSON Representation</span></span>
<span data-ttu-id="d5431-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5431-174">Here is a JSON representation of the resource.</span></span>
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



