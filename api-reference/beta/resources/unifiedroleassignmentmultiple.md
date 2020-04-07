---
title: unifiedRoleAssignmentMultiple 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c8c3f66f051a2ab9a9855f3b9ec5fab79e9f5b33
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160336"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="30c04-103">unifiedRoleAssignmentMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="30c04-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="30c04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30c04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30c04-105">UnifiedRoleAssignmentMultiple 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="30c04-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="30c04-106">它表示分配给范围数组的主体（通常为用户）数组的角色定义。</span><span class="sxs-lookup"><span data-stu-id="30c04-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="30c04-107">此类 RBAC 提供程序的一个示例是 Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="30c04-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="30c04-108">在 Microsoft Intune 中，可以创建具有多个主体和多个作用域的角色分配。</span><span class="sxs-lookup"><span data-stu-id="30c04-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="30c04-109">提供 " **directoryScopeIds** " 或 " **appScopeIds** " 是必需的。</span><span class="sxs-lookup"><span data-stu-id="30c04-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="30c04-110">方法</span><span class="sxs-lookup"><span data-stu-id="30c04-110">Methods</span></span>

| <span data-ttu-id="30c04-111">方法</span><span class="sxs-lookup"><span data-stu-id="30c04-111">Method</span></span>       | <span data-ttu-id="30c04-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="30c04-112">Return Type</span></span> | <span data-ttu-id="30c04-113">说明</span><span class="sxs-lookup"><span data-stu-id="30c04-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="30c04-114">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="30c04-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="30c04-116">读取 unifiedRoleAssignmentMultiple 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30c04-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="30c04-117">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="30c04-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="30c04-119">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="30c04-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="30c04-120">更新 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="30c04-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="30c04-122">更新现有的 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="30c04-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="30c04-123">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="30c04-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="30c04-124">无</span><span class="sxs-lookup"><span data-stu-id="30c04-124">None</span></span> | <span data-ttu-id="30c04-125">删除 unifiedRoleAssignmentMultiple 对象。</span><span class="sxs-lookup"><span data-stu-id="30c04-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="30c04-126">属性</span><span class="sxs-lookup"><span data-stu-id="30c04-126">Properties</span></span>

