---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
ms.openlocfilehash: 15be13c0a893ed0cdc7b77b47591cc28d32c9889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009706"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="b6a4b-109">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6a4b-109">roleDefinition resource type</span></span>

> <span data-ttu-id="b6a4b-110">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6a4b-111">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-111">The Role Definition resource.</span></span> <span data-ttu-id="b6a4b-112">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="b6a4b-113">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="b6a4b-114">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="b6a4b-115">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="b6a4b-116">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="b6a4b-117">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="b6a4b-118">方法</span><span class="sxs-lookup"><span data-stu-id="b6a4b-118">Methods</span></span>
|<span data-ttu-id="b6a4b-119">方法</span><span class="sxs-lookup"><span data-stu-id="b6a4b-119">Method</span></span>|<span data-ttu-id="b6a4b-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6a4b-120">Return Type</span></span>|<span data-ttu-id="b6a4b-121">说明</span><span class="sxs-lookup"><span data-stu-id="b6a4b-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6a4b-122">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="b6a4b-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="b6a4b-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6a4b-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="b6a4b-124">列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="b6a4b-125">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="b6a4b-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b6a4b-127">读取 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="b6a4b-128">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="b6a4b-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b6a4b-130">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="b6a4b-131">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="b6a4b-132">无</span><span class="sxs-lookup"><span data-stu-id="b6a4b-132">None</span></span>|<span data-ttu-id="b6a4b-133">删除 [roleDefinition](../resources/intune-rbac-roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="b6a4b-134">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="b6a4b-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b6a4b-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="b6a4b-136">更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6a4b-137">属性</span><span class="sxs-lookup"><span data-stu-id="b6a4b-137">Properties</span></span>
|<span data-ttu-id="b6a4b-138">属性</span><span class="sxs-lookup"><span data-stu-id="b6a4b-138">Property</span></span>|<span data-ttu-id="b6a4b-139">类型</span><span class="sxs-lookup"><span data-stu-id="b6a4b-139">Type</span></span>|<span data-ttu-id="b6a4b-140">说明</span><span class="sxs-lookup"><span data-stu-id="b6a4b-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a4b-141">id</span><span class="sxs-lookup"><span data-stu-id="b6a4b-141">id</span></span>|<span data-ttu-id="b6a4b-142">String</span><span class="sxs-lookup"><span data-stu-id="b6a4b-142">String</span></span>|<span data-ttu-id="b6a4b-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-143">Key of the entity.</span></span> <span data-ttu-id="b6a4b-144">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b6a4b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b6a4b-145">displayName</span></span>|<span data-ttu-id="b6a4b-146">String</span><span class="sxs-lookup"><span data-stu-id="b6a4b-146">String</span></span>|<span data-ttu-id="b6a4b-147">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="b6a4b-148">说明</span><span class="sxs-lookup"><span data-stu-id="b6a4b-148">description</span></span>|<span data-ttu-id="b6a4b-149">String</span><span class="sxs-lookup"><span data-stu-id="b6a4b-149">String</span></span>|<span data-ttu-id="b6a4b-150">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="b6a4b-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="b6a4b-151">rolePermissions</span></span>|<span data-ttu-id="b6a4b-152">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6a4b-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b6a4b-153">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b6a4b-154">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b6a4b-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b6a4b-155">isBuiltIn</span></span>|<span data-ttu-id="b6a4b-156">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6a4b-156">Boolean</span></span>|<span data-ttu-id="b6a4b-157">角色类型。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-157">Type of Role.</span></span> <span data-ttu-id="b6a4b-158">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6a4b-159">关系</span><span class="sxs-lookup"><span data-stu-id="b6a4b-159">Relationships</span></span>
|<span data-ttu-id="b6a4b-160">关系</span><span class="sxs-lookup"><span data-stu-id="b6a4b-160">Relationship</span></span>|<span data-ttu-id="b6a4b-161">类型</span><span class="sxs-lookup"><span data-stu-id="b6a4b-161">Type</span></span>|<span data-ttu-id="b6a4b-162">说明</span><span class="sxs-lookup"><span data-stu-id="b6a4b-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a4b-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="b6a4b-163">roleAssignments</span></span>|<span data-ttu-id="b6a4b-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6a4b-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="b6a4b-165">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="b6a4b-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6a4b-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6a4b-166">JSON Representation</span></span>
<span data-ttu-id="b6a4b-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6a4b-167">Here is a JSON representation of the resource.</span></span>
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



