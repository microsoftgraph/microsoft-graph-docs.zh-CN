---
title: unifiedRoleDefinition 资源类型
description: 统一角色定义是权限的集合
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: be1b8a0b1a623c6cf322d5cf7997f04b87875c51
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437746"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="73c84-103">unifiedRoleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="73c84-103">unifiedRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73c84-104">UnifiedRoleDefinition 是列出可执行的操作 (如读取、写入和删除) 的权限的集合。</span><span class="sxs-lookup"><span data-stu-id="73c84-104">A unifiedRoleDefinition is a collection of permissions listing the operations that can be performed, such as read, write, and delete.</span></span>

## <a name="methods"></a><span data-ttu-id="73c84-105">方法</span><span class="sxs-lookup"><span data-stu-id="73c84-105">Methods</span></span>

| <span data-ttu-id="73c84-106">方法</span><span class="sxs-lookup"><span data-stu-id="73c84-106">Method</span></span>       | <span data-ttu-id="73c84-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="73c84-107">Return Type</span></span> | <span data-ttu-id="73c84-108">说明</span><span class="sxs-lookup"><span data-stu-id="73c84-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="73c84-109">列出 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-109">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="73c84-110">[unifiedRoleDefinition](unifiedroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="73c84-110">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="73c84-111">读取 unifiedRoleDefinition 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="73c84-111">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="73c84-112">获取 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-112">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="73c84-113">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-113">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="73c84-114">读取 unifiedRoleDefinition 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73c84-114">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="73c84-115">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-115">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="73c84-116">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-116">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="73c84-117">创建 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="73c84-117">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="73c84-118">更新 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-118">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="73c84-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="73c84-120">更新 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="73c84-120">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="73c84-121">删除 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73c84-121">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="73c84-122">无</span><span class="sxs-lookup"><span data-stu-id="73c84-122">None</span></span> | <span data-ttu-id="73c84-123">删除 unifiedRoleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="73c84-123">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="73c84-124">属性</span><span class="sxs-lookup"><span data-stu-id="73c84-124">Properties</span></span>

| <span data-ttu-id="73c84-125">属性</span><span class="sxs-lookup"><span data-stu-id="73c84-125">Property</span></span>     | <span data-ttu-id="73c84-126">类型</span><span class="sxs-lookup"><span data-stu-id="73c84-126">Type</span></span>        | <span data-ttu-id="73c84-127">说明</span><span class="sxs-lookup"><span data-stu-id="73c84-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73c84-128">说明</span><span class="sxs-lookup"><span data-stu-id="73c84-128">description</span></span>|<span data-ttu-id="73c84-129">String</span><span class="sxs-lookup"><span data-stu-id="73c84-129">String</span></span>| <span data-ttu-id="73c84-130">UnifiedRoleDefinition 的说明。</span><span class="sxs-lookup"><span data-stu-id="73c84-130">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="73c84-131">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-131">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="73c84-132">displayName</span><span class="sxs-lookup"><span data-stu-id="73c84-132">displayName</span></span>|<span data-ttu-id="73c84-133">字符串</span><span class="sxs-lookup"><span data-stu-id="73c84-133">String</span></span>| <span data-ttu-id="73c84-134">UnifiedRoleDefinition 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="73c84-134">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="73c84-135">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-135">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="73c84-136">必需。</span><span class="sxs-lookup"><span data-stu-id="73c84-136">Required.</span></span>|
|<span data-ttu-id="73c84-137">id</span><span class="sxs-lookup"><span data-stu-id="73c84-137">id</span></span>|<span data-ttu-id="73c84-138">字符串</span><span class="sxs-lookup"><span data-stu-id="73c84-138">String</span></span>| <span data-ttu-id="73c84-139">UnifiedRoleDefinition 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="73c84-139">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="73c84-140">键, 不可为 null, 只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-140">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="73c84-141">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="73c84-141">isBuiltIn</span></span>|<span data-ttu-id="73c84-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="73c84-142">Boolean</span></span>| <span data-ttu-id="73c84-143">指示 unifiedRoleDefinition 是否是产品或自定义的默认设置的一部分的标志。</span><span class="sxs-lookup"><span data-stu-id="73c84-143">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="73c84-144">只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-144">Read-only.</span></span> |
|<span data-ttu-id="73c84-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="73c84-145">isEnabled</span></span>|<span data-ttu-id="73c84-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="73c84-146">Boolean</span></span>| <span data-ttu-id="73c84-147">指示角色是否已启用分配的标志。</span><span class="sxs-lookup"><span data-stu-id="73c84-147">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="73c84-148">如果为 false, 则该角色不可用于分配。</span><span class="sxs-lookup"><span data-stu-id="73c84-148">If false the role is not available for assignment.</span></span> <span data-ttu-id="73c84-149">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-149">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="73c84-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="73c84-150">resourceScopes</span></span>|<span data-ttu-id="73c84-151">String collection</span><span class="sxs-lookup"><span data-stu-id="73c84-151">String collection</span></span>| <span data-ttu-id="73c84-152">由角色定义授予的范围权限列表应用于。</span><span class="sxs-lookup"><span data-stu-id="73c84-152">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="73c84-153">目前仅支持 "/"。</span><span class="sxs-lookup"><span data-stu-id="73c84-153">Currently only "/" is supported.</span></span> <span data-ttu-id="73c84-154">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-154">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="73c84-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="73c84-155">rolePermissions</span></span>|<span data-ttu-id="73c84-156">[unifiedRolePermission](unifiedrolepermission.md)集合</span><span class="sxs-lookup"><span data-stu-id="73c84-156">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="73c84-157">角色中包含的权限的列表。</span><span class="sxs-lookup"><span data-stu-id="73c84-157">List of permissions included in the role.</span></span> <span data-ttu-id="73c84-158">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-158">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="73c84-159">必需。</span><span class="sxs-lookup"><span data-stu-id="73c84-159">Required.</span></span> |
|<span data-ttu-id="73c84-160">templateId</span><span class="sxs-lookup"><span data-stu-id="73c84-160">templateId</span></span>|<span data-ttu-id="73c84-161">String</span><span class="sxs-lookup"><span data-stu-id="73c84-161">String</span></span>| <span data-ttu-id="73c84-162">当 isBuiltIn 为 false 时可设置的自定义模板标识符。</span><span class="sxs-lookup"><span data-stu-id="73c84-162">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="73c84-163">如果一个要求标识符在不同目录中是相同的, 则通常使用此标识符。</span><span class="sxs-lookup"><span data-stu-id="73c84-163">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="73c84-164">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-164">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="73c84-165">version</span><span class="sxs-lookup"><span data-stu-id="73c84-165">version</span></span>|<span data-ttu-id="73c84-166">String</span><span class="sxs-lookup"><span data-stu-id="73c84-166">String</span></span>| <span data-ttu-id="73c84-167">指示 unifiedRoleDefinition 的版本。</span><span class="sxs-lookup"><span data-stu-id="73c84-167">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="73c84-168">当 isBuiltIn 为 true 时为只读。</span><span class="sxs-lookup"><span data-stu-id="73c84-168">Read-only when isBuiltIn is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73c84-169">关系</span><span class="sxs-lookup"><span data-stu-id="73c84-169">Relationships</span></span>

<span data-ttu-id="73c84-170">无</span><span class="sxs-lookup"><span data-stu-id="73c84-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73c84-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73c84-171">JSON representation</span></span>

<span data-ttu-id="73c84-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73c84-172">The following is a JSON representation of the resource.</span></span>

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