| <span data-ttu-id="30c04-127">属性</span><span class="sxs-lookup"><span data-stu-id="30c04-127">Property</span></span>     | <span data-ttu-id="30c04-128">类型</span><span class="sxs-lookup"><span data-stu-id="30c04-128">Type</span></span>        | <span data-ttu-id="30c04-129">说明</span><span class="sxs-lookup"><span data-stu-id="30c04-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="30c04-130">id</span><span class="sxs-lookup"><span data-stu-id="30c04-130">id</span></span> | <span data-ttu-id="30c04-131">字符串</span><span class="sxs-lookup"><span data-stu-id="30c04-131">String</span></span> | <span data-ttu-id="30c04-132">UnifiedRoleAssignmentMultiple 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="30c04-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="30c04-133">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="30c04-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="30c04-134">displayName</span><span class="sxs-lookup"><span data-stu-id="30c04-134">displayName</span></span> | <span data-ttu-id="30c04-135">String</span><span class="sxs-lookup"><span data-stu-id="30c04-135">String</span></span> | <span data-ttu-id="30c04-136">角色分配的名称。</span><span class="sxs-lookup"><span data-stu-id="30c04-136">Name of the role assignment.</span></span> |
| <span data-ttu-id="30c04-137">description</span><span class="sxs-lookup"><span data-stu-id="30c04-137">description</span></span> | <span data-ttu-id="30c04-138">String</span><span class="sxs-lookup"><span data-stu-id="30c04-138">String</span></span> | <span data-ttu-id="30c04-139">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="30c04-139">Description of the role assignment.</span></span> |
| <span data-ttu-id="30c04-140">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="30c04-140">roleDefinitionId</span></span> | <span data-ttu-id="30c04-141">String</span><span class="sxs-lookup"><span data-stu-id="30c04-141">String</span></span> | <span data-ttu-id="30c04-142">工作分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="30c04-142">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="30c04-143">只读。</span><span class="sxs-lookup"><span data-stu-id="30c04-143">Read only.</span></span> |
| <span data-ttu-id="30c04-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="30c04-144">roleDefinition</span></span> | [<span data-ttu-id="30c04-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="30c04-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="30c04-146">指示工作分配所针对的 roleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="30c04-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="30c04-147">提供，以便呼叫者可以在获取角色分配`$expand`的同时使用该角色定义。</span><span class="sxs-lookup"><span data-stu-id="30c04-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> |
| <span data-ttu-id="30c04-148">principalIds</span><span class="sxs-lookup"><span data-stu-id="30c04-148">principalIds</span></span> | <span data-ttu-id="30c04-149">String 集合</span><span class="sxs-lookup"><span data-stu-id="30c04-149">String collection</span></span> | <span data-ttu-id="30c04-150">向其授予分配的主体的 Objectids。</span><span class="sxs-lookup"><span data-stu-id="30c04-150">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="30c04-151">原理</span><span class="sxs-lookup"><span data-stu-id="30c04-151">principals</span></span>| <span data-ttu-id="30c04-152">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="30c04-152">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="30c04-153">引用所分配的主体的只读集合。</span><span class="sxs-lookup"><span data-stu-id="30c04-153">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="30c04-154">提供，以便呼叫者可以在获取角色`$expand`分配的同时使用这些承担者。</span><span class="sxs-lookup"><span data-stu-id="30c04-154">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="30c04-155">只读。</span><span class="sxs-lookup"><span data-stu-id="30c04-155">Read-only.</span></span> |
| <span data-ttu-id="30c04-156">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="30c04-156">directoryScopeIds</span></span> | <span data-ttu-id="30c04-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="30c04-157">String collection</span></span> | <span data-ttu-id="30c04-158">表示工作分配范围的目录对象的 id。</span><span class="sxs-lookup"><span data-stu-id="30c04-158">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="30c04-159">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="30c04-159">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="30c04-160">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="30c04-160">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="30c04-161">应用范围是此应用程序仅定义和理解的作用域。</span><span class="sxs-lookup"><span data-stu-id="30c04-161">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="30c04-162">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="30c04-162">directoryScopes</span></span> | <span data-ttu-id="30c04-163">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="30c04-163">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="30c04-164">只读集合，引用属于分配范围的目录对象。</span><span class="sxs-lookup"><span data-stu-id="30c04-164">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="30c04-165">提供，以便呼叫者可以使用`$expand`与获取角色分配相同的时间获取目录对象。</span><span class="sxs-lookup"><span data-stu-id="30c04-165">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="30c04-166">只读。</span><span class="sxs-lookup"><span data-stu-id="30c04-166">Read-only.</span></span> |
| <span data-ttu-id="30c04-167">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="30c04-167">appScopeIds</span></span> | <span data-ttu-id="30c04-168">String 集合</span><span class="sxs-lookup"><span data-stu-id="30c04-168">String collection</span></span> | <span data-ttu-id="30c04-169">当分配作用域是特定于应用的应用程序特定作用域的 id。</span><span class="sxs-lookup"><span data-stu-id="30c04-169">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="30c04-170">工作分配的范围决定了主体已被授予访问权限的一组资源。</span><span class="sxs-lookup"><span data-stu-id="30c04-170">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="30c04-171">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="30c04-171">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="30c04-172">对租户范围范围使用 "/"。</span><span class="sxs-lookup"><span data-stu-id="30c04-172">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="30c04-173">应用范围是此应用程序仅定义和理解的作用域。</span><span class="sxs-lookup"><span data-stu-id="30c04-173">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="30c04-174">appScopes</span><span class="sxs-lookup"><span data-stu-id="30c04-174">appScopes</span></span> | <span data-ttu-id="30c04-175">[appScope](appscope.md)集合</span><span class="sxs-lookup"><span data-stu-id="30c04-175">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="30c04-176">只读集合，其中包含应用程序特定作用域的详细信息，当分配作用域为应用程序特定时。</span><span class="sxs-lookup"><span data-stu-id="30c04-176">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="30c04-177">包容实体。</span><span class="sxs-lookup"><span data-stu-id="30c04-177">Containment entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="30c04-178">关系</span><span class="sxs-lookup"><span data-stu-id="30c04-178">Relationships</span></span>

<span data-ttu-id="30c04-179">无</span><span class="sxs-lookup"><span data-stu-id="30c04-179">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30c04-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30c04-180">JSON representation</span></span>

<span data-ttu-id="30c04-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30c04-181">The following is a JSON representation of the resource.</span></span>

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