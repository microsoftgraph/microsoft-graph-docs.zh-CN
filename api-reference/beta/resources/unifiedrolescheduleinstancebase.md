---
title: unifiedRoleScheduleInstanceBase 资源类型
description: 将统一角色计划实例与统角色分配角色资格计划实例组合在一起的统一角色计划实例的基属性
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ddf4311fdddc44089410a0f073d6e041660283f2
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682199"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a><span data-ttu-id="94a7d-103">unifiedRoleScheduleInstanceBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="94a7d-103">unifiedRoleScheduleInstanceBase resource type</span></span>

<span data-ttu-id="94a7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94a7d-105">"将统一角色计划实例与统角色分配角色资格计划实例组合在一起的统一角色计划实例的基属性</span><span class="sxs-lookup"><span data-stu-id="94a7d-105">"Base property of unified role schedule instance that combines unified role assignment schedule instance and unified role eligibility schedule instance</span></span>

## <a name="properties"></a><span data-ttu-id="94a7d-106">属性</span><span class="sxs-lookup"><span data-stu-id="94a7d-106">Properties</span></span>
|<span data-ttu-id="94a7d-107">属性</span><span class="sxs-lookup"><span data-stu-id="94a7d-107">Property</span></span>|<span data-ttu-id="94a7d-108">类型</span><span class="sxs-lookup"><span data-stu-id="94a7d-108">Type</span></span>|<span data-ttu-id="94a7d-109">说明</span><span class="sxs-lookup"><span data-stu-id="94a7d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a7d-110">appScopeId</span><span class="sxs-lookup"><span data-stu-id="94a7d-110">appScopeId</span></span>|<span data-ttu-id="94a7d-111">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-111">String</span></span>|<span data-ttu-id="94a7d-112">当分配范围特定于应用时，特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="94a7d-112">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="94a7d-113">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="94a7d-113">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="94a7d-114">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="94a7d-114">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="94a7d-115">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="94a7d-115">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="94a7d-116">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="94a7d-116">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="94a7d-117">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="94a7d-117">directoryScopeId</span></span>|<span data-ttu-id="94a7d-118">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-118">String</span></span>|<span data-ttu-id="94a7d-119">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="94a7d-119">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="94a7d-120">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="94a7d-120">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="94a7d-121">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="94a7d-121">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="94a7d-122">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="94a7d-122">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="94a7d-123">id</span><span class="sxs-lookup"><span data-stu-id="94a7d-123">id</span></span>|<span data-ttu-id="94a7d-124">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-124">String</span></span>|<span data-ttu-id="94a7d-125">unifiedRoleAssignmentScheduleInstance 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="94a7d-125">The unique identifier for the unifiedRoleAssignmentScheduleInstance.</span></span> <span data-ttu-id="94a7d-126">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="94a7d-126">Key, not nullable, Read-only.</span></span>|
|<span data-ttu-id="94a7d-127">principalId</span><span class="sxs-lookup"><span data-stu-id="94a7d-127">principalId</span></span>|<span data-ttu-id="94a7d-128">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-128">String</span></span>|<span data-ttu-id="94a7d-129">要授予分配的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="94a7d-129">Objectid of the principal to which the assignment is being granted to.</span></span>|
|<span data-ttu-id="94a7d-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="94a7d-130">roleDefinitionId</span></span>|<span data-ttu-id="94a7d-131">String</span><span class="sxs-lookup"><span data-stu-id="94a7d-131">String</span></span>|<span data-ttu-id="94a7d-132">分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="94a7d-132">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="94a7d-133">只读。</span><span class="sxs-lookup"><span data-stu-id="94a7d-133">Read only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94a7d-134">关系</span><span class="sxs-lookup"><span data-stu-id="94a7d-134">Relationships</span></span>
|<span data-ttu-id="94a7d-135">关系</span><span class="sxs-lookup"><span data-stu-id="94a7d-135">Relationship</span></span>|<span data-ttu-id="94a7d-136">类型</span><span class="sxs-lookup"><span data-stu-id="94a7d-136">Type</span></span>|<span data-ttu-id="94a7d-137">说明</span><span class="sxs-lookup"><span data-stu-id="94a7d-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a7d-138">appScope</span><span class="sxs-lookup"><span data-stu-id="94a7d-138">appScope</span></span>|[<span data-ttu-id="94a7d-139">appScope</span><span class="sxs-lookup"><span data-stu-id="94a7d-139">appScope</span></span>](../resources/appscope.md)|<span data-ttu-id="94a7d-140">只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。</span><span class="sxs-lookup"><span data-stu-id="94a7d-140">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="94a7d-141">包含实体。</span><span class="sxs-lookup"><span data-stu-id="94a7d-141">Containment entity.</span></span> |
|<span data-ttu-id="94a7d-142">directoryScope</span><span class="sxs-lookup"><span data-stu-id="94a7d-142">directoryScope</span></span>|[<span data-ttu-id="94a7d-143">directoryObject</span><span class="sxs-lookup"><span data-stu-id="94a7d-143">directoryObject</span></span>](../resources/directoryobject.md)|<span data-ttu-id="94a7d-144">分配范围的目录对象。</span><span class="sxs-lookup"><span data-stu-id="94a7d-144">The directory object that is the scope of the assignment.</span></span> <span data-ttu-id="94a7d-145">启用目录对象的检索，同时使用 获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="94a7d-145">Enables the retrieval of the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="94a7d-146">只读。</span><span class="sxs-lookup"><span data-stu-id="94a7d-146">Read-only.</span></span>|
|<span data-ttu-id="94a7d-147">principal</span><span class="sxs-lookup"><span data-stu-id="94a7d-147">principal</span></span>|[<span data-ttu-id="94a7d-148">directoryObject</span><span class="sxs-lookup"><span data-stu-id="94a7d-148">directoryObject</span></span>](../resources/directoryobject.md)|<span data-ttu-id="94a7d-149">通过请求获取角色分配主体。</span><span class="sxs-lookup"><span data-stu-id="94a7d-149">The principal that is getting a role assignment through the request.</span></span> <span data-ttu-id="94a7d-150">启用检索主体，同时使用 获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="94a7d-150">Enables the retrieval of the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="94a7d-151">只读。</span><span class="sxs-lookup"><span data-stu-id="94a7d-151">Read-only.</span></span>|
|<span data-ttu-id="94a7d-152">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="94a7d-152">roleDefinition</span></span>|[<span data-ttu-id="94a7d-153">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="94a7d-153">unifiedRoleDefinition</span></span>](../resources/unifiedroledefinition.md)|<span data-ttu-id="94a7d-154">工作分配的 roleDefinition。</span><span class="sxs-lookup"><span data-stu-id="94a7d-154">The roleDefinition for the assignment.</span></span> <span data-ttu-id="94a7d-155">启用检索角色定义，同时使用 获取 `$expand` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="94a7d-155">Enables the retrieval of the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="94a7d-156">将自动 roleDefinition.Id 扩展该设置。</span><span class="sxs-lookup"><span data-stu-id="94a7d-156">The roleDefinition.Id is automatically expanded.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94a7d-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94a7d-157">JSON representation</span></span>
<span data-ttu-id="94a7d-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a7d-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleInstanceBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String"
}
```
