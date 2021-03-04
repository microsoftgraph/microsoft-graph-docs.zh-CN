---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在"角色分配 Identity Management"中执行所有操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 889baa55f6f639537b278eff5ff4b93cbfc8a1f6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443095"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="78a12-103">governanceRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="78a12-103">governanceRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="78a12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78a12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78a12-105">表示在"角色分配 Identity Management"中执行所有操作的请求。</span><span class="sxs-lookup"><span data-stu-id="78a12-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="78a12-106">`governanceRoleAssignmentRequest` 是一个票证模型实体，用于管理角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="78a12-106">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="78a12-107">它表示用户和管理员的意图/决定，还提供了实现反复选择、审批入口等的灵活性，与直接公开、操作 `POST` `PUT` `DELETE` 相比 `governanceRoleAssignment` 。</span><span class="sxs-lookup"><span data-stu-id="78a12-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="78a12-108">Methods</span><span class="sxs-lookup"><span data-stu-id="78a12-108">Methods</span></span>

| <span data-ttu-id="78a12-109">方法</span><span class="sxs-lookup"><span data-stu-id="78a12-109">Method</span></span>          |<span data-ttu-id="78a12-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="78a12-110">Return Type</span></span>  |<span data-ttu-id="78a12-111">说明</span><span class="sxs-lookup"><span data-stu-id="78a12-111">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="78a12-112">获取</span><span class="sxs-lookup"><span data-stu-id="78a12-112">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="78a12-113">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="78a12-113">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="78a12-114">获取角色分配 ID 指定的请求。</span><span class="sxs-lookup"><span data-stu-id="78a12-114">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="78a12-115">List</span><span class="sxs-lookup"><span data-stu-id="78a12-115">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="78a12-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  集合</span><span class="sxs-lookup"><span data-stu-id="78a12-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="78a12-117">获取角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="78a12-117">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="78a12-118">创建</span><span class="sxs-lookup"><span data-stu-id="78a12-118">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="78a12-119">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="78a12-119">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="78a12-120">创建一个请求，以管理现有或新数据库的角色分配。</span><span class="sxs-lookup"><span data-stu-id="78a12-120">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="78a12-121">Cancel</span><span class="sxs-lookup"><span data-stu-id="78a12-121">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="78a12-122">取消挂起角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="78a12-122">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="78a12-123">更新</span><span class="sxs-lookup"><span data-stu-id="78a12-123">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="78a12-124">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="78a12-124">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="78a12-125">如果请求的状态为 ，则管理员更新对请求的决策 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="78a12-125">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="78a12-126">属性</span><span class="sxs-lookup"><span data-stu-id="78a12-126">Properties</span></span>
| <span data-ttu-id="78a12-127">属性</span><span class="sxs-lookup"><span data-stu-id="78a12-127">Property</span></span>                  | <span data-ttu-id="78a12-128">类型</span><span class="sxs-lookup"><span data-stu-id="78a12-128">Type</span></span>          |<span data-ttu-id="78a12-129">说明</span><span class="sxs-lookup"><span data-stu-id="78a12-129">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="78a12-130">id</span><span class="sxs-lookup"><span data-stu-id="78a12-130">id</span></span>                         |<span data-ttu-id="78a12-131">String</span><span class="sxs-lookup"><span data-stu-id="78a12-131">String</span></span>         |<span data-ttu-id="78a12-132">请求角色分配 ID。</span><span class="sxs-lookup"><span data-stu-id="78a12-132">The id of the role assignment request.</span></span>|
|<span data-ttu-id="78a12-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="78a12-133">resourceId</span></span>                 |<span data-ttu-id="78a12-134">String</span><span class="sxs-lookup"><span data-stu-id="78a12-134">String</span></span>         |<span data-ttu-id="78a12-135">必需。</span><span class="sxs-lookup"><span data-stu-id="78a12-135">Required.</span></span> <span data-ttu-id="78a12-136">与请求关联的角色分配 ID。</span><span class="sxs-lookup"><span data-stu-id="78a12-136">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="78a12-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="78a12-137">roleDefinitionId</span></span>           |<span data-ttu-id="78a12-138">String</span><span class="sxs-lookup"><span data-stu-id="78a12-138">String</span></span>         |<span data-ttu-id="78a12-139">必需。</span><span class="sxs-lookup"><span data-stu-id="78a12-139">Required.</span></span> <span data-ttu-id="78a12-140">与请求关联的角色分配定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="78a12-140">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="78a12-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="78a12-141">subjectId</span></span>                  |<span data-ttu-id="78a12-142">String</span><span class="sxs-lookup"><span data-stu-id="78a12-142">String</span></span>         |<span data-ttu-id="78a12-143">必需。</span><span class="sxs-lookup"><span data-stu-id="78a12-143">Required.</span></span> <span data-ttu-id="78a12-144">与请求关联的角色分配 ID。</span><span class="sxs-lookup"><span data-stu-id="78a12-144">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="78a12-145">type</span><span class="sxs-lookup"><span data-stu-id="78a12-145">type</span></span>                       |<span data-ttu-id="78a12-146">String</span><span class="sxs-lookup"><span data-stu-id="78a12-146">String</span></span>         |<span data-ttu-id="78a12-147">必需。</span><span class="sxs-lookup"><span data-stu-id="78a12-147">Required.</span></span> <span data-ttu-id="78a12-148">表示对象上的操作角色分配。</span><span class="sxs-lookup"><span data-stu-id="78a12-148">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="78a12-149">值可以是</span><span class="sxs-lookup"><span data-stu-id="78a12-149">The value can be</span></span> <ul><li><span data-ttu-id="78a12-150">`AdminAdd`：管理员将用户/组分配给角色;</span><span class="sxs-lookup"><span data-stu-id="78a12-150">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="78a12-151">`UserAdd`：用户激活符合条件的分配;</span><span class="sxs-lookup"><span data-stu-id="78a12-151">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="78a12-152">`AdminUpdate`：管理员更改现有角色分配</span><span class="sxs-lookup"><span data-stu-id="78a12-152">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="78a12-153">`AdminRemove`：管理员从角色中删除用户/组;</span><span class="sxs-lookup"><span data-stu-id="78a12-153">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="78a12-154">`UserRemove`：用户停用活动分配;</span><span class="sxs-lookup"><span data-stu-id="78a12-154">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="78a12-155">`UserExtend`：用户请求延长其过期分配;</span><span class="sxs-lookup"><span data-stu-id="78a12-155">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="78a12-156">`AdminExtend`：管理员扩展即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="78a12-156">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="78a12-157">`UserRenew`：用户请求续订其已过期的工作分配;</span><span class="sxs-lookup"><span data-stu-id="78a12-157">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="78a12-158">`AdminRenew`：管理员扩展即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="78a12-158">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="78a12-159">assignmentState</span><span class="sxs-lookup"><span data-stu-id="78a12-159">assignmentState</span></span>|<span data-ttu-id="78a12-160">String</span><span class="sxs-lookup"><span data-stu-id="78a12-160">String</span></span>  |<span data-ttu-id="78a12-161">必需。</span><span class="sxs-lookup"><span data-stu-id="78a12-161">Required.</span></span> <span data-ttu-id="78a12-162">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="78a12-162">The state of the assignment.</span></span> <span data-ttu-id="78a12-163">值可以是</span><span class="sxs-lookup"><span data-stu-id="78a12-163">The value can be</span></span> <ul><li> <span data-ttu-id="78a12-164">`Eligible` 对于符合条件的分配</span><span class="sxs-lookup"><span data-stu-id="78a12-164">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="78a12-165">`Active` - 如果由管理员直接分配，或由用户根据符合条件的分配 `Active` 激活。</span><span class="sxs-lookup"><span data-stu-id="78a12-165">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="78a12-166">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="78a12-166">requestedDateTime</span></span>          |<span data-ttu-id="78a12-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78a12-167">DateTimeOffset</span></span> |<span data-ttu-id="78a12-168">只读。</span><span class="sxs-lookup"><span data-stu-id="78a12-168">Read-only.</span></span> <span data-ttu-id="78a12-169">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="78a12-169">The request create time.</span></span> <span data-ttu-id="78a12-170">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="78a12-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78a12-171">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78a12-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78a12-172">schedule</span><span class="sxs-lookup"><span data-stu-id="78a12-172">schedule</span></span>                   |[<span data-ttu-id="78a12-173">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="78a12-173">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="78a12-174">请求的计划角色分配对象。</span><span class="sxs-lookup"><span data-stu-id="78a12-174">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="78a12-175">reason</span><span class="sxs-lookup"><span data-stu-id="78a12-175">reason</span></span>                     |<span data-ttu-id="78a12-176">String</span><span class="sxs-lookup"><span data-stu-id="78a12-176">String</span></span>         |<span data-ttu-id="78a12-177">用户和管理员在创建请求时提供的消息，说明为什么需要它。</span><span class="sxs-lookup"><span data-stu-id="78a12-177">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="78a12-178">status</span><span class="sxs-lookup"><span data-stu-id="78a12-178">status</span></span>                     |[<span data-ttu-id="78a12-179">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="78a12-179">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="78a12-180">请求角色分配状态。</span><span class="sxs-lookup"><span data-stu-id="78a12-180">The status of the role assignment request.</span></span>|
|<span data-ttu-id="78a12-181">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="78a12-181">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="78a12-182">String</span><span class="sxs-lookup"><span data-stu-id="78a12-182">String</span></span>        |<span data-ttu-id="78a12-183">如果这是角色激活请求，则它表示被引用 `eligible assignment` 的 ID;否则，值为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="78a12-183">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="78a12-184">关系</span><span class="sxs-lookup"><span data-stu-id="78a12-184">Relationships</span></span>
| <span data-ttu-id="78a12-185">关系</span><span class="sxs-lookup"><span data-stu-id="78a12-185">Relationship</span></span> | <span data-ttu-id="78a12-186">类型</span><span class="sxs-lookup"><span data-stu-id="78a12-186">Type</span></span>                                |<span data-ttu-id="78a12-187">说明</span><span class="sxs-lookup"><span data-stu-id="78a12-187">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="78a12-188">资源</span><span class="sxs-lookup"><span data-stu-id="78a12-188">resource</span></span>      |[<span data-ttu-id="78a12-189">governanceResource</span><span class="sxs-lookup"><span data-stu-id="78a12-189">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="78a12-190">只读。</span><span class="sxs-lookup"><span data-stu-id="78a12-190">Read-only.</span></span> <span data-ttu-id="78a12-191">请求的目标资源。</span><span class="sxs-lookup"><span data-stu-id="78a12-191">The resource that the request aims to.</span></span> |
|<span data-ttu-id="78a12-192">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="78a12-192">roleDefinition</span></span>|[<span data-ttu-id="78a12-193">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="78a12-193">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="78a12-194">只读。</span><span class="sxs-lookup"><span data-stu-id="78a12-194">Read-only.</span></span> <span data-ttu-id="78a12-195">请求的目标角色定义。</span><span class="sxs-lookup"><span data-stu-id="78a12-195">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="78a12-196">subject</span><span class="sxs-lookup"><span data-stu-id="78a12-196">subject</span></span>       |[<span data-ttu-id="78a12-197">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="78a12-197">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="78a12-198">只读。</span><span class="sxs-lookup"><span data-stu-id="78a12-198">Read-only.</span></span> <span data-ttu-id="78a12-199">用户/组主体。</span><span class="sxs-lookup"><span data-stu-id="78a12-199">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="78a12-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78a12-200">JSON representation</span></span>

<span data-ttu-id="78a12-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78a12-201">Here is a JSON representation of the resource.</span></span>

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


