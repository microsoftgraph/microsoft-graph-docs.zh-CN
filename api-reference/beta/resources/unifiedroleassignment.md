---
title: unifiedRoleAssignment 资源类型
description: 一角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4dc0ec6bb692c88d2b01a440bae1d7789bd042a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159022"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="87f95-103">unifiedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="87f95-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="87f95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87f95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87f95-105">unifiedRoleAssignment 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="87f95-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="87f95-106">它表示分配给主体的角色定义 (通常是特定) 用户的角色定义。</span><span class="sxs-lookup"><span data-stu-id="87f95-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="87f95-107">提供 directoryScopeId 或 appScopeId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="87f95-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="87f95-108">方法</span><span class="sxs-lookup"><span data-stu-id="87f95-108">Methods</span></span>

| <span data-ttu-id="87f95-109">方法</span><span class="sxs-lookup"><span data-stu-id="87f95-109">Method</span></span>       | <span data-ttu-id="87f95-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="87f95-110">Return Type</span></span> | <span data-ttu-id="87f95-111">说明</span><span class="sxs-lookup"><span data-stu-id="87f95-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="87f95-112">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="87f95-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="87f95-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="87f95-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="87f95-114">读取 unifiedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87f95-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="87f95-115">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="87f95-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="87f95-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="87f95-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="87f95-117">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="87f95-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="87f95-118">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="87f95-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="87f95-119">无</span><span class="sxs-lookup"><span data-stu-id="87f95-119">None</span></span> | <span data-ttu-id="87f95-120">删除 unifiedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="87f95-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="87f95-121">属性</span><span class="sxs-lookup"><span data-stu-id="87f95-121">Properties</span></span>

| <span data-ttu-id="87f95-122">属性</span><span class="sxs-lookup"><span data-stu-id="87f95-122">Property</span></span>     | <span data-ttu-id="87f95-123">类型</span><span class="sxs-lookup"><span data-stu-id="87f95-123">Type</span></span>        | <span data-ttu-id="87f95-124">说明</span><span class="sxs-lookup"><span data-stu-id="87f95-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87f95-125">id</span><span class="sxs-lookup"><span data-stu-id="87f95-125">id</span></span>|<span data-ttu-id="87f95-126">String</span><span class="sxs-lookup"><span data-stu-id="87f95-126">String</span></span>| <span data-ttu-id="87f95-127">unifiedRoleAssignment 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="87f95-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="87f95-128">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="87f95-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="87f95-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="87f95-129">roleDefinitionId</span></span>|<span data-ttu-id="87f95-130">String</span><span class="sxs-lookup"><span data-stu-id="87f95-130">String</span></span>| <span data-ttu-id="87f95-131">分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="87f95-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="87f95-132">只读。</span><span class="sxs-lookup"><span data-stu-id="87f95-132">Read only.</span></span> |
|<span data-ttu-id="87f95-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="87f95-133">roleDefinition</span></span>|[<span data-ttu-id="87f95-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="87f95-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="87f95-135">指示工作分配所针对的角色定义的属性。</span><span class="sxs-lookup"><span data-stu-id="87f95-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="87f95-136">提供，以便调用方可以在获取角色定义的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="87f95-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="87f95-137">roleDefinition.Id自动展开</span><span class="sxs-lookup"><span data-stu-id="87f95-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="87f95-138">principalId</span><span class="sxs-lookup"><span data-stu-id="87f95-138">principalId</span></span>|<span data-ttu-id="87f95-139">String</span><span class="sxs-lookup"><span data-stu-id="87f95-139">String</span></span>| <span data-ttu-id="87f95-140">分配授予的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="87f95-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="87f95-141">principal</span><span class="sxs-lookup"><span data-stu-id="87f95-141">principal</span></span>|[<span data-ttu-id="87f95-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="87f95-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="87f95-143">引用分配的主体的属性。</span><span class="sxs-lookup"><span data-stu-id="87f95-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="87f95-144">提供此权限，以便调用方可以同时使用主体获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="87f95-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="87f95-145">只读。</span><span class="sxs-lookup"><span data-stu-id="87f95-145">Read-only.</span></span> |
|<span data-ttu-id="87f95-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="87f95-146">directoryScopeId</span></span>|<span data-ttu-id="87f95-147">String</span><span class="sxs-lookup"><span data-stu-id="87f95-147">String</span></span>|<span data-ttu-id="87f95-148">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="87f95-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="87f95-149">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="87f95-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="87f95-150">目录范围是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="87f95-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="87f95-151">应用范围是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="87f95-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="87f95-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="87f95-152">directoryScope</span></span>|[<span data-ttu-id="87f95-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="87f95-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="87f95-154">引用作为分配范围的目录对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87f95-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="87f95-155">提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="87f95-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="87f95-156">只读。</span><span class="sxs-lookup"><span data-stu-id="87f95-156">Read-only.</span></span> |
|<span data-ttu-id="87f95-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="87f95-157">appScopeId</span></span>|<span data-ttu-id="87f95-158">String</span><span class="sxs-lookup"><span data-stu-id="87f95-158">String</span></span>|<span data-ttu-id="87f95-159">当分配范围特定于应用时，应用特定范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="87f95-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="87f95-160">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="87f95-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="87f95-161">目录范围是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="87f95-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="87f95-162">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="87f95-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="87f95-163">应用范围是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="87f95-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="87f95-164">appScope</span><span class="sxs-lookup"><span data-stu-id="87f95-164">appScope</span></span>|[<span data-ttu-id="87f95-165">appScope</span><span class="sxs-lookup"><span data-stu-id="87f95-165">appScope</span></span>](appscope.md)|<span data-ttu-id="87f95-166">当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。</span><span class="sxs-lookup"><span data-stu-id="87f95-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="87f95-167">包含实体。</span><span class="sxs-lookup"><span data-stu-id="87f95-167">Containment entity.</span></span> |
|<span data-ttu-id="87f95-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="87f95-168">resourceScope</span></span>|<span data-ttu-id="87f95-169">String</span><span class="sxs-lookup"><span data-stu-id="87f95-169">String</span></span>| <span data-ttu-id="87f95-170">unifiedRoleAssignment 适用的范围。</span><span class="sxs-lookup"><span data-stu-id="87f95-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="87f95-171">对于服务范围，这是"/"。</span><span class="sxs-lookup"><span data-stu-id="87f95-171">This is "/" for service-wide.</span></span> <span data-ttu-id="87f95-172">**请勿使用。此属性将很快弃用。**</span><span class="sxs-lookup"><span data-stu-id="87f95-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="87f95-173">关系</span><span class="sxs-lookup"><span data-stu-id="87f95-173">Relationships</span></span>

<span data-ttu-id="87f95-174">无</span><span class="sxs-lookup"><span data-stu-id="87f95-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87f95-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87f95-175">JSON representation</span></span>

<span data-ttu-id="87f95-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87f95-176">The following is a JSON representation of the resource.</span></span>

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

