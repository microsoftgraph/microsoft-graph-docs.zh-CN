---
title: unifiedRoleAssignmentMultiple 资源类型
description: 分配给主体数组的角色定义 (通常是用户) 一组主体。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b6f345dbf4947212f22a5386fded551d62b0e24d
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241056"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="1fceb-103">unifiedRoleAssignmentMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fceb-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="1fceb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fceb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fceb-105">unifiedRoleAssignmentMultiple 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="1fceb-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="1fceb-106">它表示分配给主体数组的角色定义 (通常是用户通过) 组进行分配。</span><span class="sxs-lookup"><span data-stu-id="1fceb-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="1fceb-107">此类 RBAC 提供程序的一个示例是Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="1fceb-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="1fceb-108">在Microsoft Intune中，可以创建具有角色分配和多个作用域的组。</span><span class="sxs-lookup"><span data-stu-id="1fceb-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="1fceb-109">需要 **提供 directoryScopeIds** 或 **appScopeIds。**</span><span class="sxs-lookup"><span data-stu-id="1fceb-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="1fceb-110">方法</span><span class="sxs-lookup"><span data-stu-id="1fceb-110">Methods</span></span>

| <span data-ttu-id="1fceb-111">方法</span><span class="sxs-lookup"><span data-stu-id="1fceb-111">Method</span></span>       | <span data-ttu-id="1fceb-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1fceb-112">Return Type</span></span> | <span data-ttu-id="1fceb-113">说明</span><span class="sxs-lookup"><span data-stu-id="1fceb-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1fceb-114">列出 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-114">List unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | [<span data-ttu-id="1fceb-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="1fceb-116">读取 unifiedRoleAssignmentMultiple 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="1fceb-116">Read a list of unifiedRoleAssignmentMultiple objects and their properties.</span></span> |
| [<span data-ttu-id="1fceb-117">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-117">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="1fceb-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="1fceb-119">读取 unifiedRoleAssignmentMultiple 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fceb-119">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="1fceb-120">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-120">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="1fceb-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="1fceb-122">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="1fceb-122">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="1fceb-123">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-123">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="1fceb-124">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-124">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="1fceb-125">更新现有的 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="1fceb-125">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="1fceb-126">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="1fceb-126">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="1fceb-127">无</span><span class="sxs-lookup"><span data-stu-id="1fceb-127">None</span></span> | <span data-ttu-id="1fceb-128">删除 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="1fceb-128">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1fceb-129">属性</span><span class="sxs-lookup"><span data-stu-id="1fceb-129">Properties</span></span>

| <span data-ttu-id="1fceb-130">属性</span><span class="sxs-lookup"><span data-stu-id="1fceb-130">Property</span></span>     | <span data-ttu-id="1fceb-131">类型</span><span class="sxs-lookup"><span data-stu-id="1fceb-131">Type</span></span>        | <span data-ttu-id="1fceb-132">说明</span><span class="sxs-lookup"><span data-stu-id="1fceb-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1fceb-133">id</span><span class="sxs-lookup"><span data-stu-id="1fceb-133">id</span></span> | <span data-ttu-id="1fceb-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1fceb-134">String</span></span> | <span data-ttu-id="1fceb-135">unifiedRoleAssignmentMultiple 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1fceb-135">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="1fceb-136">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="1fceb-136">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="1fceb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1fceb-137">displayName</span></span> | <span data-ttu-id="1fceb-138">字符串</span><span class="sxs-lookup"><span data-stu-id="1fceb-138">String</span></span> | <span data-ttu-id="1fceb-139">域名角色分配。</span><span class="sxs-lookup"><span data-stu-id="1fceb-139">Name of the role assignment.</span></span> <span data-ttu-id="1fceb-140">必需。</span><span class="sxs-lookup"><span data-stu-id="1fceb-140">Required.</span></span> |
| <span data-ttu-id="1fceb-141">description</span><span class="sxs-lookup"><span data-stu-id="1fceb-141">description</span></span> | <span data-ttu-id="1fceb-142">字符串</span><span class="sxs-lookup"><span data-stu-id="1fceb-142">String</span></span> | <span data-ttu-id="1fceb-143">项目说明角色分配。</span><span class="sxs-lookup"><span data-stu-id="1fceb-143">Description of the role assignment.</span></span> |
| <span data-ttu-id="1fceb-144">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1fceb-144">roleDefinitionId</span></span> | <span data-ttu-id="1fceb-145">字符串</span><span class="sxs-lookup"><span data-stu-id="1fceb-145">String</span></span> | <span data-ttu-id="1fceb-146">分配所针对的 unifiedRoleDefinition 的标识符。</span><span class="sxs-lookup"><span data-stu-id="1fceb-146">Identifier of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="1fceb-147">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1fceb-147">roleDefinition</span></span> | [<span data-ttu-id="1fceb-148">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1fceb-148">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="1fceb-149">指示分配所针对的 roleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="1fceb-149">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="1fceb-150">提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="1fceb-150">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="1fceb-151">只读。</span><span class="sxs-lookup"><span data-stu-id="1fceb-151">Read-only.</span></span> <span data-ttu-id="1fceb-152">支持 `$filter` (`eq` **id** **、isBuiltIn** 和 **displayName** 上的 `startsWith` **displayName** 和) `$expand` 运算符。</span><span class="sxs-lookup"><span data-stu-id="1fceb-152">Supports `$filter` (`eq` operator on **id**, **isBuiltIn**, and **displayName**, and `startsWith` operator on **displayName**)  and `$expand`.</span></span>  |
| <span data-ttu-id="1fceb-153">principalIds</span><span class="sxs-lookup"><span data-stu-id="1fceb-153">principalIds</span></span> | <span data-ttu-id="1fceb-154">String collection</span><span class="sxs-lookup"><span data-stu-id="1fceb-154">String collection</span></span> | <span data-ttu-id="1fceb-155">分配授予的主体的标识符。</span><span class="sxs-lookup"><span data-stu-id="1fceb-155">Identifiers of the principals to which the assignment is granted.</span></span>  <span data-ttu-id="1fceb-156">仅 `$filter` (`any` 运算符) 。</span><span class="sxs-lookup"><span data-stu-id="1fceb-156">Supports `$filter` (`any` operator only).</span></span> |
| <span data-ttu-id="1fceb-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="1fceb-157">directoryScopeIds</span></span> | <span data-ttu-id="1fceb-158">String collection</span><span class="sxs-lookup"><span data-stu-id="1fceb-158">String collection</span></span> | <span data-ttu-id="1fceb-159">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="1fceb-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="1fceb-160">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="1fceb-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="1fceb-161">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="1fceb-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="1fceb-162">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="1fceb-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="1fceb-163">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="1fceb-163">appScopeIds</span></span> | <span data-ttu-id="1fceb-164">String collection</span><span class="sxs-lookup"><span data-stu-id="1fceb-164">String collection</span></span> | <span data-ttu-id="1fceb-165">当分配范围特定于应用时，特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="1fceb-165">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="1fceb-166">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="1fceb-166">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="1fceb-167">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="1fceb-167">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="1fceb-168">用于 `/` 租户范围范围。</span><span class="sxs-lookup"><span data-stu-id="1fceb-168">Use `/` for tenant-wide scope.</span></span> <span data-ttu-id="1fceb-169">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="1fceb-169">App scopes are scopes that are defined and understood by this application only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1fceb-170">关系</span><span class="sxs-lookup"><span data-stu-id="1fceb-170">Relationships</span></span>

| <span data-ttu-id="1fceb-171">关系</span><span class="sxs-lookup"><span data-stu-id="1fceb-171">Relationship</span></span> | <span data-ttu-id="1fceb-172">类型</span><span class="sxs-lookup"><span data-stu-id="1fceb-172">Type</span></span>   |<span data-ttu-id="1fceb-173">说明</span><span class="sxs-lookup"><span data-stu-id="1fceb-173">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fceb-174">appScopes</span><span class="sxs-lookup"><span data-stu-id="1fceb-174">appScopes</span></span> | <span data-ttu-id="1fceb-175">[appScope](appscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fceb-175">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="1fceb-176">当分配范围特定于应用时，具有特定于应用的范围的详细信息的只读集合。</span><span class="sxs-lookup"><span data-stu-id="1fceb-176">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="1fceb-177">包含实体。</span><span class="sxs-lookup"><span data-stu-id="1fceb-177">Containment entity.</span></span> <span data-ttu-id="1fceb-178">只读。</span><span class="sxs-lookup"><span data-stu-id="1fceb-178">Read-only.</span></span>  |
| <span data-ttu-id="1fceb-179">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="1fceb-179">directoryScopes</span></span> | <span data-ttu-id="1fceb-180">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1fceb-180">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="1fceb-181">引用作为分配范围的目录对象的只读集合。</span><span class="sxs-lookup"><span data-stu-id="1fceb-181">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="1fceb-182">提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="1fceb-182">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="1fceb-183">只读。</span><span class="sxs-lookup"><span data-stu-id="1fceb-183">Read-only.</span></span>  <span data-ttu-id="1fceb-184">支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="1fceb-184">Supports `$expand`.</span></span>|
| <span data-ttu-id="1fceb-185">principals</span><span class="sxs-lookup"><span data-stu-id="1fceb-185">principals</span></span>| <span data-ttu-id="1fceb-186">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1fceb-186">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="1fceb-187">引用分配的主体的只读集合。</span><span class="sxs-lookup"><span data-stu-id="1fceb-187">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="1fceb-188">提供此权限，以便调用方可以使用 与获取 角色分配 `$expand` 同时使用。</span><span class="sxs-lookup"><span data-stu-id="1fceb-188">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="1fceb-189">只读。</span><span class="sxs-lookup"><span data-stu-id="1fceb-189">Read-only.</span></span>  <span data-ttu-id="1fceb-190">支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="1fceb-190">Supports `$expand`.</span></span>|
|<span data-ttu-id="1fceb-191">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1fceb-191">roleDefinition</span></span>|[<span data-ttu-id="1fceb-192">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1fceb-192">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="1fceb-193">分配用于的 roleDefinition。</span><span class="sxs-lookup"><span data-stu-id="1fceb-193">The roleDefinition the assignment is for.</span></span> <span data-ttu-id="1fceb-194">提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="1fceb-194">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="1fceb-195">**roleDefinition.id** 自动展开。</span><span class="sxs-lookup"><span data-stu-id="1fceb-195">**roleDefinition.id** will be auto expanded.</span></span> <span data-ttu-id="1fceb-196">支持 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="1fceb-196">Supports `$expand`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1fceb-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fceb-197">JSON representation</span></span>

<span data-ttu-id="1fceb-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fceb-198">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


