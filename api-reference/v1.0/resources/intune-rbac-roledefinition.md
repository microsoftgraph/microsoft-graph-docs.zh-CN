---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2704b26265a6e1f39ef7d7383f1ade1ef1ffc9ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037792"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="9af06-109">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="9af06-109">roleDefinition resource type</span></span>

<span data-ttu-id="9af06-110">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9af06-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9af06-111">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9af06-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9af06-112">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="9af06-112">The Role Definition resource.</span></span> <span data-ttu-id="9af06-113">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="9af06-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="9af06-114">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="9af06-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="9af06-115">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="9af06-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="9af06-116">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="9af06-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="9af06-117">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="9af06-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="9af06-118">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="9af06-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="9af06-119">方法</span><span class="sxs-lookup"><span data-stu-id="9af06-119">Methods</span></span>
|<span data-ttu-id="9af06-120">方法</span><span class="sxs-lookup"><span data-stu-id="9af06-120">Method</span></span>|<span data-ttu-id="9af06-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="9af06-121">Return Type</span></span>|<span data-ttu-id="9af06-122">说明</span><span class="sxs-lookup"><span data-stu-id="9af06-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9af06-123">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="9af06-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="9af06-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af06-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="9af06-125">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9af06-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="9af06-126">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="9af06-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="9af06-128">读取 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9af06-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="9af06-129">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="9af06-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="9af06-131">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9af06-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="9af06-132">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="9af06-133">无</span><span class="sxs-lookup"><span data-stu-id="9af06-133">None</span></span>|<span data-ttu-id="9af06-134">删除 [roleDefinition](../resources/intune-rbac-roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9af06-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="9af06-135">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="9af06-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9af06-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="9af06-137">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9af06-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9af06-138">属性</span><span class="sxs-lookup"><span data-stu-id="9af06-138">Properties</span></span>
|<span data-ttu-id="9af06-139">属性</span><span class="sxs-lookup"><span data-stu-id="9af06-139">Property</span></span>|<span data-ttu-id="9af06-140">类型</span><span class="sxs-lookup"><span data-stu-id="9af06-140">Type</span></span>|<span data-ttu-id="9af06-141">说明</span><span class="sxs-lookup"><span data-stu-id="9af06-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9af06-142">id</span><span class="sxs-lookup"><span data-stu-id="9af06-142">id</span></span>|<span data-ttu-id="9af06-143">String</span><span class="sxs-lookup"><span data-stu-id="9af06-143">String</span></span>|<span data-ttu-id="9af06-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9af06-144">Key of the entity.</span></span> <span data-ttu-id="9af06-145">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="9af06-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9af06-146">displayName</span><span class="sxs-lookup"><span data-stu-id="9af06-146">displayName</span></span>|<span data-ttu-id="9af06-147">String</span><span class="sxs-lookup"><span data-stu-id="9af06-147">String</span></span>|<span data-ttu-id="9af06-148">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9af06-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="9af06-149">description</span><span class="sxs-lookup"><span data-stu-id="9af06-149">description</span></span>|<span data-ttu-id="9af06-150">String</span><span class="sxs-lookup"><span data-stu-id="9af06-150">String</span></span>|<span data-ttu-id="9af06-151">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="9af06-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="9af06-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="9af06-152">rolePermissions</span></span>|<span data-ttu-id="9af06-153">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af06-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="9af06-154">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="9af06-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="9af06-155">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="9af06-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="9af06-156">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="9af06-156">isBuiltIn</span></span>|<span data-ttu-id="9af06-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="9af06-157">Boolean</span></span>|<span data-ttu-id="9af06-158">角色类型。</span><span class="sxs-lookup"><span data-stu-id="9af06-158">Type of Role.</span></span> <span data-ttu-id="9af06-159">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="9af06-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9af06-160">关系</span><span class="sxs-lookup"><span data-stu-id="9af06-160">Relationships</span></span>
|<span data-ttu-id="9af06-161">关系</span><span class="sxs-lookup"><span data-stu-id="9af06-161">Relationship</span></span>|<span data-ttu-id="9af06-162">类型</span><span class="sxs-lookup"><span data-stu-id="9af06-162">Type</span></span>|<span data-ttu-id="9af06-163">说明</span><span class="sxs-lookup"><span data-stu-id="9af06-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9af06-164">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="9af06-164">roleAssignments</span></span>|<span data-ttu-id="9af06-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af06-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="9af06-166">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="9af06-166">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9af06-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9af06-167">JSON Representation</span></span>
<span data-ttu-id="9af06-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9af06-168">Here is a JSON representation of the resource.</span></span>
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









