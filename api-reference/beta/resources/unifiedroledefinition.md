---
title: unifiedRoleDefinition 资源类型
description: 统一的角色定义是权限的集合
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d146f215586533b9564d267c686a437f1314d54b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159827"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="80976-103">unifiedRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="80976-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="80976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80976-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80976-105">unifiedRoleDefinition 是列出可以执行的操作（如读取、写入和删除）的权限集合。</span><span class="sxs-lookup"><span data-stu-id="80976-105">A unifiedRoleDefinition is a collection of permissions listing the operations that can be performed, such as read, write, and delete.</span></span>

## <a name="methods"></a><span data-ttu-id="80976-106">方法</span><span class="sxs-lookup"><span data-stu-id="80976-106">Methods</span></span>

| <span data-ttu-id="80976-107">方法</span><span class="sxs-lookup"><span data-stu-id="80976-107">Method</span></span>       | <span data-ttu-id="80976-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="80976-108">Return Type</span></span> | <span data-ttu-id="80976-109">说明</span><span class="sxs-lookup"><span data-stu-id="80976-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="80976-110">列出 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-110">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="80976-111">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80976-111">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="80976-112">读取 unifiedRoleDefinition 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="80976-112">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="80976-113">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-113">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="80976-114">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-114">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="80976-115">读取 unifiedRoleDefinition 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="80976-115">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="80976-116">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-116">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="80976-117">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-117">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="80976-118">创建 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="80976-118">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="80976-119">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-119">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="80976-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="80976-121">更新 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="80976-121">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="80976-122">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80976-122">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="80976-123">无</span><span class="sxs-lookup"><span data-stu-id="80976-123">None</span></span> | <span data-ttu-id="80976-124">删除 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="80976-124">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80976-125">属性</span><span class="sxs-lookup"><span data-stu-id="80976-125">Properties</span></span>

| <span data-ttu-id="80976-126">属性</span><span class="sxs-lookup"><span data-stu-id="80976-126">Property</span></span>     | <span data-ttu-id="80976-127">类型</span><span class="sxs-lookup"><span data-stu-id="80976-127">Type</span></span>        | <span data-ttu-id="80976-128">说明</span><span class="sxs-lookup"><span data-stu-id="80976-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80976-129">说明</span><span class="sxs-lookup"><span data-stu-id="80976-129">description</span></span>|<span data-ttu-id="80976-130">String</span><span class="sxs-lookup"><span data-stu-id="80976-130">String</span></span>| <span data-ttu-id="80976-131">unifiedRoleDefinition 的说明。</span><span class="sxs-lookup"><span data-stu-id="80976-131">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="80976-132">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="80976-133">displayName</span><span class="sxs-lookup"><span data-stu-id="80976-133">displayName</span></span>|<span data-ttu-id="80976-134">String</span><span class="sxs-lookup"><span data-stu-id="80976-134">String</span></span>| <span data-ttu-id="80976-135">unifiedRoleDefinition 的 显示名称。</span><span class="sxs-lookup"><span data-stu-id="80976-135">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="80976-136">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="80976-137">必需。</span><span class="sxs-lookup"><span data-stu-id="80976-137">Required.</span></span>|
|<span data-ttu-id="80976-138">id</span><span class="sxs-lookup"><span data-stu-id="80976-138">id</span></span>|<span data-ttu-id="80976-139">String</span><span class="sxs-lookup"><span data-stu-id="80976-139">String</span></span>| <span data-ttu-id="80976-140">unifiedRoleDefinition 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="80976-140">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="80976-141">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="80976-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="80976-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="80976-142">isBuiltIn</span></span>|<span data-ttu-id="80976-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="80976-143">Boolean</span></span>| <span data-ttu-id="80976-144">指示 unifiedRoleDefinition 是否属于产品或自定义中包含的默认集的标志。</span><span class="sxs-lookup"><span data-stu-id="80976-144">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="80976-145">只读。</span><span class="sxs-lookup"><span data-stu-id="80976-145">Read-only.</span></span> |
|<span data-ttu-id="80976-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="80976-146">isEnabled</span></span>|<span data-ttu-id="80976-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="80976-147">Boolean</span></span>| <span data-ttu-id="80976-148">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="80976-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="80976-149">如果为 false，则角色不能分配。</span><span class="sxs-lookup"><span data-stu-id="80976-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="80976-150">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="80976-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="80976-151">resourceScopes</span></span>|<span data-ttu-id="80976-152">String collection</span><span class="sxs-lookup"><span data-stu-id="80976-152">String collection</span></span>| <span data-ttu-id="80976-153">角色定义授予的范围权限列表适用。</span><span class="sxs-lookup"><span data-stu-id="80976-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="80976-154">目前仅支持"/"。</span><span class="sxs-lookup"><span data-stu-id="80976-154">Currently only "/" is supported.</span></span> <span data-ttu-id="80976-155">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-155">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="80976-156">**请勿使用。这将很快被弃用。将作用域附加到角色分配**</span><span class="sxs-lookup"><span data-stu-id="80976-156">**DO NOT USE. This is going to be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="80976-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="80976-157">rolePermissions</span></span>|<span data-ttu-id="80976-158">[unifiedRolePermission](unifiedrolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80976-158">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="80976-159">角色中包含的权限列表。</span><span class="sxs-lookup"><span data-stu-id="80976-159">List of permissions included in the role.</span></span> <span data-ttu-id="80976-160">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-160">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="80976-161">必需。</span><span class="sxs-lookup"><span data-stu-id="80976-161">Required.</span></span> |
|<span data-ttu-id="80976-162">templateId</span><span class="sxs-lookup"><span data-stu-id="80976-162">templateId</span></span>|<span data-ttu-id="80976-163">String</span><span class="sxs-lookup"><span data-stu-id="80976-163">String</span></span>| <span data-ttu-id="80976-164">当 isBuiltIn 为 false 时可以设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="80976-164">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="80976-165">如果不同目录的标识符需要相同，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="80976-165">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="80976-166">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-166">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="80976-167">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="80976-167">inheritsPermissionsFrom</span></span>| <span data-ttu-id="80976-168">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80976-168">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="80976-169">给定角色定义继承自的角色定义的只读集合。</span><span class="sxs-lookup"><span data-stu-id="80976-169">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="80976-170">只有 Azure AD 内置角色支持此属性。</span><span class="sxs-lookup"><span data-stu-id="80976-170">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="80976-171">version</span><span class="sxs-lookup"><span data-stu-id="80976-171">version</span></span>|<span data-ttu-id="80976-172">String</span><span class="sxs-lookup"><span data-stu-id="80976-172">String</span></span>| <span data-ttu-id="80976-173">指示 unifiedRoleDefinition 的版本。</span><span class="sxs-lookup"><span data-stu-id="80976-173">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="80976-174">isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="80976-174">Read-only when isBuiltIn is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80976-175">关系</span><span class="sxs-lookup"><span data-stu-id="80976-175">Relationships</span></span>

<span data-ttu-id="80976-176">无</span><span class="sxs-lookup"><span data-stu-id="80976-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80976-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80976-177">JSON representation</span></span>

<span data-ttu-id="80976-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80976-178">The following is a JSON representation of the resource.</span></span>

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


