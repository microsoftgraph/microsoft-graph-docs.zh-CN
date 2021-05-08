---
title: unifiedRoleDefinition 资源类型
description: 统一角色定义是权限的集合
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e9f44d194eb2eebf961abf40d49aac302f9db4b5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239777"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="cce41-103">unifiedRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="cce41-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="cce41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cce41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cce41-105">unifiedRoleDefinition 是列出可以执行的操作（如读取、写入和删除）的权限集合。</span><span class="sxs-lookup"><span data-stu-id="cce41-105">A unifiedRoleDefinition is a collection of permissions listing the operations that can be performed, such as read, write, and delete.</span></span>

## <a name="methods"></a><span data-ttu-id="cce41-106">方法</span><span class="sxs-lookup"><span data-stu-id="cce41-106">Methods</span></span>

| <span data-ttu-id="cce41-107">方法</span><span class="sxs-lookup"><span data-stu-id="cce41-107">Method</span></span>       | <span data-ttu-id="cce41-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cce41-108">Return Type</span></span> | <span data-ttu-id="cce41-109">说明</span><span class="sxs-lookup"><span data-stu-id="cce41-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cce41-110">列出 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-110">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="cce41-111">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce41-111">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="cce41-112">读取 unifiedRoleDefinition 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="cce41-112">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="cce41-113">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-113">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="cce41-114">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-114">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="cce41-115">读取 unifiedRoleDefinition 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cce41-115">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="cce41-116">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-116">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="cce41-117">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-117">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="cce41-118">创建 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="cce41-118">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="cce41-119">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-119">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="cce41-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="cce41-121">更新 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="cce41-121">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="cce41-122">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cce41-122">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="cce41-123">无</span><span class="sxs-lookup"><span data-stu-id="cce41-123">None</span></span> | <span data-ttu-id="cce41-124">删除 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="cce41-124">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cce41-125">属性</span><span class="sxs-lookup"><span data-stu-id="cce41-125">Properties</span></span>

