---
title: unifiedRoleAssignmentMultiple 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: eb763490e9d60ca386400eef3dae1b9e2d382d21
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038662"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="d6e22-103">unifiedRoleAssignmentMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6e22-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="d6e22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6e22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e22-105">UnifiedRoleAssignmentMultiple 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d6e22-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="d6e22-106">它表示分配给范围数组的主体（通常为用户）数组的角色定义。</span><span class="sxs-lookup"><span data-stu-id="d6e22-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="d6e22-107">此类 RBAC 提供程序的一个示例是 Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="d6e22-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="d6e22-108">在 Microsoft Intune 中，可以创建具有多个主体和多个作用域的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d6e22-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="d6e22-109">提供 " **directoryScopeIds** " 或 " **appScopeIds** " 是必需的。</span><span class="sxs-lookup"><span data-stu-id="d6e22-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="d6e22-110">方法</span><span class="sxs-lookup"><span data-stu-id="d6e22-110">Methods</span></span>

| <span data-ttu-id="d6e22-111">方法</span><span class="sxs-lookup"><span data-stu-id="d6e22-111">Method</span></span>       | <span data-ttu-id="d6e22-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6e22-112">Return Type</span></span> | <span data-ttu-id="d6e22-113">说明</span><span class="sxs-lookup"><span data-stu-id="d6e22-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d6e22-114">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="d6e22-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="d6e22-116">读取 unifiedRoleAssignmentMultiple 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6e22-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="d6e22-117">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="d6e22-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="d6e22-119">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="d6e22-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="d6e22-120">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="d6e22-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="d6e22-122">更新现有的 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="d6e22-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="d6e22-123">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d6e22-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="d6e22-124">无</span><span class="sxs-lookup"><span data-stu-id="d6e22-124">None</span></span> | <span data-ttu-id="d6e22-125">删除 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="d6e22-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d6e22-126">属性</span><span class="sxs-lookup"><span data-stu-id="d6e22-126">Properties</span></span>

