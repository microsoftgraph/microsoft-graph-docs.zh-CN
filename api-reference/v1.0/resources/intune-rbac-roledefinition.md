---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff5403f7741191021d45aeb6dfb87b2a299f4b85
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751186"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="aa8f1-109">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa8f1-109">roleDefinition resource type</span></span>

<span data-ttu-id="aa8f1-110">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa8f1-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa8f1-111">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa8f1-112">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-112">The Role Definition resource.</span></span> <span data-ttu-id="aa8f1-113">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="aa8f1-114">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="aa8f1-115">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="aa8f1-116">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="aa8f1-117">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="aa8f1-118">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="aa8f1-119">Methods</span><span class="sxs-lookup"><span data-stu-id="aa8f1-119">Methods</span></span>
|<span data-ttu-id="aa8f1-120">方法</span><span class="sxs-lookup"><span data-stu-id="aa8f1-120">Method</span></span>|<span data-ttu-id="aa8f1-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa8f1-121">Return Type</span></span>|<span data-ttu-id="aa8f1-122">Description</span><span class="sxs-lookup"><span data-stu-id="aa8f1-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa8f1-123">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="aa8f1-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="aa8f1-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8f1-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="aa8f1-125">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="aa8f1-126">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="aa8f1-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="aa8f1-128">读取 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="aa8f1-129">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="aa8f1-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="aa8f1-131">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="aa8f1-132">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="aa8f1-133">无</span><span class="sxs-lookup"><span data-stu-id="aa8f1-133">None</span></span>|<span data-ttu-id="aa8f1-134">删除 [roleDefinition](../resources/intune-rbac-roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="aa8f1-135">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="aa8f1-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa8f1-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="aa8f1-137">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa8f1-138">属性</span><span class="sxs-lookup"><span data-stu-id="aa8f1-138">Properties</span></span>
|<span data-ttu-id="aa8f1-139">属性</span><span class="sxs-lookup"><span data-stu-id="aa8f1-139">Property</span></span>|<span data-ttu-id="aa8f1-140">类型</span><span class="sxs-lookup"><span data-stu-id="aa8f1-140">Type</span></span>|<span data-ttu-id="aa8f1-141">说明</span><span class="sxs-lookup"><span data-stu-id="aa8f1-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa8f1-142">id</span><span class="sxs-lookup"><span data-stu-id="aa8f1-142">id</span></span>|<span data-ttu-id="aa8f1-143">String</span><span class="sxs-lookup"><span data-stu-id="aa8f1-143">String</span></span>|<span data-ttu-id="aa8f1-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-144">Key of the entity.</span></span> <span data-ttu-id="aa8f1-145">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="aa8f1-146">displayName</span><span class="sxs-lookup"><span data-stu-id="aa8f1-146">displayName</span></span>|<span data-ttu-id="aa8f1-147">String</span><span class="sxs-lookup"><span data-stu-id="aa8f1-147">String</span></span>|<span data-ttu-id="aa8f1-148">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="aa8f1-149">说明</span><span class="sxs-lookup"><span data-stu-id="aa8f1-149">description</span></span>|<span data-ttu-id="aa8f1-150">String</span><span class="sxs-lookup"><span data-stu-id="aa8f1-150">String</span></span>|<span data-ttu-id="aa8f1-151">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="aa8f1-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="aa8f1-152">rolePermissions</span></span>|<span data-ttu-id="aa8f1-153">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8f1-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="aa8f1-154">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="aa8f1-155">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="aa8f1-156">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="aa8f1-156">isBuiltIn</span></span>|<span data-ttu-id="aa8f1-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa8f1-157">Boolean</span></span>|<span data-ttu-id="aa8f1-158">角色类型。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-158">Type of Role.</span></span> <span data-ttu-id="aa8f1-159">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa8f1-160">关系</span><span class="sxs-lookup"><span data-stu-id="aa8f1-160">Relationships</span></span>
|<span data-ttu-id="aa8f1-161">关系</span><span class="sxs-lookup"><span data-stu-id="aa8f1-161">Relationship</span></span>|<span data-ttu-id="aa8f1-162">类型</span><span class="sxs-lookup"><span data-stu-id="aa8f1-162">Type</span></span>|<span data-ttu-id="aa8f1-163">Description</span><span class="sxs-lookup"><span data-stu-id="aa8f1-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa8f1-164">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="aa8f1-164">roleAssignments</span></span>|<span data-ttu-id="aa8f1-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8f1-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="aa8f1-166">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="aa8f1-166">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa8f1-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa8f1-167">JSON Representation</span></span>
<span data-ttu-id="aa8f1-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa8f1-168">Here is a JSON representation of the resource.</span></span>
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




