---
title: unifiedRoleScheduleBase 资源类型
description: 将统一角色计划与统一角色资格计划角色分配统一角色计划的基础属性
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 898f990ae7ffa09b3f251ce83fd71da04c2eafc6
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299119"
---
# <a name="unifiedroleschedulebase-resource-type"></a><span data-ttu-id="d3846-103">unifiedRoleScheduleBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3846-103">unifiedRoleScheduleBase resource type</span></span>

<span data-ttu-id="d3846-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3846-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3846-105">将统一角色计划与统一角色资格计划角色分配统一角色计划的基础属性</span><span class="sxs-lookup"><span data-stu-id="d3846-105">Base property of unified role schedules that combines unified role assignment schedules and unified role eligibility schedules</span></span>

## <a name="properties"></a><span data-ttu-id="d3846-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3846-106">Properties</span></span>

| <span data-ttu-id="d3846-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3846-107">Property</span></span>         | <span data-ttu-id="d3846-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3846-108">Type</span></span>           | <span data-ttu-id="d3846-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3846-109">Description</span></span>               |
| :--------------- | :------------- | :------------------------ |
| <span data-ttu-id="d3846-110">appScopeId</span><span class="sxs-lookup"><span data-stu-id="d3846-110">appScopeId</span></span>       | <span data-ttu-id="d3846-111">String</span><span class="sxs-lookup"><span data-stu-id="d3846-111">String</span></span>         | <span data-ttu-id="d3846-112">当分配范围特定于应用时，特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3846-112">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="d3846-113">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="d3846-113">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="d3846-114">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="d3846-114">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="d3846-115">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="d3846-115">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="d3846-116">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="d3846-116">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="d3846-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3846-117">createdDateTime</span></span>  | <span data-ttu-id="d3846-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3846-118">DateTimeOffset</span></span> | <span data-ttu-id="d3846-119">创建计划的时间。</span><span class="sxs-lookup"><span data-stu-id="d3846-119">Time that the schedule was created.</span></span> |
| <span data-ttu-id="d3846-120">createdUsing</span><span class="sxs-lookup"><span data-stu-id="d3846-120">createdUsing</span></span>     | <span data-ttu-id="d3846-121">String</span><span class="sxs-lookup"><span data-stu-id="d3846-121">String</span></span>         | <span data-ttu-id="d3846-122">创建此计划的 roleAssignmentScheduleRequest 的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3846-122">ID of the roleAssignmentScheduleRequest that created this schedule.</span></span> |
| <span data-ttu-id="d3846-123">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="d3846-123">directoryScopeId</span></span> | <span data-ttu-id="d3846-124">String</span><span class="sxs-lookup"><span data-stu-id="d3846-124">String</span></span>         | <span data-ttu-id="d3846-125">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3846-125">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="d3846-126">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="d3846-126">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="d3846-127">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="d3846-127">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="d3846-128">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="d3846-128">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="d3846-129">id</span><span class="sxs-lookup"><span data-stu-id="d3846-129">id</span></span>               | <span data-ttu-id="d3846-130">String</span><span class="sxs-lookup"><span data-stu-id="d3846-130">String</span></span>         | <span data-ttu-id="d3846-131">unifiedRoleAssignmentSchedule 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d3846-131">The unique identifier for the unifiedRoleAssignmentSchedule.</span></span> <span data-ttu-id="d3846-132">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="d3846-132">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="d3846-133">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3846-133">modifiedDateTime</span></span> | <span data-ttu-id="d3846-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3846-134">DateTimeOffset</span></span> | <span data-ttu-id="d3846-135">上次更新计划的时间。</span><span class="sxs-lookup"><span data-stu-id="d3846-135">Last time the schedule was updated.</span></span> |
| <span data-ttu-id="d3846-136">principalId</span><span class="sxs-lookup"><span data-stu-id="d3846-136">principalId</span></span>      | <span data-ttu-id="d3846-137">String</span><span class="sxs-lookup"><span data-stu-id="d3846-137">String</span></span>         | <span data-ttu-id="d3846-138">要授予分配的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="d3846-138">Objectid of the principal to which the assignment is being granted to.</span></span> |
| <span data-ttu-id="d3846-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d3846-139">roleDefinitionId</span></span> | <span data-ttu-id="d3846-140">String</span><span class="sxs-lookup"><span data-stu-id="d3846-140">String</span></span>         | <span data-ttu-id="d3846-141">分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3846-141">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="d3846-142">只读。</span><span class="sxs-lookup"><span data-stu-id="d3846-142">Read only.</span></span> |
| <span data-ttu-id="d3846-143">状态</span><span class="sxs-lookup"><span data-stu-id="d3846-143">status</span></span>           | <span data-ttu-id="d3846-144">String</span><span class="sxs-lookup"><span data-stu-id="d3846-144">String</span></span>         | <span data-ttu-id="d3846-145">的状态 `roleAssignmentSchedule` 。</span><span class="sxs-lookup"><span data-stu-id="d3846-145">Status for the `roleAssignmentSchedule`.</span></span> <span data-ttu-id="d3846-146">它可以包含与状态相关的消息，如 `Provisioned` `Revoked` `Pending Provisioning` 、、 和 `Pending Approval` 。</span><span class="sxs-lookup"><span data-stu-id="d3846-146">It can include state related messages like `Provisioned`, `Revoked`, `Pending Provisioning`, and `Pending Approval`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3846-147">关系</span><span class="sxs-lookup"><span data-stu-id="d3846-147">Relationships</span></span>

