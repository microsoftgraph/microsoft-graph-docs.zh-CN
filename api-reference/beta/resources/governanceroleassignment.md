---
title: governanceRoleAssignment 资源类型
description: 表示向角色分配用户或组。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 532ea3c1d8fe5b1bc1128994c96c493774e9b19b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964560"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="02032-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="02032-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="02032-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="02032-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="02032-105">表示向角色分配用户或组。</span><span class="sxs-lookup"><span data-stu-id="02032-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="02032-106">PRIVILEGEd Identity Management (PIM) 支持两种类型的分配：</span><span class="sxs-lookup"><span data-stu-id="02032-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="02032-107">活动分配 - 表示对资源的直接/激活访问。</span><span class="sxs-lookup"><span data-stu-id="02032-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="02032-108">符合条件的分配 - 表示资源特权访问的中间阶段，介于无访问和直接访问之间。</span><span class="sxs-lookup"><span data-stu-id="02032-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="02032-109">管理员可以提前将用户/组分配给 ，并且只要需要访问权限，就可以在 上获取对资源的即时访问权限 `eligible assignment` `activation` `eligible assignment` 几个小时。</span><span class="sxs-lookup"><span data-stu-id="02032-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="02032-110">激活后 `active assignment` ，将为用户/组的成员创建 以指示激活状态。</span><span class="sxs-lookup"><span data-stu-id="02032-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="02032-111">Methods</span><span class="sxs-lookup"><span data-stu-id="02032-111">Methods</span></span>

