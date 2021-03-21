---
title: governanceRoleAssignmentRequest 资源类型
description: 代表在"角色分配 Identity Management"中执行安全操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e96a0009c6108a77383fe770a6351d7b64efd6f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961277"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="d3f70-103">governanceRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3f70-103">governanceRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="d3f70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3f70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3f70-105">表示在"角色分配 Identity Management"中执行所有操作的请求。</span><span class="sxs-lookup"><span data-stu-id="d3f70-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="d3f70-106">`governanceRoleAssignmentRequest` 是一个票证模型实体，用于管理角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="d3f70-106">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="d3f70-107">它表示用户和管理员的意图/决定，并且提供了实现反复选择、审批入口等的灵活性，与直接公开 、 和 操作相比 `POST` `PUT` `DELETE` `governanceRoleAssignment` 。</span><span class="sxs-lookup"><span data-stu-id="d3f70-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="d3f70-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d3f70-108">Methods</span></span>

| <span data-ttu-id="d3f70-109">方法</span><span class="sxs-lookup"><span data-stu-id="d3f70-109">Method</span></span>          |<span data-ttu-id="d3f70-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3f70-110">Return Type</span></span>  |<span data-ttu-id="d3f70-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3f70-111">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="d3f70-112">获取</span><span class="sxs-lookup"><span data-stu-id="d3f70-112">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="d3f70-113">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d3f70-113">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="d3f70-114">获取角色分配 ID 指定的请求。</span><span class="sxs-lookup"><span data-stu-id="d3f70-114">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="d3f70-115">列表</span><span class="sxs-lookup"><span data-stu-id="d3f70-115">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="d3f70-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  集合</span><span class="sxs-lookup"><span data-stu-id="d3f70-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="d3f70-117">获取角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="d3f70-117">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="d3f70-118">创建</span><span class="sxs-lookup"><span data-stu-id="d3f70-118">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="d3f70-119">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d3f70-119">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="d3f70-120">创建管理现有或新数据库生命周期角色分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-120">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="d3f70-121">Cancel</span><span class="sxs-lookup"><span data-stu-id="d3f70-121">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="d3f70-122">取消挂起角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="d3f70-122">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="d3f70-123">更新</span><span class="sxs-lookup"><span data-stu-id="d3f70-123">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="d3f70-124">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d3f70-124">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="d3f70-125">如果请求的状态为 ，则管理员更新对请求的决策 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="d3f70-125">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3f70-126">属性</span><span class="sxs-lookup"><span data-stu-id="d3f70-126">Properties</span></span>
| <span data-ttu-id="d3f70-127">属性</span><span class="sxs-lookup"><span data-stu-id="d3f70-127">Property</span></span>                  | <span data-ttu-id="d3f70-128">类型</span><span class="sxs-lookup"><span data-stu-id="d3f70-128">Type</span></span>          |<span data-ttu-id="d3f70-129">说明</span><span class="sxs-lookup"><span data-stu-id="d3f70-129">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="d3f70-130">id</span><span class="sxs-lookup"><span data-stu-id="d3f70-130">id</span></span>                         |<span data-ttu-id="d3f70-131">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-131">String</span></span>         |<span data-ttu-id="d3f70-132">请求角色分配 ID。</span><span class="sxs-lookup"><span data-stu-id="d3f70-132">The id of the role assignment request.</span></span>|
|<span data-ttu-id="d3f70-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="d3f70-133">resourceId</span></span>                 |<span data-ttu-id="d3f70-134">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-134">String</span></span>         |<span data-ttu-id="d3f70-135">必填。</span><span class="sxs-lookup"><span data-stu-id="d3f70-135">Required.</span></span> <span data-ttu-id="d3f70-136">与请求关联的角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3f70-136">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="d3f70-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d3f70-137">roleDefinitionId</span></span>           |<span data-ttu-id="d3f70-138">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-138">String</span></span>         |<span data-ttu-id="d3f70-139">必填。</span><span class="sxs-lookup"><span data-stu-id="d3f70-139">Required.</span></span> <span data-ttu-id="d3f70-140">与请求关联的角色角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3f70-140">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="d3f70-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="d3f70-141">subjectId</span></span>                  |<span data-ttu-id="d3f70-142">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-142">String</span></span>         |<span data-ttu-id="d3f70-143">必填。</span><span class="sxs-lookup"><span data-stu-id="d3f70-143">Required.</span></span> <span data-ttu-id="d3f70-144">与请求关联的角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3f70-144">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="d3f70-145">type</span><span class="sxs-lookup"><span data-stu-id="d3f70-145">type</span></span>                       |<span data-ttu-id="d3f70-146">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-146">String</span></span>        |<span data-ttu-id="d3f70-147">必填。</span><span class="sxs-lookup"><span data-stu-id="d3f70-147">Required.</span></span> <span data-ttu-id="d3f70-148">表示对项目执行的操作角色分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-148">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="d3f70-149">可能的值是 `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminExtend` `UserRenew` ：、、、、。 `AdminRenew`</span><span class="sxs-lookup"><span data-stu-id="d3f70-149">The possible values are: `AdminAdd` , `UserAdd` , `AdminUpdate` , `AdminRemove` , `UserRemove` , `UserExtend` , `AdminExtend` , `UserRenew` , `AdminRenew`.</span></span>|
|<span data-ttu-id="d3f70-150">assignmentState</span><span class="sxs-lookup"><span data-stu-id="d3f70-150">assignmentState</span></span>|<span data-ttu-id="d3f70-151">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-151">String</span></span>  |<span data-ttu-id="d3f70-152">必填。</span><span class="sxs-lookup"><span data-stu-id="d3f70-152">Required.</span></span> <span data-ttu-id="d3f70-153">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="d3f70-153">The state of the assignment.</span></span> <span data-ttu-id="d3f70-154">可能的值包括： (符合条件的分配) 、 (（如果管理员直接分配 `Eligible`  `Active`) 、 (或由用户) 在符合条件的分配上激活 `Active` ）。</span><span class="sxs-lookup"><span data-stu-id="d3f70-154">The possible values are: `Eligible` (for eligible assignment),  `Active` (if it is directly assigned), `Active` (by administrators, or activated on an eligible assignment by the users).</span></span>|
|<span data-ttu-id="d3f70-155">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3f70-155">requestedDateTime</span></span>          |<span data-ttu-id="d3f70-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3f70-156">DateTimeOffset</span></span> |<span data-ttu-id="d3f70-157">只读。</span><span class="sxs-lookup"><span data-stu-id="d3f70-157">Read-only.</span></span> <span data-ttu-id="d3f70-158">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="d3f70-158">The request create time.</span></span> <span data-ttu-id="d3f70-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d3f70-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3f70-160">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d3f70-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d3f70-161">schedule</span><span class="sxs-lookup"><span data-stu-id="d3f70-161">schedule</span></span>                   |[<span data-ttu-id="d3f70-162">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d3f70-162">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="d3f70-163">请求的计划角色分配对象。</span><span class="sxs-lookup"><span data-stu-id="d3f70-163">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="d3f70-164">reason</span><span class="sxs-lookup"><span data-stu-id="d3f70-164">reason</span></span>                     |<span data-ttu-id="d3f70-165">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-165">String</span></span>         |<span data-ttu-id="d3f70-166">创建请求时由用户和管理员提供的消息，说明为什么需要该请求。</span><span class="sxs-lookup"><span data-stu-id="d3f70-166">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="d3f70-167">状态</span><span class="sxs-lookup"><span data-stu-id="d3f70-167">status</span></span>                     |[<span data-ttu-id="d3f70-168">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="d3f70-168">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="d3f70-169">请求角色分配状态。</span><span class="sxs-lookup"><span data-stu-id="d3f70-169">The status of the role assignment request.</span></span>|
|<span data-ttu-id="d3f70-170">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="d3f70-170">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="d3f70-171">String</span><span class="sxs-lookup"><span data-stu-id="d3f70-171">String</span></span>        |<span data-ttu-id="d3f70-172">如果这是角色激活请求，则它表示所引用 `eligible assignment` 的 ID;否则，值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="d3f70-172">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |

|<span data-ttu-id="d3f70-173">成员</span><span class="sxs-lookup"><span data-stu-id="d3f70-173">Member</span></span>|<span data-ttu-id="d3f70-174">说明</span><span class="sxs-lookup"><span data-stu-id="d3f70-174">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3f70-175">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="d3f70-175">AdminAdd</span></span>|<span data-ttu-id="d3f70-176">管理员将用户/组分配给角色。</span><span class="sxs-lookup"><span data-stu-id="d3f70-176">Administrators assign users/groups to roles.</span></span>|
|<span data-ttu-id="d3f70-177">UserAdd</span><span class="sxs-lookup"><span data-stu-id="d3f70-177">UserAdd</span></span>|<span data-ttu-id="d3f70-178">用户激活符合条件的分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-178">Users activate eligible assignments.</span></span>|
|<span data-ttu-id="d3f70-179">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="d3f70-179">AdminUpdate</span></span>|<span data-ttu-id="d3f70-180">管理员更改现有角色分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-180">Administrators change existing role assignments.</span></span>|
|<span data-ttu-id="d3f70-181">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="d3f70-181">AdminRemove</span></span>|<span data-ttu-id="d3f70-182">管理员从角色中删除用户/组。</span><span class="sxs-lookup"><span data-stu-id="d3f70-182">Administrators remove users/groups from roles.</span></span>|
|<span data-ttu-id="d3f70-183">UserRemove</span><span class="sxs-lookup"><span data-stu-id="d3f70-183">UserRemove</span></span>|<span data-ttu-id="d3f70-184">用户停用活动分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-184">Users deactivate active assignments.</span></span>|
|<span data-ttu-id="d3f70-185">UserExtend</span><span class="sxs-lookup"><span data-stu-id="d3f70-185">UserExtend</span></span>|<span data-ttu-id="d3f70-186">用户请求延长其过期分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-186">Users request to extend their expiring assignments.</span></span>|
|<span data-ttu-id="d3f70-187">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="d3f70-187">AdminExtend</span></span>|<span data-ttu-id="d3f70-188">管理员延长即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-188">Administrators extend expiring assignments.</span></span>|
|<span data-ttu-id="d3f70-189">UserRenew</span><span class="sxs-lookup"><span data-stu-id="d3f70-189">UserRenew</span></span>|<span data-ttu-id="d3f70-190">用户请求续订其已过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-190">Users request to renew their expired assignments.</span></span>|
|<span data-ttu-id="d3f70-191">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="d3f70-191">AdminRenew</span></span>|<span data-ttu-id="d3f70-192">管理员延长即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="d3f70-192">Administrators extend expiring assignments.</span></span>|



## <a name="relationships"></a><span data-ttu-id="d3f70-193">关系</span><span class="sxs-lookup"><span data-stu-id="d3f70-193">Relationships</span></span>
| <span data-ttu-id="d3f70-194">关系</span><span class="sxs-lookup"><span data-stu-id="d3f70-194">Relationship</span></span> | <span data-ttu-id="d3f70-195">类型</span><span class="sxs-lookup"><span data-stu-id="d3f70-195">Type</span></span>                                |<span data-ttu-id="d3f70-196">说明</span><span class="sxs-lookup"><span data-stu-id="d3f70-196">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="d3f70-197">资源</span><span class="sxs-lookup"><span data-stu-id="d3f70-197">resource</span></span>      |[<span data-ttu-id="d3f70-198">governanceResource</span><span class="sxs-lookup"><span data-stu-id="d3f70-198">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="d3f70-199">只读。</span><span class="sxs-lookup"><span data-stu-id="d3f70-199">Read-only.</span></span> <span data-ttu-id="d3f70-200">请求的目标资源。</span><span class="sxs-lookup"><span data-stu-id="d3f70-200">The resource that the request aims to.</span></span> |
|<span data-ttu-id="d3f70-201">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d3f70-201">roleDefinition</span></span>|[<span data-ttu-id="d3f70-202">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d3f70-202">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="d3f70-203">只读。</span><span class="sxs-lookup"><span data-stu-id="d3f70-203">Read-only.</span></span> <span data-ttu-id="d3f70-204">请求的目标角色定义。</span><span class="sxs-lookup"><span data-stu-id="d3f70-204">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="d3f70-205">subject</span><span class="sxs-lookup"><span data-stu-id="d3f70-205">subject</span></span>       |[<span data-ttu-id="d3f70-206">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="d3f70-206">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="d3f70-207">只读。</span><span class="sxs-lookup"><span data-stu-id="d3f70-207">Read-only.</span></span> <span data-ttu-id="d3f70-208">用户/组主体。</span><span class="sxs-lookup"><span data-stu-id="d3f70-208">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="d3f70-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3f70-209">JSON representation</span></span>

<span data-ttu-id="d3f70-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3f70-210">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