| <span data-ttu-id="d3846-148">关系</span><span class="sxs-lookup"><span data-stu-id="d3846-148">Relationship</span></span>   | <span data-ttu-id="d3846-149">类型</span><span class="sxs-lookup"><span data-stu-id="d3846-149">Type</span></span>                                                                               | <span data-ttu-id="d3846-150">说明</span><span class="sxs-lookup"><span data-stu-id="d3846-150">Description</span></span>               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| <span data-ttu-id="d3846-151">activeInstance</span><span class="sxs-lookup"><span data-stu-id="d3846-151">activeInstance</span></span> | [<span data-ttu-id="d3846-152">unifiedRoleScheduleInstanceBase</span><span class="sxs-lookup"><span data-stu-id="d3846-152">unifiedRoleScheduleInstanceBase</span></span>](../resources/unifiedrolescheduleinstancebase.md) | <span data-ttu-id="d3846-153">将弃用。</span><span class="sxs-lookup"><span data-stu-id="d3846-153">Will be deprecated.</span></span> |
| <span data-ttu-id="d3846-154">appScope</span><span class="sxs-lookup"><span data-stu-id="d3846-154">appScope</span></span>       | [<span data-ttu-id="d3846-155">appScope</span><span class="sxs-lookup"><span data-stu-id="d3846-155">appScope</span></span>](../resources/appscope.md)                                               | <span data-ttu-id="d3846-156">只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d3846-156">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="d3846-157">包含实体。</span><span class="sxs-lookup"><span data-stu-id="d3846-157">Containment entity.</span></span> |
| <span data-ttu-id="d3846-158">directoryScope</span><span class="sxs-lookup"><span data-stu-id="d3846-158">directoryScope</span></span> | [<span data-ttu-id="d3846-159">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d3846-159">directoryObject</span></span>](../resources/directoryobject.md)                                 | <span data-ttu-id="d3846-160">引用作为工作分配范围的目录对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3846-160">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="d3846-161">提供，以便调用方可以在获取目录对象的同时使用 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="d3846-161">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="d3846-162">只读。</span><span class="sxs-lookup"><span data-stu-id="d3846-162">Read-only.</span></span> |
| <span data-ttu-id="d3846-163">principal</span><span class="sxs-lookup"><span data-stu-id="d3846-163">principal</span></span>      | [<span data-ttu-id="d3846-164">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d3846-164">directoryObject</span></span>](../resources/directoryobject.md)                                 | <span data-ttu-id="d3846-165">引用通过请求获取角色分配主体的属性。</span><span class="sxs-lookup"><span data-stu-id="d3846-165">Property referencing the principal that is getting a role assignment through the request.</span></span> <span data-ttu-id="d3846-166">提供此权限，以便调用方可以使用 与获取 角色分配 同时 `$expand` 使用。</span><span class="sxs-lookup"><span data-stu-id="d3846-166">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="d3846-167">只读。</span><span class="sxs-lookup"><span data-stu-id="d3846-167">Read-only.</span></span> |
| <span data-ttu-id="d3846-168">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d3846-168">roleDefinition</span></span> | [<span data-ttu-id="d3846-169">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d3846-169">unifiedRoleDefinition</span></span>](../resources/unifiedroledefinition.md)                     | <span data-ttu-id="d3846-170">指示分配所针对的 roleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="d3846-170">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="d3846-171">提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="d3846-171">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="d3846-172">roleDefinition.Id 自动展开。</span><span class="sxs-lookup"><span data-stu-id="d3846-172">roleDefinition.Id will be auto expanded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3846-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3846-173">JSON representation</span></span>

<span data-ttu-id="d3846-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3846-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String"
}
```