| <span data-ttu-id="02032-112">方法</span><span class="sxs-lookup"><span data-stu-id="02032-112">Method</span></span>          | <span data-ttu-id="02032-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="02032-113">Return Type</span></span> |<span data-ttu-id="02032-114">说明</span><span class="sxs-lookup"><span data-stu-id="02032-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="02032-115">获取</span><span class="sxs-lookup"><span data-stu-id="02032-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="02032-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="02032-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="02032-117">读取实体的属性和角色分配关系。</span><span class="sxs-lookup"><span data-stu-id="02032-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="02032-118">列表</span><span class="sxs-lookup"><span data-stu-id="02032-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="02032-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02032-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="02032-120">列出资源上的角色分配集合。</span><span class="sxs-lookup"><span data-stu-id="02032-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="02032-121">Export</span><span class="sxs-lookup"><span data-stu-id="02032-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="02032-122">octet-stream</span><span class="sxs-lookup"><span data-stu-id="02032-122">octet-stream</span></span> |<span data-ttu-id="02032-123">下载资源上的角色分配集合，并另存为 `.csv` 文件。</span><span class="sxs-lookup"><span data-stu-id="02032-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="02032-124">实体集不支持任何 、、 `POST` `PUT` 或 `PATCH` `DELETE` `roleAssignments` 操作。</span><span class="sxs-lookup"><span data-stu-id="02032-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="02032-125">对 执行的任何创建、更新和删除 `governanceRoleAssignment` 操作都由 完成 `governanceRoleAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="02032-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="02032-126">属性</span><span class="sxs-lookup"><span data-stu-id="02032-126">Properties</span></span>
| <span data-ttu-id="02032-127">属性</span><span class="sxs-lookup"><span data-stu-id="02032-127">Property</span></span>  | <span data-ttu-id="02032-128">类型</span><span class="sxs-lookup"><span data-stu-id="02032-128">Type</span></span>      |<span data-ttu-id="02032-129">说明</span><span class="sxs-lookup"><span data-stu-id="02032-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="02032-130">id</span><span class="sxs-lookup"><span data-stu-id="02032-130">id</span></span>         |<span data-ttu-id="02032-131">String</span><span class="sxs-lookup"><span data-stu-id="02032-131">String</span></span>     |<span data-ttu-id="02032-132">id of the 角色分配.</span><span class="sxs-lookup"><span data-stu-id="02032-132">The ID of the role assignment.</span></span> <span data-ttu-id="02032-133">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="02032-133">It is in GUID format.</span></span>|
|<span data-ttu-id="02032-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="02032-134">resourceId</span></span> |<span data-ttu-id="02032-135">String</span><span class="sxs-lookup"><span data-stu-id="02032-135">String</span></span>     |<span data-ttu-id="02032-136">必填。</span><span class="sxs-lookup"><span data-stu-id="02032-136">Required.</span></span> <span data-ttu-id="02032-137">与项目关联的角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="02032-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="02032-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="02032-138">roleDefinitionId</span></span>|<span data-ttu-id="02032-139">String</span><span class="sxs-lookup"><span data-stu-id="02032-139">String</span></span>|<span data-ttu-id="02032-140">必填。</span><span class="sxs-lookup"><span data-stu-id="02032-140">Required.</span></span> <span data-ttu-id="02032-141">角色定义的 ID，角色分配角色定义。</span><span class="sxs-lookup"><span data-stu-id="02032-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="02032-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="02032-142">subjectId</span></span>|<span data-ttu-id="02032-143">String</span><span class="sxs-lookup"><span data-stu-id="02032-143">String</span></span>       |<span data-ttu-id="02032-144">必填。</span><span class="sxs-lookup"><span data-stu-id="02032-144">Required.</span></span> <span data-ttu-id="02032-145">与用户关联的角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="02032-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="02032-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="02032-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="02032-147">String</span><span class="sxs-lookup"><span data-stu-id="02032-147">String</span></span>|<span data-ttu-id="02032-148">如果这是 和 由于 激活而创建的 ，则它表示 的 `active assignment` `eligible assignment` `eligible assignment` ID;否则，值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="02032-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="02032-149">externalId</span><span class="sxs-lookup"><span data-stu-id="02032-149">externalId</span></span>   |<span data-ttu-id="02032-150">String</span><span class="sxs-lookup"><span data-stu-id="02032-150">String</span></span>     |<span data-ttu-id="02032-151">用于标识提供程序中应用程序角色分配外部 ID。</span><span class="sxs-lookup"><span data-stu-id="02032-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="02032-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="02032-152">startDateTime</span></span>|<span data-ttu-id="02032-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02032-153">DateTimeOffset</span></span>|<span data-ttu-id="02032-154">会议开始时间角色分配。</span><span class="sxs-lookup"><span data-stu-id="02032-154">The start time of the role assignment.</span></span> <span data-ttu-id="02032-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="02032-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="02032-156">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="02032-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="02032-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="02032-157">endDateTime</span></span>|<span data-ttu-id="02032-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02032-158">DateTimeOffset</span></span>|<span data-ttu-id="02032-159">对于非永久角色分配，此时间将角色分配过期。</span><span class="sxs-lookup"><span data-stu-id="02032-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="02032-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="02032-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="02032-161">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="02032-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="02032-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="02032-162">assignmentState</span></span>|<span data-ttu-id="02032-163">String</span><span class="sxs-lookup"><span data-stu-id="02032-163">String</span></span>  |<span data-ttu-id="02032-164">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="02032-164">The state of the assignment.</span></span> <span data-ttu-id="02032-165">该值可用于符合条件的分配，或者如果该值是由管理员直接分配，或者由用户对符合条件的分配 `Eligible` `Active` `Active` 进行激活。</span><span class="sxs-lookup"><span data-stu-id="02032-165">The value can be `Eligible` for eligible assignment or `Active` if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="02032-166">memberType</span><span class="sxs-lookup"><span data-stu-id="02032-166">memberType</span></span>|<span data-ttu-id="02032-167">String</span><span class="sxs-lookup"><span data-stu-id="02032-167">String</span></span>      |<span data-ttu-id="02032-168">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="02032-168">The type of member.</span></span> <span data-ttu-id="02032-169">该值可以是： (如果 角色分配 继承自父资源范围) ，则 (如果 角色分配 不是继承的，但来自组分配) 的成员身份;如果 角色分配 既不继承也不从组分配) 继承 `Inherited` `Group` `User` (。</span><span class="sxs-lookup"><span data-stu-id="02032-169">The value can be: `Inherited` (if the role assignment is inherited from a parent resource scope), `Group` (if the role assignment is not inherited, but comes from the membership of a group assignment), or `User` (if the role assignment is neither inherited nor from a group assignment).</span></span>|


## <a name="relationships"></a><span data-ttu-id="02032-170">关系</span><span class="sxs-lookup"><span data-stu-id="02032-170">Relationships</span></span>
| <span data-ttu-id="02032-171">关系</span><span class="sxs-lookup"><span data-stu-id="02032-171">Relationship</span></span> | <span data-ttu-id="02032-172">类型</span><span class="sxs-lookup"><span data-stu-id="02032-172">Type</span></span>   |<span data-ttu-id="02032-173">说明</span><span class="sxs-lookup"><span data-stu-id="02032-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02032-174">资源</span><span class="sxs-lookup"><span data-stu-id="02032-174">resource</span></span>|[<span data-ttu-id="02032-175">governanceResource</span><span class="sxs-lookup"><span data-stu-id="02032-175">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="02032-176">只读。</span><span class="sxs-lookup"><span data-stu-id="02032-176">Read-only.</span></span> <span data-ttu-id="02032-177">与项目关联的角色分配。</span><span class="sxs-lookup"><span data-stu-id="02032-177">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="02032-178">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="02032-178">roleDefinition</span></span>|[<span data-ttu-id="02032-179">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="02032-179">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="02032-180">只读。</span><span class="sxs-lookup"><span data-stu-id="02032-180">Read-only.</span></span> <span data-ttu-id="02032-181">与角色关联的角色角色分配。</span><span class="sxs-lookup"><span data-stu-id="02032-181">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="02032-182">subject</span><span class="sxs-lookup"><span data-stu-id="02032-182">subject</span></span>|[<span data-ttu-id="02032-183">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="02032-183">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="02032-184">只读。</span><span class="sxs-lookup"><span data-stu-id="02032-184">Read-only.</span></span> <span data-ttu-id="02032-185">与项目关联的角色分配。</span><span class="sxs-lookup"><span data-stu-id="02032-185">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="02032-186">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="02032-186">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="02032-187">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="02032-187">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="02032-188">只读。</span><span class="sxs-lookup"><span data-stu-id="02032-188">Read-only.</span></span> <span data-ttu-id="02032-189">如果这是 和 由于 激活而创建的 ，则它表示 的 `active assignment` `eligible assignment` 对象 `eligible assignment` ;否则，值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="02032-189">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02032-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02032-190">JSON representation</span></span>

<span data-ttu-id="02032-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02032-191">Here is a JSON representation of the resource.</span></span>


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