| <span data-ttu-id="d6e22-127">属性</span><span class="sxs-lookup"><span data-stu-id="d6e22-127">Property</span></span>     | <span data-ttu-id="d6e22-128">类型</span><span class="sxs-lookup"><span data-stu-id="d6e22-128">Type</span></span>        | <span data-ttu-id="d6e22-129">说明</span><span class="sxs-lookup"><span data-stu-id="d6e22-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d6e22-130">id</span><span class="sxs-lookup"><span data-stu-id="d6e22-130">id</span></span> | <span data-ttu-id="d6e22-131">字符串</span><span class="sxs-lookup"><span data-stu-id="d6e22-131">String</span></span> | <span data-ttu-id="d6e22-132">UnifiedRoleAssignmentMultiple 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d6e22-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="d6e22-133">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="d6e22-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="d6e22-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d6e22-134">displayName</span></span> | <span data-ttu-id="d6e22-135">String</span><span class="sxs-lookup"><span data-stu-id="d6e22-135">String</span></span> | <span data-ttu-id="d6e22-136">角色分配的名称。</span><span class="sxs-lookup"><span data-stu-id="d6e22-136">Name of the role assignment.</span></span> <span data-ttu-id="d6e22-137">必需。</span><span class="sxs-lookup"><span data-stu-id="d6e22-137">Required.</span></span> |
| <span data-ttu-id="d6e22-138">description</span><span class="sxs-lookup"><span data-stu-id="d6e22-138">description</span></span> | <span data-ttu-id="d6e22-139">String</span><span class="sxs-lookup"><span data-stu-id="d6e22-139">String</span></span> | <span data-ttu-id="d6e22-140">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="d6e22-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="d6e22-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d6e22-141">roleDefinitionId</span></span> | <span data-ttu-id="d6e22-142">String</span><span class="sxs-lookup"><span data-stu-id="d6e22-142">String</span></span> | <span data-ttu-id="d6e22-143">工作分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="d6e22-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="d6e22-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d6e22-144">roleDefinition</span></span> | [<span data-ttu-id="d6e22-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d6e22-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="d6e22-146">指示工作分配所针对的 roleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="d6e22-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="d6e22-147">提供，以便呼叫者可以在获取角色分配的同时使用该角色定义 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="d6e22-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="d6e22-148">只读。</span><span class="sxs-lookup"><span data-stu-id="d6e22-148">Read-only.</span></span>  |
| <span data-ttu-id="d6e22-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="d6e22-149">principalIds</span></span> | <span data-ttu-id="d6e22-150">String collection</span><span class="sxs-lookup"><span data-stu-id="d6e22-150">String collection</span></span> | <span data-ttu-id="d6e22-151">向其授予分配的主体的 Objectids。</span><span class="sxs-lookup"><span data-stu-id="d6e22-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="d6e22-152">原理</span><span class="sxs-lookup"><span data-stu-id="d6e22-152">principals</span></span>| <span data-ttu-id="d6e22-153">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6e22-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d6e22-154">引用所分配的主体的只读集合。</span><span class="sxs-lookup"><span data-stu-id="d6e22-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="d6e22-155">提供，以便呼叫者可以在获取角色分配的同时使用这些承担者 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="d6e22-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="d6e22-156">只读。</span><span class="sxs-lookup"><span data-stu-id="d6e22-156">Read-only.</span></span> |
| <span data-ttu-id="d6e22-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="d6e22-157">directoryScopeIds</span></span> | <span data-ttu-id="d6e22-158">String collection</span><span class="sxs-lookup"><span data-stu-id="d6e22-158">String collection</span></span> | <span data-ttu-id="d6e22-159">表示工作分配范围的目录对象的 id。</span><span class="sxs-lookup"><span data-stu-id="d6e22-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="d6e22-160">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="d6e22-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="d6e22-161">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="d6e22-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="d6e22-162">应用范围是此应用程序仅定义和理解的作用域。</span><span class="sxs-lookup"><span data-stu-id="d6e22-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="d6e22-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="d6e22-163">directoryScopes</span></span> | <span data-ttu-id="d6e22-164">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6e22-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d6e22-165">只读集合，引用属于分配范围的目录对象。</span><span class="sxs-lookup"><span data-stu-id="d6e22-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="d6e22-166">提供，以便呼叫者可以使用 `$expand` 与获取角色分配相同的时间获取目录对象。</span><span class="sxs-lookup"><span data-stu-id="d6e22-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="d6e22-167">只读。</span><span class="sxs-lookup"><span data-stu-id="d6e22-167">Read-only.</span></span> |
| <span data-ttu-id="d6e22-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="d6e22-168">appScopeIds</span></span> | <span data-ttu-id="d6e22-169">String collection</span><span class="sxs-lookup"><span data-stu-id="d6e22-169">String collection</span></span> | <span data-ttu-id="d6e22-170">当分配作用域是特定于应用的应用程序特定作用域的 id。</span><span class="sxs-lookup"><span data-stu-id="d6e22-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="d6e22-171">工作分配的范围决定了主体已被授予访问权限的一组资源。</span><span class="sxs-lookup"><span data-stu-id="d6e22-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="d6e22-172">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="d6e22-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="d6e22-173">对租户范围范围使用 "/"。</span><span class="sxs-lookup"><span data-stu-id="d6e22-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="d6e22-174">应用范围是此应用程序仅定义和理解的作用域。</span><span class="sxs-lookup"><span data-stu-id="d6e22-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="d6e22-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="d6e22-175">appScopes</span></span> | <span data-ttu-id="d6e22-176">[appScope](appscope.md)集合</span><span class="sxs-lookup"><span data-stu-id="d6e22-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="d6e22-177">只读集合，其中包含应用程序特定作用域的详细信息，当分配作用域为应用程序特定时。</span><span class="sxs-lookup"><span data-stu-id="d6e22-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="d6e22-178">包容实体。</span><span class="sxs-lookup"><span data-stu-id="d6e22-178">Containment entity.</span></span> <span data-ttu-id="d6e22-179">只读。</span><span class="sxs-lookup"><span data-stu-id="d6e22-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="d6e22-180">关系</span><span class="sxs-lookup"><span data-stu-id="d6e22-180">Relationships</span></span>

<span data-ttu-id="d6e22-181">无</span><span class="sxs-lookup"><span data-stu-id="d6e22-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6e22-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6e22-182">JSON representation</span></span>

<span data-ttu-id="d6e22-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6e22-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "",
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
