---
title: governanceRoleAssignment 资源类型
description: 表示将用户或组分配至角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6d9e1b56a503ffdf1bde6bde6a583b78f8a34851
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722305"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="37c00-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="37c00-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="37c00-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="37c00-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="37c00-105">表示将用户或组分配至角色。</span><span class="sxs-lookup"><span data-stu-id="37c00-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="37c00-106">PRIVILEGEd Identity Management (PIM) 支持两种类型的分配：</span><span class="sxs-lookup"><span data-stu-id="37c00-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="37c00-107">活动分配 - 表示对资源的直接/激活访问。</span><span class="sxs-lookup"><span data-stu-id="37c00-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="37c00-108">符合条件的分配 - 表示对资源的特权访问的中间阶段，介于无访问和直接访问之间。</span><span class="sxs-lookup"><span data-stu-id="37c00-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="37c00-109">管理员可以提前将用户/组分配给用户/组，只要需要访问权限，就可以在几个小时内立即访问 `eligible assignment` `activation` `eligible assignment` 资源。</span><span class="sxs-lookup"><span data-stu-id="37c00-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="37c00-110">激活后 `active assignment` ，将为用户/组的成员创建一个指示激活状态。</span><span class="sxs-lookup"><span data-stu-id="37c00-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="37c00-111">方法</span><span class="sxs-lookup"><span data-stu-id="37c00-111">Methods</span></span>

