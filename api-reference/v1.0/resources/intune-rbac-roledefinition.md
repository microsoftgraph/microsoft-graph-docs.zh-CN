---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fca3587ccb26116257b740a91b376259e1e9dd5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262361"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="71067-109">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="71067-109">roleDefinition resource type</span></span>

> <span data-ttu-id="71067-110">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71067-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71067-111">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="71067-111">The Role Definition resource.</span></span> <span data-ttu-id="71067-112">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="71067-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="71067-113">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="71067-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="71067-114">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="71067-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="71067-115">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="71067-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="71067-116">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="71067-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="71067-117">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="71067-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="71067-118">方法</span><span class="sxs-lookup"><span data-stu-id="71067-118">Methods</span></span>
|<span data-ttu-id="71067-119">方法</span><span class="sxs-lookup"><span data-stu-id="71067-119">Method</span></span>|<span data-ttu-id="71067-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="71067-120">Return Type</span></span>|<span data-ttu-id="71067-121">说明</span><span class="sxs-lookup"><span data-stu-id="71067-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71067-122">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="71067-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="71067-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71067-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="71067-124">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71067-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="71067-125">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="71067-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="71067-127">读取 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71067-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="71067-128">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="71067-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="71067-130">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71067-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="71067-131">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="71067-132">无</span><span class="sxs-lookup"><span data-stu-id="71067-132">None</span></span>|<span data-ttu-id="71067-133">删除 [roleDefinition](../resources/intune-rbac-roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="71067-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="71067-134">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="71067-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="71067-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="71067-136">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71067-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71067-137">属性</span><span class="sxs-lookup"><span data-stu-id="71067-137">Properties</span></span>
|<span data-ttu-id="71067-138">属性</span><span class="sxs-lookup"><span data-stu-id="71067-138">Property</span></span>|<span data-ttu-id="71067-139">类型</span><span class="sxs-lookup"><span data-stu-id="71067-139">Type</span></span>|<span data-ttu-id="71067-140">说明</span><span class="sxs-lookup"><span data-stu-id="71067-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71067-141">id</span><span class="sxs-lookup"><span data-stu-id="71067-141">id</span></span>|<span data-ttu-id="71067-142">String</span><span class="sxs-lookup"><span data-stu-id="71067-142">String</span></span>|<span data-ttu-id="71067-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71067-143">Key of the entity.</span></span> <span data-ttu-id="71067-144">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="71067-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="71067-145">displayName</span><span class="sxs-lookup"><span data-stu-id="71067-145">displayName</span></span>|<span data-ttu-id="71067-146">String</span><span class="sxs-lookup"><span data-stu-id="71067-146">String</span></span>|<span data-ttu-id="71067-147">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="71067-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="71067-148">说明</span><span class="sxs-lookup"><span data-stu-id="71067-148">description</span></span>|<span data-ttu-id="71067-149">String</span><span class="sxs-lookup"><span data-stu-id="71067-149">String</span></span>|<span data-ttu-id="71067-150">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="71067-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="71067-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="71067-151">rolePermissions</span></span>|<span data-ttu-id="71067-152">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71067-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="71067-153">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="71067-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="71067-154">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="71067-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="71067-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="71067-155">isBuiltIn</span></span>|<span data-ttu-id="71067-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="71067-156">Boolean</span></span>|<span data-ttu-id="71067-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="71067-157">Type of Role.</span></span> <span data-ttu-id="71067-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="71067-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71067-159">关系</span><span class="sxs-lookup"><span data-stu-id="71067-159">Relationships</span></span>
|<span data-ttu-id="71067-160">关系</span><span class="sxs-lookup"><span data-stu-id="71067-160">Relationship</span></span>|<span data-ttu-id="71067-161">类型</span><span class="sxs-lookup"><span data-stu-id="71067-161">Type</span></span>|<span data-ttu-id="71067-162">说明</span><span class="sxs-lookup"><span data-stu-id="71067-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71067-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="71067-163">roleAssignments</span></span>|<span data-ttu-id="71067-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71067-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="71067-165">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="71067-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71067-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71067-166">JSON Representation</span></span>
<span data-ttu-id="71067-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71067-167">Here is a JSON representation of the resource.</span></span>
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