| <span data-ttu-id="cce41-126">属性</span><span class="sxs-lookup"><span data-stu-id="cce41-126">Property</span></span>     | <span data-ttu-id="cce41-127">类型</span><span class="sxs-lookup"><span data-stu-id="cce41-127">Type</span></span>        | <span data-ttu-id="cce41-128">说明</span><span class="sxs-lookup"><span data-stu-id="cce41-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cce41-129">说明</span><span class="sxs-lookup"><span data-stu-id="cce41-129">description</span></span>|<span data-ttu-id="cce41-130">字符串</span><span class="sxs-lookup"><span data-stu-id="cce41-130">String</span></span>| <span data-ttu-id="cce41-131">unifiedRoleDefinition 的说明。</span><span class="sxs-lookup"><span data-stu-id="cce41-131">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="cce41-132">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-132">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="cce41-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cce41-133">displayName</span></span>|<span data-ttu-id="cce41-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cce41-134">String</span></span>| <span data-ttu-id="cce41-135">unifiedRoleDefinition 的 显示名称。</span><span class="sxs-lookup"><span data-stu-id="cce41-135">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="cce41-136">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-136">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="cce41-137">必需。</span><span class="sxs-lookup"><span data-stu-id="cce41-137">Required.</span></span>  <span data-ttu-id="cce41-138">仅 `$filter` (`eq` `startsWith` 和运算符) 。</span><span class="sxs-lookup"><span data-stu-id="cce41-138">Supports `$filter` (`eq` and `startsWith` operators only).</span></span>|
|<span data-ttu-id="cce41-139">id</span><span class="sxs-lookup"><span data-stu-id="cce41-139">id</span></span>|<span data-ttu-id="cce41-140">字符串</span><span class="sxs-lookup"><span data-stu-id="cce41-140">String</span></span>| <span data-ttu-id="cce41-141">unifiedRoleDefinition 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cce41-141">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="cce41-142">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-142">Key, not nullable, Read-only.</span></span>  <span data-ttu-id="cce41-143">仅 `$filter` (`eq` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="cce41-143">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="cce41-144">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cce41-144">isBuiltIn</span></span>|<span data-ttu-id="cce41-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cce41-145">Boolean</span></span>| <span data-ttu-id="cce41-146">指示 unifiedRoleDefinition 是否属于产品或自定义中包含的默认集的标志。</span><span class="sxs-lookup"><span data-stu-id="cce41-146">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="cce41-147">只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-147">Read-only.</span></span>  <span data-ttu-id="cce41-148">仅 `$filter` (`eq` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="cce41-148">Supports `$filter` (`eq` operator only).</span></span>|
|<span data-ttu-id="cce41-149">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cce41-149">isEnabled</span></span>|<span data-ttu-id="cce41-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="cce41-150">Boolean</span></span>| <span data-ttu-id="cce41-151">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="cce41-151">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="cce41-152">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="cce41-152">If false the role is not available for assignment.</span></span> <span data-ttu-id="cce41-153">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-153">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="cce41-154">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="cce41-154">resourceScopes</span></span>|<span data-ttu-id="cce41-155">String collection</span><span class="sxs-lookup"><span data-stu-id="cce41-155">String collection</span></span>| <span data-ttu-id="cce41-156">角色定义授予的作用域权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="cce41-156">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="cce41-157">当前仅 `/` 受支持。</span><span class="sxs-lookup"><span data-stu-id="cce41-157">Currently only `/` is supported.</span></span> <span data-ttu-id="cce41-158">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-158">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="cce41-159">**请勿使用。这将很快被弃用。将作用域附加到角色分配**</span><span class="sxs-lookup"><span data-stu-id="cce41-159">**DO NOT USE. This is going to be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="cce41-160">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cce41-160">rolePermissions</span></span>|<span data-ttu-id="cce41-161">[unifiedRolePermission](unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce41-161">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="cce41-162">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="cce41-162">List of permissions included in the role.</span></span> <span data-ttu-id="cce41-163">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-163">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="cce41-164">必需。</span><span class="sxs-lookup"><span data-stu-id="cce41-164">Required.</span></span> |
|<span data-ttu-id="cce41-165">templateId</span><span class="sxs-lookup"><span data-stu-id="cce41-165">templateId</span></span>|<span data-ttu-id="cce41-166">字符串</span><span class="sxs-lookup"><span data-stu-id="cce41-166">String</span></span>| <span data-ttu-id="cce41-167">可以在 isBuiltIn 为 false 时设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="cce41-167">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="cce41-168">如果一个标识符在不同目录之间需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="cce41-168">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="cce41-169">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-169">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="cce41-170">version</span><span class="sxs-lookup"><span data-stu-id="cce41-170">version</span></span>|<span data-ttu-id="cce41-171">String</span><span class="sxs-lookup"><span data-stu-id="cce41-171">String</span></span>| <span data-ttu-id="cce41-172">指示 unifiedRoleDefinition 的版本。</span><span class="sxs-lookup"><span data-stu-id="cce41-172">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="cce41-173">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="cce41-173">Read-only when **isBuiltIn** is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cce41-174">关系</span><span class="sxs-lookup"><span data-stu-id="cce41-174">Relationships</span></span>

| <span data-ttu-id="cce41-175">关系</span><span class="sxs-lookup"><span data-stu-id="cce41-175">Relationship</span></span> | <span data-ttu-id="cce41-176">类型</span><span class="sxs-lookup"><span data-stu-id="cce41-176">Type</span></span>   |<span data-ttu-id="cce41-177">说明</span><span class="sxs-lookup"><span data-stu-id="cce41-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cce41-178">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="cce41-178">inheritsPermissionsFrom</span></span>| <span data-ttu-id="cce41-179">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cce41-179">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="cce41-180">给定角色定义从其继承的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="cce41-180">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="cce41-181">仅 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="cce41-181">Only Azure AD built-in roles support this attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cce41-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cce41-182">JSON representation</span></span>

<span data-ttu-id="cce41-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cce41-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "inheritsPermissionsFrom": [{"@odata.type": "microsoft.graph.unifiedRoleDefinition"}],
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