| <span data-ttu-id="37c00-112">方法</span><span class="sxs-lookup"><span data-stu-id="37c00-112">Method</span></span>          | <span data-ttu-id="37c00-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="37c00-113">Return Type</span></span> |<span data-ttu-id="37c00-114">说明</span><span class="sxs-lookup"><span data-stu-id="37c00-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="37c00-115">获取</span><span class="sxs-lookup"><span data-stu-id="37c00-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="37c00-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="37c00-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="37c00-117">读取实体的属性角色分配关系。</span><span class="sxs-lookup"><span data-stu-id="37c00-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="37c00-118">List</span><span class="sxs-lookup"><span data-stu-id="37c00-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="37c00-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="37c00-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="37c00-120">列出资源上的角色分配集合。</span><span class="sxs-lookup"><span data-stu-id="37c00-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="37c00-121">Export</span><span class="sxs-lookup"><span data-stu-id="37c00-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="37c00-122">octet-stream</span><span class="sxs-lookup"><span data-stu-id="37c00-122">octet-stream</span></span> |<span data-ttu-id="37c00-123">下载资源上的角色分配集合并另存为 `.csv` 文件。</span><span class="sxs-lookup"><span data-stu-id="37c00-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="37c00-124">实体 `POST` 集不支持 ，，或 `PUT` `PATCH` `DELETE` `roleAssignments` 操作。</span><span class="sxs-lookup"><span data-stu-id="37c00-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="37c00-125">任何创建、更新和删除操作 `governanceRoleAssignment` 都由 `governanceRoleAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="37c00-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="37c00-126">属性</span><span class="sxs-lookup"><span data-stu-id="37c00-126">Properties</span></span>
| <span data-ttu-id="37c00-127">属性</span><span class="sxs-lookup"><span data-stu-id="37c00-127">Property</span></span>  | <span data-ttu-id="37c00-128">类型</span><span class="sxs-lookup"><span data-stu-id="37c00-128">Type</span></span>      |<span data-ttu-id="37c00-129">说明</span><span class="sxs-lookup"><span data-stu-id="37c00-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="37c00-130">id</span><span class="sxs-lookup"><span data-stu-id="37c00-130">id</span></span>         |<span data-ttu-id="37c00-131">String</span><span class="sxs-lookup"><span data-stu-id="37c00-131">String</span></span>     |<span data-ttu-id="37c00-132">id of the 角色分配.</span><span class="sxs-lookup"><span data-stu-id="37c00-132">The ID of the role assignment.</span></span> <span data-ttu-id="37c00-133">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="37c00-133">It is in GUID format.</span></span>|
|<span data-ttu-id="37c00-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="37c00-134">resourceId</span></span> |<span data-ttu-id="37c00-135">String</span><span class="sxs-lookup"><span data-stu-id="37c00-135">String</span></span>     |<span data-ttu-id="37c00-136">必填。</span><span class="sxs-lookup"><span data-stu-id="37c00-136">Required.</span></span> <span data-ttu-id="37c00-137">与其关联的角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="37c00-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="37c00-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="37c00-138">roleDefinitionId</span></span>|<span data-ttu-id="37c00-139">String</span><span class="sxs-lookup"><span data-stu-id="37c00-139">String</span></span>|<span data-ttu-id="37c00-140">必填。</span><span class="sxs-lookup"><span data-stu-id="37c00-140">Required.</span></span> <span data-ttu-id="37c00-141">角色定义与角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="37c00-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="37c00-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="37c00-142">subjectId</span></span>|<span data-ttu-id="37c00-143">String</span><span class="sxs-lookup"><span data-stu-id="37c00-143">String</span></span>       |<span data-ttu-id="37c00-144">必填。</span><span class="sxs-lookup"><span data-stu-id="37c00-144">Required.</span></span> <span data-ttu-id="37c00-145">与其关联的角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="37c00-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="37c00-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="37c00-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="37c00-147">String</span><span class="sxs-lookup"><span data-stu-id="37c00-147">String</span></span>|<span data-ttu-id="37c00-148">如果这是由于激活 `active assignment` 而创建的，则它表示该 `eligible assignment` `eligible assignment` ID;否则，值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="37c00-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="37c00-149">externalId</span><span class="sxs-lookup"><span data-stu-id="37c00-149">externalId</span></span>   |<span data-ttu-id="37c00-150">String</span><span class="sxs-lookup"><span data-stu-id="37c00-150">String</span></span>     |<span data-ttu-id="37c00-151">用于标识提供程序中的外部角色分配 ID。</span><span class="sxs-lookup"><span data-stu-id="37c00-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="37c00-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="37c00-152">startDateTime</span></span>|<span data-ttu-id="37c00-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c00-153">DateTimeOffset</span></span>|<span data-ttu-id="37c00-154">开始时间的角色分配。</span><span class="sxs-lookup"><span data-stu-id="37c00-154">The start time of the role assignment.</span></span> <span data-ttu-id="37c00-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="37c00-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37c00-156">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="37c00-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="37c00-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="37c00-157">endDateTime</span></span>|<span data-ttu-id="37c00-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c00-158">DateTimeOffset</span></span>|<span data-ttu-id="37c00-159">对于非永久角色分配，此时角色分配过期。</span><span class="sxs-lookup"><span data-stu-id="37c00-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="37c00-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="37c00-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37c00-161">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="37c00-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="37c00-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="37c00-162">assignmentState</span></span>|<span data-ttu-id="37c00-163">String</span><span class="sxs-lookup"><span data-stu-id="37c00-163">String</span></span>  |<span data-ttu-id="37c00-164">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="37c00-164">The state of the assignment.</span></span> <span data-ttu-id="37c00-165">值可以是</span><span class="sxs-lookup"><span data-stu-id="37c00-165">The value can be</span></span> <ul><li> <span data-ttu-id="37c00-166">`Eligible` 对于符合条件的分配</span><span class="sxs-lookup"><span data-stu-id="37c00-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="37c00-167">`Active` - 如果由管理员直接分配，或由用户在符合条件的分配 `Active` 上激活。</span><span class="sxs-lookup"><span data-stu-id="37c00-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="37c00-168">memberType</span><span class="sxs-lookup"><span data-stu-id="37c00-168">memberType</span></span>|<span data-ttu-id="37c00-169">String</span><span class="sxs-lookup"><span data-stu-id="37c00-169">String</span></span>      |<span data-ttu-id="37c00-170">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="37c00-170">The type of member.</span></span> <span data-ttu-id="37c00-171">值可以是：</span><span class="sxs-lookup"><span data-stu-id="37c00-171">The value can be:</span></span> <ul><li><span data-ttu-id="37c00-172">`Inherited` - 角色分配父资源作用域继承的资源</span><span class="sxs-lookup"><span data-stu-id="37c00-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="37c00-173">`Group`- 角色分配继承，但来自组分配的成员身份</span><span class="sxs-lookup"><span data-stu-id="37c00-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="37c00-174">`User` - 角色分配既不继承也不从组分配继承。</span><span class="sxs-lookup"><span data-stu-id="37c00-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="37c00-175">关系</span><span class="sxs-lookup"><span data-stu-id="37c00-175">Relationships</span></span>
| <span data-ttu-id="37c00-176">关系</span><span class="sxs-lookup"><span data-stu-id="37c00-176">Relationship</span></span> | <span data-ttu-id="37c00-177">类型</span><span class="sxs-lookup"><span data-stu-id="37c00-177">Type</span></span>   |<span data-ttu-id="37c00-178">说明</span><span class="sxs-lookup"><span data-stu-id="37c00-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37c00-179">资源</span><span class="sxs-lookup"><span data-stu-id="37c00-179">resource</span></span>|[<span data-ttu-id="37c00-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="37c00-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="37c00-181">只读。</span><span class="sxs-lookup"><span data-stu-id="37c00-181">Read-only.</span></span> <span data-ttu-id="37c00-182">与项目关联的角色分配。</span><span class="sxs-lookup"><span data-stu-id="37c00-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="37c00-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="37c00-183">roleDefinition</span></span>|[<span data-ttu-id="37c00-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="37c00-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="37c00-185">只读。</span><span class="sxs-lookup"><span data-stu-id="37c00-185">Read-only.</span></span> <span data-ttu-id="37c00-186">与角色关联的角色角色分配。</span><span class="sxs-lookup"><span data-stu-id="37c00-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="37c00-187">subject</span><span class="sxs-lookup"><span data-stu-id="37c00-187">subject</span></span>|[<span data-ttu-id="37c00-188">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="37c00-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="37c00-189">只读。</span><span class="sxs-lookup"><span data-stu-id="37c00-189">Read-only.</span></span> <span data-ttu-id="37c00-190">与主题关联的角色分配。</span><span class="sxs-lookup"><span data-stu-id="37c00-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="37c00-191">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="37c00-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="37c00-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="37c00-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="37c00-193">只读。</span><span class="sxs-lookup"><span data-stu-id="37c00-193">Read-only.</span></span> <span data-ttu-id="37c00-194">如果这是一 `active assignment` 个由于激活而创建的， `eligible assignment` 则它表示该对象 `eligible assignment` ;否则，值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="37c00-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37c00-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37c00-195">JSON representation</span></span>

<span data-ttu-id="37c00-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37c00-196">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


