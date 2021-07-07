---
title: unifiedRoleDefinition 资源类型
description: 统一角色定义是权限的集合
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 804315ae2ae4b803088a419913ca91c11a8e51c4
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316494"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="4411b-103">unifiedRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="4411b-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="4411b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4411b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4411b-105">表示列出操作（如读取、写入和删除）的权限集合，这些操作可在 RBAC 角色管理中由 RBAC Microsoft 365[执行](rolemanagement.md)。</span><span class="sxs-lookup"><span data-stu-id="4411b-105">Represents a collection of permissions listing the operations, such as read, write, and delete, that can be performed by an RBAC provider, as part of Microsoft 365 RBAC [role management](rolemanagement.md).</span></span>

<span data-ttu-id="4411b-106">目前支持以下 RBAC 提供程序：</span><span class="sxs-lookup"><span data-stu-id="4411b-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="4411b-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="4411b-107">cloud PC</span></span> 
- <span data-ttu-id="4411b-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="4411b-108">device management (Intune)</span></span>
- <span data-ttu-id="4411b-109">Azure AD (目录) </span><span class="sxs-lookup"><span data-stu-id="4411b-109">directory (Azure AD)</span></span> 
- <span data-ttu-id="4411b-110">Azure AD (授权) </span><span class="sxs-lookup"><span data-stu-id="4411b-110">entitlement management (Azure AD)</span></span>

