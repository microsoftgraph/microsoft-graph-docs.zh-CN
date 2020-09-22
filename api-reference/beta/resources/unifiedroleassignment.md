---
title: unifiedRoleAssignment 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf08510d15f661f98365fe0346eb72b9b6d7b0bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985627"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="a36b9-103">unifiedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="a36b9-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="a36b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a36b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a36b9-105">UnifiedRoleAssignment 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a36b9-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="a36b9-106">它表示分配给主体的角色定义 (通常是特定范围内的用户) 。</span><span class="sxs-lookup"><span data-stu-id="a36b9-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="a36b9-107">提供 directoryScopeId 或 appScopeId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="a36b9-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="a36b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="a36b9-108">Methods</span></span>

| <span data-ttu-id="a36b9-109">方法</span><span class="sxs-lookup"><span data-stu-id="a36b9-109">Method</span></span>       | <span data-ttu-id="a36b9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a36b9-110">Return Type</span></span> | <span data-ttu-id="a36b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="a36b9-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a36b9-112">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a36b9-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="a36b9-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a36b9-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="a36b9-114">读取 unifiedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a36b9-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="a36b9-115">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a36b9-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="a36b9-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a36b9-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="a36b9-117">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="a36b9-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="a36b9-118">删除 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a36b9-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="a36b9-119">无</span><span class="sxs-lookup"><span data-stu-id="a36b9-119">None</span></span> | <span data-ttu-id="a36b9-120">删除 unifiedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="a36b9-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a36b9-121">属性</span><span class="sxs-lookup"><span data-stu-id="a36b9-121">Properties</span></span>

