---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f0f2fc18315b6c07c24cd95f5d88ce81f72e1f3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360802"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="b2eac-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2eac-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="b2eac-110">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2eac-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2eac-111">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="b2eac-111">The Role Definition resource.</span></span> <span data-ttu-id="b2eac-112">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="b2eac-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="b2eac-113">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="b2eac-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="b2eac-114">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="b2eac-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="b2eac-115">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="b2eac-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="b2eac-116">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="b2eac-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="b2eac-117">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="b2eac-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="b2eac-118">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b2eac-119">方法</span><span class="sxs-lookup"><span data-stu-id="b2eac-119">Methods</span></span>
|<span data-ttu-id="b2eac-120">方法</span><span class="sxs-lookup"><span data-stu-id="b2eac-120">Method</span></span>|<span data-ttu-id="b2eac-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="b2eac-121">Return Type</span></span>|<span data-ttu-id="b2eac-122">说明</span><span class="sxs-lookup"><span data-stu-id="b2eac-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b2eac-123">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="b2eac-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="b2eac-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2eac-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="b2eac-125">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b2eac-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="b2eac-126">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="b2eac-127">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-127">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="b2eac-128">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b2eac-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="b2eac-129">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="b2eac-130">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-130">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="b2eac-131">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2eac-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="b2eac-132">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="b2eac-133">无</span><span class="sxs-lookup"><span data-stu-id="b2eac-133">None</span></span>|<span data-ttu-id="b2eac-134">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b2eac-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="b2eac-135">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="b2eac-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b2eac-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="b2eac-137">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b2eac-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2eac-138">属性</span><span class="sxs-lookup"><span data-stu-id="b2eac-138">Properties</span></span>
|<span data-ttu-id="b2eac-139">属性</span><span class="sxs-lookup"><span data-stu-id="b2eac-139">Property</span></span>|<span data-ttu-id="b2eac-140">类型</span><span class="sxs-lookup"><span data-stu-id="b2eac-140">Type</span></span>|<span data-ttu-id="b2eac-141">说明</span><span class="sxs-lookup"><span data-stu-id="b2eac-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2eac-142">id</span><span class="sxs-lookup"><span data-stu-id="b2eac-142">id</span></span>|<span data-ttu-id="b2eac-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b2eac-143">String</span></span>|<span data-ttu-id="b2eac-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b2eac-144">Key of the entity.</span></span> <span data-ttu-id="b2eac-145">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="b2eac-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="b2eac-146">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="b2eac-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b2eac-147">displayName</span></span>|<span data-ttu-id="b2eac-148">String</span><span class="sxs-lookup"><span data-stu-id="b2eac-148">String</span></span>|<span data-ttu-id="b2eac-149">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b2eac-149">Display Name of the Role definition.</span></span> <span data-ttu-id="b2eac-150">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="b2eac-151">说明</span><span class="sxs-lookup"><span data-stu-id="b2eac-151">description</span></span>|<span data-ttu-id="b2eac-152">String</span><span class="sxs-lookup"><span data-stu-id="b2eac-152">String</span></span>|<span data-ttu-id="b2eac-153">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="b2eac-153">Description of the Role definition.</span></span> <span data-ttu-id="b2eac-154">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="b2eac-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="b2eac-155">rolePermissions</span></span>|<span data-ttu-id="b2eac-156">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2eac-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b2eac-157">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="b2eac-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b2eac-158">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="b2eac-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="b2eac-159">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="b2eac-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b2eac-160">isBuiltIn</span></span>|<span data-ttu-id="b2eac-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2eac-161">Boolean</span></span>|<span data-ttu-id="b2eac-162">角色类型。</span><span class="sxs-lookup"><span data-stu-id="b2eac-162">Type of Role.</span></span> <span data-ttu-id="b2eac-163">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="b2eac-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="b2eac-164">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2eac-165">关系</span><span class="sxs-lookup"><span data-stu-id="b2eac-165">Relationships</span></span>
|<span data-ttu-id="b2eac-166">关系</span><span class="sxs-lookup"><span data-stu-id="b2eac-166">Relationship</span></span>|<span data-ttu-id="b2eac-167">类型</span><span class="sxs-lookup"><span data-stu-id="b2eac-167">Type</span></span>|<span data-ttu-id="b2eac-168">说明</span><span class="sxs-lookup"><span data-stu-id="b2eac-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2eac-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="b2eac-169">roleAssignments</span></span>|<span data-ttu-id="b2eac-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2eac-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="b2eac-171">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="b2eac-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="b2eac-172">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2eac-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2eac-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2eac-173">JSON Representation</span></span>
<span data-ttu-id="b2eac-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2eac-174">Here is a JSON representation of the resource.</span></span>
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