> [!NOTE]
> <span data-ttu-id="4411b-111">云电脑和权利管理 RBAC 提供程序当前仅支持[列表和](../api/rbacapplication-list-roledefinitions.md)[获取](../api/unifiedroledefinition-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="4411b-111">The cloud PC and entitlement management RBAC providers currently support only the [list](../api/rbacapplication-list-roledefinitions.md) and [get](../api/unifiedroledefinition-get.md) operations.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="4411b-112">Methods</span><span class="sxs-lookup"><span data-stu-id="4411b-112">Methods</span></span>

| <span data-ttu-id="4411b-113">方法</span><span class="sxs-lookup"><span data-stu-id="4411b-113">Method</span></span>       | <span data-ttu-id="4411b-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="4411b-114">Return Type</span></span> | <span data-ttu-id="4411b-115">说明</span><span class="sxs-lookup"><span data-stu-id="4411b-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4411b-116">列出 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-116">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="4411b-117">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4411b-117">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="4411b-118">读取 unifiedRoleDefinition 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="4411b-118">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="4411b-119">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-119">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="4411b-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="4411b-121">读取 unifiedRoleDefinition 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4411b-121">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="4411b-122">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-122">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="4411b-123">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-123">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="4411b-124">创建 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="4411b-124">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="4411b-125">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-125">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="4411b-126">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-126">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="4411b-127">更新 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="4411b-127">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="4411b-128">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4411b-128">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="4411b-129">无</span><span class="sxs-lookup"><span data-stu-id="4411b-129">None</span></span> | <span data-ttu-id="4411b-130">删除 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="4411b-130">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4411b-131">属性</span><span class="sxs-lookup"><span data-stu-id="4411b-131">Properties</span></span>

| <span data-ttu-id="4411b-132">属性</span><span class="sxs-lookup"><span data-stu-id="4411b-132">Property</span></span>     | <span data-ttu-id="4411b-133">类型</span><span class="sxs-lookup"><span data-stu-id="4411b-133">Type</span></span>        | <span data-ttu-id="4411b-134">说明</span><span class="sxs-lookup"><span data-stu-id="4411b-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4411b-135">说明</span><span class="sxs-lookup"><span data-stu-id="4411b-135">description</span></span>|<span data-ttu-id="4411b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4411b-136">String</span></span>| <span data-ttu-id="4411b-137">unifiedRoleDefinition 的说明。</span><span class="sxs-lookup"><span data-stu-id="4411b-137">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="4411b-138">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-138">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="4411b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="4411b-139">displayName</span></span>|<span data-ttu-id="4411b-140">字符串</span><span class="sxs-lookup"><span data-stu-id="4411b-140">String</span></span>| <span data-ttu-id="4411b-141">unifiedRoleDefinition 的 显示名称。</span><span class="sxs-lookup"><span data-stu-id="4411b-141">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="4411b-142">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-142">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="4411b-143">必需项。</span><span class="sxs-lookup"><span data-stu-id="4411b-143">Required.</span></span>  <span data-ttu-id="4411b-144">仅 `$filter` (`eq` `startsWith` 和运算符) 。</span><span class="sxs-lookup"><span data-stu-id="4411b-144">Supports `$filter` (`eq` and `startsWith` operators only).</span></span>|
|<span data-ttu-id="4411b-145">id</span><span class="sxs-lookup"><span data-stu-id="4411b-145">id</span></span>|<span data-ttu-id="4411b-146">字符串</span><span class="sxs-lookup"><span data-stu-id="4411b-146">String</span></span>| <span data-ttu-id="4411b-147">unifiedRoleDefinition 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4411b-147">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="4411b-148">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-148">Key, not nullable, Read-only.</span></span>  <span data-ttu-id="4411b-149">仅 `$filter` (`eq` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="4411b-149">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="4411b-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4411b-150">isBuiltIn</span></span>|<span data-ttu-id="4411b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4411b-151">Boolean</span></span>| <span data-ttu-id="4411b-152">指示 unifiedRoleDefinition 是否属于产品或自定义中包含的默认集的标志。</span><span class="sxs-lookup"><span data-stu-id="4411b-152">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="4411b-153">只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-153">Read-only.</span></span>  <span data-ttu-id="4411b-154">仅 `$filter` (`eq` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="4411b-154">Supports `$filter` (`eq` operator only).</span></span>|
|<span data-ttu-id="4411b-155">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4411b-155">isEnabled</span></span>|<span data-ttu-id="4411b-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4411b-156">Boolean</span></span>| <span data-ttu-id="4411b-157">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="4411b-157">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="4411b-158">如果为 false，则角色不能用于分配。</span><span class="sxs-lookup"><span data-stu-id="4411b-158">If false the role is not available for assignment.</span></span> <span data-ttu-id="4411b-159">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-159">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="4411b-160">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="4411b-160">resourceScopes</span></span>|<span data-ttu-id="4411b-161">String collection</span><span class="sxs-lookup"><span data-stu-id="4411b-161">String collection</span></span>| <span data-ttu-id="4411b-162">角色定义授予的作用域权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="4411b-162">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="4411b-163">当前仅 `/` 受支持。</span><span class="sxs-lookup"><span data-stu-id="4411b-163">Currently only `/` is supported.</span></span> <span data-ttu-id="4411b-164">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-164">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="4411b-165">**请勿使用。这将很快被弃用。将作用域附加到角色分配**</span><span class="sxs-lookup"><span data-stu-id="4411b-165">**DO NOT USE. This is going to be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="4411b-166">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="4411b-166">rolePermissions</span></span>|<span data-ttu-id="4411b-167">[unifiedRolePermission](unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4411b-167">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="4411b-168">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="4411b-168">List of permissions included in the role.</span></span> <span data-ttu-id="4411b-169">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-169">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="4411b-170">必需项。</span><span class="sxs-lookup"><span data-stu-id="4411b-170">Required.</span></span> |
|<span data-ttu-id="4411b-171">templateId</span><span class="sxs-lookup"><span data-stu-id="4411b-171">templateId</span></span>|<span data-ttu-id="4411b-172">字符串</span><span class="sxs-lookup"><span data-stu-id="4411b-172">String</span></span>| <span data-ttu-id="4411b-173">可以在 isBuiltIn 为 false 时设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="4411b-173">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="4411b-174">如果一个标识符在不同目录之间需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="4411b-174">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="4411b-175">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-175">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="4411b-176">version</span><span class="sxs-lookup"><span data-stu-id="4411b-176">version</span></span>|<span data-ttu-id="4411b-177">String</span><span class="sxs-lookup"><span data-stu-id="4411b-177">String</span></span>| <span data-ttu-id="4411b-178">指示 unifiedRoleDefinition 的版本。</span><span class="sxs-lookup"><span data-stu-id="4411b-178">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="4411b-179">**isBuiltIn** 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="4411b-179">Read-only when **isBuiltIn** is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4411b-180">关系</span><span class="sxs-lookup"><span data-stu-id="4411b-180">Relationships</span></span>

| <span data-ttu-id="4411b-181">关系</span><span class="sxs-lookup"><span data-stu-id="4411b-181">Relationship</span></span> | <span data-ttu-id="4411b-182">类型</span><span class="sxs-lookup"><span data-stu-id="4411b-182">Type</span></span>   |<span data-ttu-id="4411b-183">说明</span><span class="sxs-lookup"><span data-stu-id="4411b-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4411b-184">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="4411b-184">inheritsPermissionsFrom</span></span>| <span data-ttu-id="4411b-185">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4411b-185">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="4411b-186">给定角色定义从其继承的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="4411b-186">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="4411b-187">仅 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="4411b-187">Only Azure AD built-in roles support this attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4411b-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4411b-188">JSON representation</span></span>

<span data-ttu-id="4411b-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4411b-189">The following is a JSON representation of the resource.</span></span>

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


