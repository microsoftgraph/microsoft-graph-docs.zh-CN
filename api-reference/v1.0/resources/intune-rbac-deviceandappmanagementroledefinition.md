---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b3241a8cdd909f6e267b5016167c89aaa6fb7b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447953"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="cea2e-109">deviceAndAppManagementRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="cea2e-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="cea2e-110">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cea2e-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cea2e-111">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cea2e-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cea2e-112">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="cea2e-112">The Role Definition resource.</span></span> <span data-ttu-id="cea2e-113">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="cea2e-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="cea2e-114">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="cea2e-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="cea2e-115">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="cea2e-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="cea2e-116">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="cea2e-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="cea2e-117">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="cea2e-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="cea2e-118">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="cea2e-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="cea2e-119">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cea2e-120">方法</span><span class="sxs-lookup"><span data-stu-id="cea2e-120">Methods</span></span>
|<span data-ttu-id="cea2e-121">方法</span><span class="sxs-lookup"><span data-stu-id="cea2e-121">Method</span></span>|<span data-ttu-id="cea2e-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="cea2e-122">Return Type</span></span>|<span data-ttu-id="cea2e-123">说明</span><span class="sxs-lookup"><span data-stu-id="cea2e-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cea2e-124">List deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="cea2e-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="cea2e-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cea2e-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="cea2e-126">列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cea2e-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="cea2e-127">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="cea2e-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="cea2e-129">读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cea2e-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="cea2e-130">Create deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="cea2e-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="cea2e-132">创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cea2e-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="cea2e-133">Delete deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="cea2e-134">无</span><span class="sxs-lookup"><span data-stu-id="cea2e-134">None</span></span>|<span data-ttu-id="cea2e-135">删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="cea2e-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="cea2e-136">Update deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="cea2e-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cea2e-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="cea2e-138">更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cea2e-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cea2e-139">属性</span><span class="sxs-lookup"><span data-stu-id="cea2e-139">Properties</span></span>
|<span data-ttu-id="cea2e-140">属性</span><span class="sxs-lookup"><span data-stu-id="cea2e-140">Property</span></span>|<span data-ttu-id="cea2e-141">类型</span><span class="sxs-lookup"><span data-stu-id="cea2e-141">Type</span></span>|<span data-ttu-id="cea2e-142">说明</span><span class="sxs-lookup"><span data-stu-id="cea2e-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cea2e-143">id</span><span class="sxs-lookup"><span data-stu-id="cea2e-143">id</span></span>|<span data-ttu-id="cea2e-144">字符串</span><span class="sxs-lookup"><span data-stu-id="cea2e-144">String</span></span>|<span data-ttu-id="cea2e-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cea2e-145">Key of the entity.</span></span> <span data-ttu-id="cea2e-146">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="cea2e-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="cea2e-147">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="cea2e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="cea2e-148">displayName</span></span>|<span data-ttu-id="cea2e-149">String</span><span class="sxs-lookup"><span data-stu-id="cea2e-149">String</span></span>|<span data-ttu-id="cea2e-150">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cea2e-150">Display Name of the Role definition.</span></span> <span data-ttu-id="cea2e-151">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="cea2e-152">说明</span><span class="sxs-lookup"><span data-stu-id="cea2e-152">description</span></span>|<span data-ttu-id="cea2e-153">String</span><span class="sxs-lookup"><span data-stu-id="cea2e-153">String</span></span>|<span data-ttu-id="cea2e-154">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="cea2e-154">Description of the Role definition.</span></span> <span data-ttu-id="cea2e-155">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="cea2e-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cea2e-156">rolePermissions</span></span>|<span data-ttu-id="cea2e-157">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cea2e-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cea2e-158">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="cea2e-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cea2e-159">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="cea2e-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="cea2e-160">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="cea2e-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cea2e-161">isBuiltIn</span></span>|<span data-ttu-id="cea2e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cea2e-162">Boolean</span></span>|<span data-ttu-id="cea2e-163">角色类型。</span><span class="sxs-lookup"><span data-stu-id="cea2e-163">Type of Role.</span></span> <span data-ttu-id="cea2e-164">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="cea2e-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="cea2e-165">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cea2e-166">关系</span><span class="sxs-lookup"><span data-stu-id="cea2e-166">Relationships</span></span>
|<span data-ttu-id="cea2e-167">关系</span><span class="sxs-lookup"><span data-stu-id="cea2e-167">Relationship</span></span>|<span data-ttu-id="cea2e-168">类型</span><span class="sxs-lookup"><span data-stu-id="cea2e-168">Type</span></span>|<span data-ttu-id="cea2e-169">说明</span><span class="sxs-lookup"><span data-stu-id="cea2e-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cea2e-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="cea2e-170">roleAssignments</span></span>|<span data-ttu-id="cea2e-171">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cea2e-171">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="cea2e-172">此角色定义的角色分配列表。</span><span class="sxs-lookup"><span data-stu-id="cea2e-172">List of Role assignments for this role definition.</span></span> <span data-ttu-id="cea2e-173">继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cea2e-173">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cea2e-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cea2e-174">JSON Representation</span></span>
<span data-ttu-id="cea2e-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cea2e-175">Here is a JSON representation of the resource.</span></span>
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




