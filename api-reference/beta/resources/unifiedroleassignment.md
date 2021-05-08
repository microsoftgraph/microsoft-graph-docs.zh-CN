---
title: unifiedRoleAssignment 资源类型
description: 一角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c52e6bb05c9258680a36f04ad428c24a3a2829fc
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239959"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="0d5d6-103">unifiedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d5d6-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="0d5d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d5d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d5d6-105">unifiedRoleAssignment 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="0d5d6-106">它表示分配给主体的角色定义 (通常是用户) 作用域中的角色定义。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="0d5d6-107">需要提供 directoryScopeId 或 appScopeId。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="0d5d6-108">方法</span><span class="sxs-lookup"><span data-stu-id="0d5d6-108">Methods</span></span>

| <span data-ttu-id="0d5d6-109">方法</span><span class="sxs-lookup"><span data-stu-id="0d5d6-109">Method</span></span>       | <span data-ttu-id="0d5d6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d5d6-110">Return Type</span></span> | <span data-ttu-id="0d5d6-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d5d6-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0d5d6-112">列出 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-112">List unifiedRoleAssignment</span></span>](../api/rbacapplication-list-roleassignments.md) | [<span data-ttu-id="0d5d6-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="0d5d6-114">读取 unifiedRoleAssignment 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-114">Read a list of unifiedRoleAssignment objects and their properties.</span></span> |
| [<span data-ttu-id="0d5d6-115">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-115">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="0d5d6-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="0d5d6-117">读取 unifiedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-117">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="0d5d6-118">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-118">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="0d5d6-119">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-119">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="0d5d6-120">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-120">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="0d5d6-121">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0d5d6-121">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="0d5d6-122">无</span><span class="sxs-lookup"><span data-stu-id="0d5d6-122">None</span></span> | <span data-ttu-id="0d5d6-123">删除 unifiedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-123">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d5d6-124">属性</span><span class="sxs-lookup"><span data-stu-id="0d5d6-124">Properties</span></span>

| <span data-ttu-id="0d5d6-125">属性</span><span class="sxs-lookup"><span data-stu-id="0d5d6-125">Property</span></span>     | <span data-ttu-id="0d5d6-126">类型</span><span class="sxs-lookup"><span data-stu-id="0d5d6-126">Type</span></span>        | <span data-ttu-id="0d5d6-127">说明</span><span class="sxs-lookup"><span data-stu-id="0d5d6-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d5d6-128">id</span><span class="sxs-lookup"><span data-stu-id="0d5d6-128">id</span></span>|<span data-ttu-id="0d5d6-129">字符串</span><span class="sxs-lookup"><span data-stu-id="0d5d6-129">String</span></span>| <span data-ttu-id="0d5d6-130">unifiedRoleAssignment 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-130">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="0d5d6-131">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-131">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="0d5d6-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0d5d6-132">roleDefinitionId</span></span>|<span data-ttu-id="0d5d6-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0d5d6-133">String</span></span>| <span data-ttu-id="0d5d6-134">分配所针对的 unifiedRoleDefinition 的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-134">Identifier of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="0d5d6-135">只读。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-135">Read-only.</span></span> <span data-ttu-id="0d5d6-136">仅 `$filter` (`eq` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-136">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="0d5d6-137">principalId</span><span class="sxs-lookup"><span data-stu-id="0d5d6-137">principalId</span></span>|<span data-ttu-id="0d5d6-138">字符串</span><span class="sxs-lookup"><span data-stu-id="0d5d6-138">String</span></span>| <span data-ttu-id="0d5d6-139">分配授予的主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-139">Identifier of the principal to which the assignment is granted.</span></span> <span data-ttu-id="0d5d6-140">仅 `$filter` (`eq` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-140">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="0d5d6-141">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="0d5d6-141">directoryScopeId</span></span>|<span data-ttu-id="0d5d6-142">字符串</span><span class="sxs-lookup"><span data-stu-id="0d5d6-142">String</span></span>|<span data-ttu-id="0d5d6-143">表示工作分配范围的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-143">Identifier of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="0d5d6-144">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-144">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="0d5d6-145">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-145">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="0d5d6-146">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-146">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="0d5d6-147">appScopeId</span><span class="sxs-lookup"><span data-stu-id="0d5d6-147">appScopeId</span></span>|<span data-ttu-id="0d5d6-148">字符串</span><span class="sxs-lookup"><span data-stu-id="0d5d6-148">String</span></span>|<span data-ttu-id="0d5d6-149">当分配范围特定于应用时，特定于应用的范围的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-149">Identifier of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="0d5d6-150">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-150">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="0d5d6-151">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-151">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="0d5d6-152">用于 `/` 租户范围范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-152">Use `/` for tenant-wide scope.</span></span> <span data-ttu-id="0d5d6-153">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-153">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="0d5d6-154">resourceScope</span><span class="sxs-lookup"><span data-stu-id="0d5d6-154">resourceScope</span></span>|<span data-ttu-id="0d5d6-155">字符串</span><span class="sxs-lookup"><span data-stu-id="0d5d6-155">String</span></span>| <span data-ttu-id="0d5d6-156">unifiedRoleAssignment 适用的范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-156">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="0d5d6-157">这 `/` 适用于服务范围。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-157">This is `/` for service-wide.</span></span> <span data-ttu-id="0d5d6-158">**请勿使用。此属性将很快弃用。**</span><span class="sxs-lookup"><span data-stu-id="0d5d6-158">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d5d6-159">关系</span><span class="sxs-lookup"><span data-stu-id="0d5d6-159">Relationships</span></span>

| <span data-ttu-id="0d5d6-160">关系</span><span class="sxs-lookup"><span data-stu-id="0d5d6-160">Relationship</span></span> | <span data-ttu-id="0d5d6-161">类型</span><span class="sxs-lookup"><span data-stu-id="0d5d6-161">Type</span></span>   |<span data-ttu-id="0d5d6-162">说明</span><span class="sxs-lookup"><span data-stu-id="0d5d6-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d5d6-163">appScope</span><span class="sxs-lookup"><span data-stu-id="0d5d6-163">appScope</span></span>|[<span data-ttu-id="0d5d6-164">appScope</span><span class="sxs-lookup"><span data-stu-id="0d5d6-164">appScope</span></span>](appscope.md)|<span data-ttu-id="0d5d6-165">当分配范围特定于应用时，应用特定范围的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-165">Details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="0d5d6-166">包含实体。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-166">Containment entity.</span></span> |
|<span data-ttu-id="0d5d6-167">directoryScope</span><span class="sxs-lookup"><span data-stu-id="0d5d6-167">directoryScope</span></span>|[<span data-ttu-id="0d5d6-168">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0d5d6-168">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="0d5d6-169">分配范围的目录对象。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-169">The directory object that is the scope of the assignment.</span></span> <span data-ttu-id="0d5d6-170">提供，以便调用方可以在获取目录对象的同时使用 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-170">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="0d5d6-171">只读。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-171">Read-only.</span></span> <span data-ttu-id="0d5d6-172">支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-172">Supports `$expand`.</span></span> |
|<span data-ttu-id="0d5d6-173">principal</span><span class="sxs-lookup"><span data-stu-id="0d5d6-173">principal</span></span>|[<span data-ttu-id="0d5d6-174">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0d5d6-174">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0d5d6-175">分配的主体。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-175">The assigned principal.</span></span> <span data-ttu-id="0d5d6-176">提供此权限，以便调用方可以使用 与获取 角色分配 同时 `$expand` 使用。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-176">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="0d5d6-177">只读。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-177">Read-only.</span></span> <span data-ttu-id="0d5d6-178">支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-178">Supports `$expand`.</span></span> |
|<span data-ttu-id="0d5d6-179">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="0d5d6-179">roleDefinition</span></span>|[<span data-ttu-id="0d5d6-180">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0d5d6-180">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="0d5d6-181">分配用于的 roleDefinition。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-181">The roleDefinition the assignment is for.</span></span> <span data-ttu-id="0d5d6-182">提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-182">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="0d5d6-183">**roleDefinition.id** 自动展开。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-183">**roleDefinition.id** will be auto expanded.</span></span> <span data-ttu-id="0d5d6-184">支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-184">Supports `$expand`.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="0d5d6-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d5d6-185">JSON representation</span></span>

<span data-ttu-id="0d5d6-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d5d6-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalId": "String",
  "principal": {"@odata.type": "microsoft.graph.directoryObject"},
  "directoryScopeId": "String",
  "directoryScope": {"@odata.type": "microsoft.graph.directoryObject"},
  "appScopeId": "String",
  "appScope": {"@odata.type": "microsoft.graph.appScope"},
  "resourceScope": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

