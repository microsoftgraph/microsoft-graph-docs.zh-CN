---
title: unifiedRoleDefinition 资源类型
description: 统一角色定义是权限的集合
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd26a0526327c4b630f52fd80d5a75b4df9430c7
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218021"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="1b1f7-103">unifiedRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b1f7-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="1b1f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b1f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b1f7-105">UnifiedRoleDefinition 是列出可执行的操作（如读取、写入和删除）的权限的集合。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-105">A unifiedRoleDefinition is a collection of permissions listing the operations that can be performed, such as read, write, and delete.</span></span>

## <a name="methods"></a><span data-ttu-id="1b1f7-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1b1f7-106">Methods</span></span>

| <span data-ttu-id="1b1f7-107">方法</span><span class="sxs-lookup"><span data-stu-id="1b1f7-107">Method</span></span>       | <span data-ttu-id="1b1f7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b1f7-108">Return Type</span></span> | <span data-ttu-id="1b1f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b1f7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1b1f7-110">列出 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-110">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="1b1f7-111">[unifiedRoleDefinition](unifiedroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b1f7-111">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="1b1f7-112">读取 unifiedRoleDefinition 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-112">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="1b1f7-113">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-113">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="1b1f7-114">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-114">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="1b1f7-115">读取 unifiedRoleDefinition 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-115">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="1b1f7-116">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-116">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="1b1f7-117">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-117">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="1b1f7-118">创建 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-118">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="1b1f7-119">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-119">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="1b1f7-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="1b1f7-121">更新 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-121">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="1b1f7-122">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b1f7-122">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="1b1f7-123">无</span><span class="sxs-lookup"><span data-stu-id="1b1f7-123">None</span></span> | <span data-ttu-id="1b1f7-124">删除 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-124">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b1f7-125">属性</span><span class="sxs-lookup"><span data-stu-id="1b1f7-125">Properties</span></span>

| <span data-ttu-id="1b1f7-126">属性</span><span class="sxs-lookup"><span data-stu-id="1b1f7-126">Property</span></span>     | <span data-ttu-id="1b1f7-127">类型</span><span class="sxs-lookup"><span data-stu-id="1b1f7-127">Type</span></span>        | <span data-ttu-id="1b1f7-128">说明</span><span class="sxs-lookup"><span data-stu-id="1b1f7-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b1f7-129">说明</span><span class="sxs-lookup"><span data-stu-id="1b1f7-129">description</span></span>|<span data-ttu-id="1b1f7-130">String</span><span class="sxs-lookup"><span data-stu-id="1b1f7-130">String</span></span>| <span data-ttu-id="1b1f7-131">UnifiedRoleDefinition 的说明。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-131">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="1b1f7-132">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="1b1f7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1b1f7-133">displayName</span></span>|<span data-ttu-id="1b1f7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1b1f7-134">String</span></span>| <span data-ttu-id="1b1f7-135">UnifiedRoleDefinition 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-135">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="1b1f7-136">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="1b1f7-137">必需。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-137">Required.</span></span>|
|<span data-ttu-id="1b1f7-138">id</span><span class="sxs-lookup"><span data-stu-id="1b1f7-138">id</span></span>|<span data-ttu-id="1b1f7-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1b1f7-139">String</span></span>| <span data-ttu-id="1b1f7-140">UnifiedRoleDefinition 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-140">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="1b1f7-141">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="1b1f7-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="1b1f7-142">isBuiltIn</span></span>|<span data-ttu-id="1b1f7-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="1b1f7-143">Boolean</span></span>| <span data-ttu-id="1b1f7-144">指示 unifiedRoleDefinition 是否是产品或自定义的默认设置的一部分的标志。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-144">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="1b1f7-145">只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-145">Read-only.</span></span> |
|<span data-ttu-id="1b1f7-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1b1f7-146">isEnabled</span></span>|<span data-ttu-id="1b1f7-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b1f7-147">Boolean</span></span>| <span data-ttu-id="1b1f7-148">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="1b1f7-149">如果为 false，则该角色不可用于分配。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="1b1f7-150">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="1b1f7-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1b1f7-151">resourceScopes</span></span>|<span data-ttu-id="1b1f7-152">String collection</span><span class="sxs-lookup"><span data-stu-id="1b1f7-152">String collection</span></span>| <span data-ttu-id="1b1f7-153">由角色定义授予的范围权限列表应用于。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="1b1f7-154">目前仅支持 "/"。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-154">Currently only "/" is supported.</span></span> <span data-ttu-id="1b1f7-155">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-155">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="1b1f7-156">**请勿使用。即将弃用此建议。将作用域附加到角色分配**</span><span class="sxs-lookup"><span data-stu-id="1b1f7-156">**DO NOT USE. This is going to be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="1b1f7-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="1b1f7-157">rolePermissions</span></span>|<span data-ttu-id="1b1f7-158">[unifiedRolePermission](unifiedrolepermission.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b1f7-158">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="1b1f7-159">角色中包含的权限的列表。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-159">List of permissions included in the role.</span></span> <span data-ttu-id="1b1f7-160">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-160">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="1b1f7-161">必需。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-161">Required.</span></span> |
|<span data-ttu-id="1b1f7-162">templateId</span><span class="sxs-lookup"><span data-stu-id="1b1f7-162">templateId</span></span>|<span data-ttu-id="1b1f7-163">字符串</span><span class="sxs-lookup"><span data-stu-id="1b1f7-163">String</span></span>| <span data-ttu-id="1b1f7-164">当 isBuiltIn 为 false 时可设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-164">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="1b1f7-165">如果一个要求标识符在不同目录中是相同的，则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-165">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="1b1f7-166">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-166">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="1b1f7-167">version</span><span class="sxs-lookup"><span data-stu-id="1b1f7-167">version</span></span>|<span data-ttu-id="1b1f7-168">String</span><span class="sxs-lookup"><span data-stu-id="1b1f7-168">String</span></span>| <span data-ttu-id="1b1f7-169">指示 unifiedRoleDefinition 的版本。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-169">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="1b1f7-170">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-170">Read-only when isBuiltIn is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b1f7-171">关系</span><span class="sxs-lookup"><span data-stu-id="1b1f7-171">Relationships</span></span>

<span data-ttu-id="1b1f7-172">无</span><span class="sxs-lookup"><span data-stu-id="1b1f7-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b1f7-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b1f7-173">JSON representation</span></span>

<span data-ttu-id="1b1f7-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b1f7-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "baseType": "",
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