---
title: unifiedRoleAssignmentMultiple 资源类型
description: 一角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4df17c6b112cefe03a12631ee763f49e976fb568
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159841"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="3b81e-103">unifiedRoleAssignmentMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b81e-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="3b81e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b81e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b81e-105">unifiedRoleAssignmentMultiple 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="3b81e-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="3b81e-106">它表示分配给主体数组的角色定义 (通常是用户) 一组作用域。</span><span class="sxs-lookup"><span data-stu-id="3b81e-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="3b81e-107">Microsoft Intune 就是此类 RBAC 提供程序的一个示例。</span><span class="sxs-lookup"><span data-stu-id="3b81e-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="3b81e-108">在 Microsoft Intune 中，你可以创建一角色分配多个主体和多个作用域。</span><span class="sxs-lookup"><span data-stu-id="3b81e-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="3b81e-109">提供 **directoryScopeIds** 或 **appScopeIds 是必需的** 。</span><span class="sxs-lookup"><span data-stu-id="3b81e-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="3b81e-110">方法</span><span class="sxs-lookup"><span data-stu-id="3b81e-110">Methods</span></span>

| <span data-ttu-id="3b81e-111">方法</span><span class="sxs-lookup"><span data-stu-id="3b81e-111">Method</span></span>       | <span data-ttu-id="3b81e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b81e-112">Return Type</span></span> | <span data-ttu-id="3b81e-113">说明</span><span class="sxs-lookup"><span data-stu-id="3b81e-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3b81e-114">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="3b81e-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3b81e-116">读取 unifiedRoleAssignmentMultiple 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b81e-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="3b81e-117">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="3b81e-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3b81e-119">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="3b81e-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="3b81e-120">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="3b81e-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3b81e-122">更新现有的 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="3b81e-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="3b81e-123">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3b81e-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="3b81e-124">无</span><span class="sxs-lookup"><span data-stu-id="3b81e-124">None</span></span> | <span data-ttu-id="3b81e-125">删除 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="3b81e-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b81e-126">属性</span><span class="sxs-lookup"><span data-stu-id="3b81e-126">Properties</span></span>

| <span data-ttu-id="3b81e-127">属性</span><span class="sxs-lookup"><span data-stu-id="3b81e-127">Property</span></span>     | <span data-ttu-id="3b81e-128">类型</span><span class="sxs-lookup"><span data-stu-id="3b81e-128">Type</span></span>        | <span data-ttu-id="3b81e-129">说明</span><span class="sxs-lookup"><span data-stu-id="3b81e-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3b81e-130">id</span><span class="sxs-lookup"><span data-stu-id="3b81e-130">id</span></span> | <span data-ttu-id="3b81e-131">String</span><span class="sxs-lookup"><span data-stu-id="3b81e-131">String</span></span> | <span data-ttu-id="3b81e-132">unifiedRoleAssignmentMultiple 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3b81e-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="3b81e-133">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="3b81e-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="3b81e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3b81e-134">displayName</span></span> | <span data-ttu-id="3b81e-135">String</span><span class="sxs-lookup"><span data-stu-id="3b81e-135">String</span></span> | <span data-ttu-id="3b81e-136">名称角色分配。</span><span class="sxs-lookup"><span data-stu-id="3b81e-136">Name of the role assignment.</span></span> <span data-ttu-id="3b81e-137">必需。</span><span class="sxs-lookup"><span data-stu-id="3b81e-137">Required.</span></span> |
| <span data-ttu-id="3b81e-138">description</span><span class="sxs-lookup"><span data-stu-id="3b81e-138">description</span></span> | <span data-ttu-id="3b81e-139">String</span><span class="sxs-lookup"><span data-stu-id="3b81e-139">String</span></span> | <span data-ttu-id="3b81e-140">属性角色分配。</span><span class="sxs-lookup"><span data-stu-id="3b81e-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="3b81e-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3b81e-141">roleDefinitionId</span></span> | <span data-ttu-id="3b81e-142">String</span><span class="sxs-lookup"><span data-stu-id="3b81e-142">String</span></span> | <span data-ttu-id="3b81e-143">分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b81e-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="3b81e-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b81e-144">roleDefinition</span></span> | [<span data-ttu-id="3b81e-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b81e-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="3b81e-146">指示工作分配所针对的角色定义的属性。</span><span class="sxs-lookup"><span data-stu-id="3b81e-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="3b81e-147">提供，以便调用方可以在获取角色定义的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="3b81e-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="3b81e-148">只读。</span><span class="sxs-lookup"><span data-stu-id="3b81e-148">Read-only.</span></span>  |
| <span data-ttu-id="3b81e-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="3b81e-149">principalIds</span></span> | <span data-ttu-id="3b81e-150">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3b81e-150">String collection</span></span> | <span data-ttu-id="3b81e-151">分配所授予的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="3b81e-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="3b81e-152">principals</span><span class="sxs-lookup"><span data-stu-id="3b81e-152">principals</span></span>| <span data-ttu-id="3b81e-153">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b81e-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3b81e-154">引用分配的主体的只读集合。</span><span class="sxs-lookup"><span data-stu-id="3b81e-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="3b81e-155">提供此权限，以便调用方可以在获取权限的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="3b81e-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="3b81e-156">只读。</span><span class="sxs-lookup"><span data-stu-id="3b81e-156">Read-only.</span></span> |
| <span data-ttu-id="3b81e-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="3b81e-157">directoryScopeIds</span></span> | <span data-ttu-id="3b81e-158">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3b81e-158">String collection</span></span> | <span data-ttu-id="3b81e-159">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b81e-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="3b81e-160">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="3b81e-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="3b81e-161">目录范围是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="3b81e-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="3b81e-162">应用范围是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="3b81e-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="3b81e-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="3b81e-163">directoryScopes</span></span> | <span data-ttu-id="3b81e-164">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b81e-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3b81e-165">引用作为分配范围的目录对象的只读集合。</span><span class="sxs-lookup"><span data-stu-id="3b81e-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="3b81e-166">提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="3b81e-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="3b81e-167">只读。</span><span class="sxs-lookup"><span data-stu-id="3b81e-167">Read-only.</span></span> |
| <span data-ttu-id="3b81e-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="3b81e-168">appScopeIds</span></span> | <span data-ttu-id="3b81e-169">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3b81e-169">String collection</span></span> | <span data-ttu-id="3b81e-170">当分配范围特定于应用时，应用特定范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b81e-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="3b81e-171">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="3b81e-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="3b81e-172">目录范围是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="3b81e-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="3b81e-173">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="3b81e-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="3b81e-174">应用范围是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="3b81e-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="3b81e-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="3b81e-175">appScopes</span></span> | <span data-ttu-id="3b81e-176">[appScope](appscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b81e-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="3b81e-177">当分配范围特定于应用时，具有特定于应用的范围的详细信息的只读集合。</span><span class="sxs-lookup"><span data-stu-id="3b81e-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="3b81e-178">包含实体。</span><span class="sxs-lookup"><span data-stu-id="3b81e-178">Containment entity.</span></span> <span data-ttu-id="3b81e-179">只读。</span><span class="sxs-lookup"><span data-stu-id="3b81e-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="3b81e-180">关系</span><span class="sxs-lookup"><span data-stu-id="3b81e-180">Relationships</span></span>

<span data-ttu-id="3b81e-181">无</span><span class="sxs-lookup"><span data-stu-id="3b81e-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b81e-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b81e-182">JSON representation</span></span>

<span data-ttu-id="3b81e-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b81e-183">The following is a JSON representation of the resource.</span></span>

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