| <span data-ttu-id="a36b9-122">属性</span><span class="sxs-lookup"><span data-stu-id="a36b9-122">Property</span></span>     | <span data-ttu-id="a36b9-123">类型</span><span class="sxs-lookup"><span data-stu-id="a36b9-123">Type</span></span>        | <span data-ttu-id="a36b9-124">说明</span><span class="sxs-lookup"><span data-stu-id="a36b9-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a36b9-125">id</span><span class="sxs-lookup"><span data-stu-id="a36b9-125">id</span></span>|<span data-ttu-id="a36b9-126">String</span><span class="sxs-lookup"><span data-stu-id="a36b9-126">String</span></span>| <span data-ttu-id="a36b9-127">UnifiedRoleAssignment 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a36b9-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="a36b9-128">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="a36b9-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="a36b9-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a36b9-129">roleDefinitionId</span></span>|<span data-ttu-id="a36b9-130">String</span><span class="sxs-lookup"><span data-stu-id="a36b9-130">String</span></span>| <span data-ttu-id="a36b9-131">工作分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="a36b9-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="a36b9-132">只读。</span><span class="sxs-lookup"><span data-stu-id="a36b9-132">Read only.</span></span> |
|<span data-ttu-id="a36b9-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a36b9-133">roleDefinition</span></span>|[<span data-ttu-id="a36b9-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a36b9-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="a36b9-135">指示工作分配所针对的 roleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="a36b9-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="a36b9-136">提供，以便呼叫者可以在获取角色分配的同时使用该角色定义 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="a36b9-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="a36b9-137">roleDefinition.Id 将自动展开</span><span class="sxs-lookup"><span data-stu-id="a36b9-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="a36b9-138">principalId</span><span class="sxs-lookup"><span data-stu-id="a36b9-138">principalId</span></span>|<span data-ttu-id="a36b9-139">String</span><span class="sxs-lookup"><span data-stu-id="a36b9-139">String</span></span>| <span data-ttu-id="a36b9-140">向其授予分配的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="a36b9-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="a36b9-141">作主</span><span class="sxs-lookup"><span data-stu-id="a36b9-141">principal</span></span>|[<span data-ttu-id="a36b9-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a36b9-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="a36b9-143">引用分配的主体的属性。</span><span class="sxs-lookup"><span data-stu-id="a36b9-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="a36b9-144">提供，以便呼叫者可以 `$expand` 在获取角色分配的同时使用。</span><span class="sxs-lookup"><span data-stu-id="a36b9-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="a36b9-145">只读。</span><span class="sxs-lookup"><span data-stu-id="a36b9-145">Read-only.</span></span> |
|<span data-ttu-id="a36b9-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="a36b9-146">directoryScopeId</span></span>|<span data-ttu-id="a36b9-147">String</span><span class="sxs-lookup"><span data-stu-id="a36b9-147">String</span></span>|<span data-ttu-id="a36b9-148">表示工作分配范围的目录对象的 Id。</span><span class="sxs-lookup"><span data-stu-id="a36b9-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="a36b9-149">工作分配的范围决定了主体已被授予访问权限的一组资源。</span><span class="sxs-lookup"><span data-stu-id="a36b9-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="a36b9-150">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="a36b9-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="a36b9-151">应用范围是此应用程序仅定义和理解的作用域。</span><span class="sxs-lookup"><span data-stu-id="a36b9-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="a36b9-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="a36b9-152">directoryScope</span></span>|[<span data-ttu-id="a36b9-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a36b9-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="a36b9-154">属性引用作为工作分配范围的目录对象。</span><span class="sxs-lookup"><span data-stu-id="a36b9-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="a36b9-155">提供，以便呼叫者可以使用 `$expand` 与获取角色分配相同的时间获取目录对象。</span><span class="sxs-lookup"><span data-stu-id="a36b9-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="a36b9-156">只读。</span><span class="sxs-lookup"><span data-stu-id="a36b9-156">Read-only.</span></span> |
|<span data-ttu-id="a36b9-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="a36b9-157">appScopeId</span></span>|<span data-ttu-id="a36b9-158">String</span><span class="sxs-lookup"><span data-stu-id="a36b9-158">String</span></span>|<span data-ttu-id="a36b9-159">当分配作用域是特定于应用的应用程序特定作用域的 Id。</span><span class="sxs-lookup"><span data-stu-id="a36b9-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="a36b9-160">工作分配的范围决定了主体已被授予访问权限的一组资源。</span><span class="sxs-lookup"><span data-stu-id="a36b9-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="a36b9-161">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="a36b9-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="a36b9-162">对租户范围范围使用 "/"。</span><span class="sxs-lookup"><span data-stu-id="a36b9-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="a36b9-163">应用范围是此应用程序仅定义和理解的作用域。</span><span class="sxs-lookup"><span data-stu-id="a36b9-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="a36b9-164">appScope</span><span class="sxs-lookup"><span data-stu-id="a36b9-164">appScope</span></span>|[<span data-ttu-id="a36b9-165">appScope</span><span class="sxs-lookup"><span data-stu-id="a36b9-165">appScope</span></span>](appscope.md)|<span data-ttu-id="a36b9-166">只读属性，其中包含特定应用程序作用域的详细信息，当分配作用域为应用程序特定时。</span><span class="sxs-lookup"><span data-stu-id="a36b9-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="a36b9-167">包容实体。</span><span class="sxs-lookup"><span data-stu-id="a36b9-167">Containment entity.</span></span> |
|<span data-ttu-id="a36b9-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="a36b9-168">resourceScope</span></span>|<span data-ttu-id="a36b9-169">String</span><span class="sxs-lookup"><span data-stu-id="a36b9-169">String</span></span>| <span data-ttu-id="a36b9-170">应用 unifiedRoleAssignment 的范围。</span><span class="sxs-lookup"><span data-stu-id="a36b9-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="a36b9-171">对于服务范围，这是 "/"。</span><span class="sxs-lookup"><span data-stu-id="a36b9-171">This is "/" for service-wide.</span></span> <span data-ttu-id="a36b9-172">**请勿使用。此属性将很快被弃用。**</span><span class="sxs-lookup"><span data-stu-id="a36b9-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="a36b9-173">关系</span><span class="sxs-lookup"><span data-stu-id="a36b9-173">Relationships</span></span>

<span data-ttu-id="a36b9-174">无</span><span class="sxs-lookup"><span data-stu-id="a36b9-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a36b9-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a36b9-175">JSON representation</span></span>

<span data-ttu-id="a36b9-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a36b9-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
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

