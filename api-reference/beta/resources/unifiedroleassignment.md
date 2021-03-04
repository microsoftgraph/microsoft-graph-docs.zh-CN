---
title: unifiedRoleAssignment 资源类型
description: 角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 04d296371a5d10dc447ea7588fdfbf5faea4f99d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442710"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="5cddf-103">unifiedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cddf-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="5cddf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cddf-105">unifiedRoleAssignment 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="5cddf-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="5cddf-106">它表示分配给主体角色的角色 (通常是用户) 作用域中的角色定义。</span><span class="sxs-lookup"><span data-stu-id="5cddf-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="5cddf-107">需要提供 directoryScopeId 或 appScopeId。</span><span class="sxs-lookup"><span data-stu-id="5cddf-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="5cddf-108">Methods</span><span class="sxs-lookup"><span data-stu-id="5cddf-108">Methods</span></span>

| <span data-ttu-id="5cddf-109">方法</span><span class="sxs-lookup"><span data-stu-id="5cddf-109">Method</span></span>       | <span data-ttu-id="5cddf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cddf-110">Return Type</span></span> | <span data-ttu-id="5cddf-111">说明</span><span class="sxs-lookup"><span data-stu-id="5cddf-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5cddf-112">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5cddf-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="5cddf-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5cddf-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="5cddf-114">读取 unifiedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5cddf-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="5cddf-115">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5cddf-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="5cddf-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5cddf-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="5cddf-117">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="5cddf-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="5cddf-118">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5cddf-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="5cddf-119">无</span><span class="sxs-lookup"><span data-stu-id="5cddf-119">None</span></span> | <span data-ttu-id="5cddf-120">删除 unifiedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="5cddf-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cddf-121">属性</span><span class="sxs-lookup"><span data-stu-id="5cddf-121">Properties</span></span>

| <span data-ttu-id="5cddf-122">属性</span><span class="sxs-lookup"><span data-stu-id="5cddf-122">Property</span></span>     | <span data-ttu-id="5cddf-123">类型</span><span class="sxs-lookup"><span data-stu-id="5cddf-123">Type</span></span>        | <span data-ttu-id="5cddf-124">说明</span><span class="sxs-lookup"><span data-stu-id="5cddf-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cddf-125">id</span><span class="sxs-lookup"><span data-stu-id="5cddf-125">id</span></span>|<span data-ttu-id="5cddf-126">String</span><span class="sxs-lookup"><span data-stu-id="5cddf-126">String</span></span>| <span data-ttu-id="5cddf-127">unifiedRoleAssignment 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5cddf-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="5cddf-128">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="5cddf-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="5cddf-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5cddf-129">roleDefinitionId</span></span>|<span data-ttu-id="5cddf-130">String</span><span class="sxs-lookup"><span data-stu-id="5cddf-130">String</span></span>| <span data-ttu-id="5cddf-131">工作分配的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="5cddf-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="5cddf-132">只读。</span><span class="sxs-lookup"><span data-stu-id="5cddf-132">Read only.</span></span> |
|<span data-ttu-id="5cddf-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5cddf-133">roleDefinition</span></span>|[<span data-ttu-id="5cddf-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5cddf-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="5cddf-135">指示工作分配所针对的 roleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="5cddf-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="5cddf-136">已提供，以便调用方可以在获取角色定义的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="5cddf-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="5cddf-137">roleDefinition.Id自动展开</span><span class="sxs-lookup"><span data-stu-id="5cddf-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="5cddf-138">principalId</span><span class="sxs-lookup"><span data-stu-id="5cddf-138">principalId</span></span>|<span data-ttu-id="5cddf-139">String</span><span class="sxs-lookup"><span data-stu-id="5cddf-139">String</span></span>| <span data-ttu-id="5cddf-140">分配授予的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="5cddf-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="5cddf-141">principal</span><span class="sxs-lookup"><span data-stu-id="5cddf-141">principal</span></span>|[<span data-ttu-id="5cddf-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="5cddf-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="5cddf-143">引用分配的主体的属性。</span><span class="sxs-lookup"><span data-stu-id="5cddf-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="5cddf-144">提供此权限，以便呼叫者可以同时使用主体获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="5cddf-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="5cddf-145">只读。</span><span class="sxs-lookup"><span data-stu-id="5cddf-145">Read-only.</span></span> |
|<span data-ttu-id="5cddf-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="5cddf-146">directoryScopeId</span></span>|<span data-ttu-id="5cddf-147">String</span><span class="sxs-lookup"><span data-stu-id="5cddf-147">String</span></span>|<span data-ttu-id="5cddf-148">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="5cddf-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="5cddf-149">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="5cddf-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="5cddf-150">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="5cddf-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="5cddf-151">应用范围是仅此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="5cddf-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="5cddf-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="5cddf-152">directoryScope</span></span>|[<span data-ttu-id="5cddf-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="5cddf-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="5cddf-154">引用作为工作分配范围的目录对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5cddf-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="5cddf-155">提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="5cddf-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="5cddf-156">只读。</span><span class="sxs-lookup"><span data-stu-id="5cddf-156">Read-only.</span></span> |
|<span data-ttu-id="5cddf-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="5cddf-157">appScopeId</span></span>|<span data-ttu-id="5cddf-158">String</span><span class="sxs-lookup"><span data-stu-id="5cddf-158">String</span></span>|<span data-ttu-id="5cddf-159">当分配范围特定于应用时，应用特定范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="5cddf-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="5cddf-160">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="5cddf-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="5cddf-161">目录范围是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="5cddf-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="5cddf-162">对租户范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="5cddf-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="5cddf-163">应用范围是仅此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="5cddf-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="5cddf-164">appScope</span><span class="sxs-lookup"><span data-stu-id="5cddf-164">appScope</span></span>|[<span data-ttu-id="5cddf-165">appScope</span><span class="sxs-lookup"><span data-stu-id="5cddf-165">appScope</span></span>](appscope.md)|<span data-ttu-id="5cddf-166">当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。</span><span class="sxs-lookup"><span data-stu-id="5cddf-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="5cddf-167">包含实体。</span><span class="sxs-lookup"><span data-stu-id="5cddf-167">Containment entity.</span></span> |
|<span data-ttu-id="5cddf-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="5cddf-168">resourceScope</span></span>|<span data-ttu-id="5cddf-169">String</span><span class="sxs-lookup"><span data-stu-id="5cddf-169">String</span></span>| <span data-ttu-id="5cddf-170">unifiedRoleAssignment 适用的范围。</span><span class="sxs-lookup"><span data-stu-id="5cddf-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="5cddf-171">这是服务范围的"/"。</span><span class="sxs-lookup"><span data-stu-id="5cddf-171">This is "/" for service-wide.</span></span> <span data-ttu-id="5cddf-172">**请勿使用。此属性将很快弃用。**</span><span class="sxs-lookup"><span data-stu-id="5cddf-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cddf-173">关系</span><span class="sxs-lookup"><span data-stu-id="5cddf-173">Relationships</span></span>

<span data-ttu-id="5cddf-174">无</span><span class="sxs-lookup"><span data-stu-id="5cddf-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cddf-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cddf-175">JSON representation</span></span>

<span data-ttu-id="5cddf-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cddf-176">The following is a JSON representation of the resource.</span></span>

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

