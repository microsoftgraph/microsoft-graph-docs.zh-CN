---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理角色分配操作的请求。
localization_priority: Normal
ms.openlocfilehash: 838d16455a2eaea2183d008800eaef72a0af2a15
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572099"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="2c2f6-103">governanceRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c2f6-103">governanceRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c2f6-104">表示在 Privilegd 标识管理角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="2c2f6-105">`governanceRoleAssignmentRequest`用于管理角色分配的生命周期的票证建模的实体。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-105">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="2c2f6-106">它表示意图/决策的用户和管理员，并且还提供灵活地启用实施定期 schduling、 审批入口和等等，与直接公开`POST`， `PUT`，和`DELETE`操作在`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="2c2f6-107">方法</span><span class="sxs-lookup"><span data-stu-id="2c2f6-107">Methods</span></span>

| <span data-ttu-id="2c2f6-108">方法</span><span class="sxs-lookup"><span data-stu-id="2c2f6-108">Method</span></span>          |<span data-ttu-id="2c2f6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c2f6-109">Return Type</span></span>  |<span data-ttu-id="2c2f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="2c2f6-110">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="2c2f6-111">Get</span><span class="sxs-lookup"><span data-stu-id="2c2f6-111">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="2c2f6-112">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c2f6-112">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="2c2f6-113">获取由 ID 指定的角色分配请求</span><span class="sxs-lookup"><span data-stu-id="2c2f6-113">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="2c2f6-114">List</span><span class="sxs-lookup"><span data-stu-id="2c2f6-114">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="2c2f6-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="2c2f6-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="2c2f6-116">获取角色分配请求的资源。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-116">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="2c2f6-117">Create</span><span class="sxs-lookup"><span data-stu-id="2c2f6-117">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="2c2f6-118">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c2f6-118">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="2c2f6-119">创建管理现有或新角色分配的生命周期的请求。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-119">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="2c2f6-120">Cancel</span><span class="sxs-lookup"><span data-stu-id="2c2f6-120">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="2c2f6-121">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-121">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="2c2f6-122">Update</span><span class="sxs-lookup"><span data-stu-id="2c2f6-122">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="2c2f6-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2c2f6-123">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="2c2f6-124">如果请求中的状态，管理员更新对请求的决策`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-124">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c2f6-125">属性</span><span class="sxs-lookup"><span data-stu-id="2c2f6-125">Properties</span></span>
| <span data-ttu-id="2c2f6-126">属性</span><span class="sxs-lookup"><span data-stu-id="2c2f6-126">Property</span></span>                  | <span data-ttu-id="2c2f6-127">类型</span><span class="sxs-lookup"><span data-stu-id="2c2f6-127">Type</span></span>          |<span data-ttu-id="2c2f6-128">说明</span><span class="sxs-lookup"><span data-stu-id="2c2f6-128">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="2c2f6-129">id</span><span class="sxs-lookup"><span data-stu-id="2c2f6-129">id</span></span>                         |<span data-ttu-id="2c2f6-130">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-130">String</span></span>         |<span data-ttu-id="2c2f6-131">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-131">The id of the role assignment request.</span></span>|
|<span data-ttu-id="2c2f6-132">resourceId</span><span class="sxs-lookup"><span data-stu-id="2c2f6-132">resourceId</span></span>                 |<span data-ttu-id="2c2f6-133">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-133">String</span></span>         |<span data-ttu-id="2c2f6-134">必需。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-134">Required.</span></span> <span data-ttu-id="2c2f6-135">与关联的角色分配请求的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-135">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="2c2f6-136">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2c2f6-136">roleDefinitionId</span></span>           |<span data-ttu-id="2c2f6-137">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-137">String</span></span>         |<span data-ttu-id="2c2f6-138">必需。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-138">Required.</span></span> <span data-ttu-id="2c2f6-139">角色分配请求相关联的角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-139">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="2c2f6-140">subjectId</span><span class="sxs-lookup"><span data-stu-id="2c2f6-140">subjectId</span></span>                  |<span data-ttu-id="2c2f6-141">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-141">String</span></span>         |<span data-ttu-id="2c2f6-142">必需。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-142">Required.</span></span> <span data-ttu-id="2c2f6-143">其关联的角色分配请求的主题的 id。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-143">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="2c2f6-144">type</span><span class="sxs-lookup"><span data-stu-id="2c2f6-144">type</span></span>                       |<span data-ttu-id="2c2f6-145">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-145">String</span></span>         |<span data-ttu-id="2c2f6-146">必需。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-146">Required.</span></span> <span data-ttu-id="2c2f6-147">表示的角色分配操作的类型。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-147">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="2c2f6-148">值可以是</span><span class="sxs-lookup"><span data-stu-id="2c2f6-148">The value can be</span></span> <ul><li><span data-ttu-id="2c2f6-149">`AdminAdd`： 管理员分配给角色; 用户/组</span><span class="sxs-lookup"><span data-stu-id="2c2f6-149">`AdminAdd`: Adminstrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="2c2f6-150">`UserAdd`： 用户激活合格分配;</span><span class="sxs-lookup"><span data-stu-id="2c2f6-150">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="2c2f6-151">`AdminUpdate`： 管理员更改现有角色分配</span><span class="sxs-lookup"><span data-stu-id="2c2f6-151">`AdminUpdate`: Adminstrators change existing role assignments</span></span></li><li><span data-ttu-id="2c2f6-152">`AdminRemove`： 管理员角色中移除用户/组</span><span class="sxs-lookup"><span data-stu-id="2c2f6-152">`AdminRemove`: Adminstrators remove users/groups from roles;</span></span><li><span data-ttu-id="2c2f6-153">`UserRemove`： 用户停用活动的工作分配;</span><span class="sxs-lookup"><span data-stu-id="2c2f6-153">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="2c2f6-154">`UserExtend`： 用户请求扩展其即将过期的分配;</span><span class="sxs-lookup"><span data-stu-id="2c2f6-154">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="2c2f6-155">`AdminExtend`： 管理员扩展即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-155">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="2c2f6-156">`UserRenew`: 续订其过期的分配; 用户申请</span><span class="sxs-lookup"><span data-stu-id="2c2f6-156">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="2c2f6-157">`AdminRenew`： 管理员扩展即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-157">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="2c2f6-158">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2c2f6-158">assignmentState</span></span>|<span data-ttu-id="2c2f6-159">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-159">String</span></span>  |<span data-ttu-id="2c2f6-160">必需。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-160">Required.</span></span> <span data-ttu-id="2c2f6-161">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-161">The state of the assignment.</span></span> <span data-ttu-id="2c2f6-162">值可以是</span><span class="sxs-lookup"><span data-stu-id="2c2f6-162">The value can be</span></span> <ul><li> <span data-ttu-id="2c2f6-163">`Eligible`合格的分配</span><span class="sxs-lookup"><span data-stu-id="2c2f6-163">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="2c2f6-164">`Active`-如果直接分配`Active`的管理员，或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-164">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="2c2f6-165">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c2f6-165">requestedDateTime</span></span>          |<span data-ttu-id="2c2f6-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c2f6-166">DateTimeOffset</span></span> |<span data-ttu-id="2c2f6-167">只读。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-167">Read-only.</span></span> <span data-ttu-id="2c2f6-168">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-168">The request create time.</span></span> <span data-ttu-id="2c2f6-169">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c2f6-170">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2c2f6-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2c2f6-171">计划</span><span class="sxs-lookup"><span data-stu-id="2c2f6-171">schedule</span></span>                   |[<span data-ttu-id="2c2f6-172">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2c2f6-172"> microsoft.graph.governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="2c2f6-173">角色分配请求的计划对象。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-173">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="2c2f6-174">原因</span><span class="sxs-lookup"><span data-stu-id="2c2f6-174">reason</span></span>                     |<span data-ttu-id="2c2f6-175">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-175">String</span></span>         |<span data-ttu-id="2c2f6-176">用户和管理员提供的一条消息时创建有关为什么需要请求。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-176">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="2c2f6-177">status</span><span class="sxs-lookup"><span data-stu-id="2c2f6-177">status</span></span>                     |[<span data-ttu-id="2c2f6-178">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="2c2f6-178">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="2c2f6-179">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-179">The status of the role assignment request.</span></span>|
|<span data-ttu-id="2c2f6-180">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="2c2f6-180">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="2c2f6-181">String</span><span class="sxs-lookup"><span data-stu-id="2c2f6-181">String</span></span>        |<span data-ttu-id="2c2f6-182">如果这是角色激活请求，它所表示的 id`eligible assignment`所引用;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-182">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="2c2f6-183">关系</span><span class="sxs-lookup"><span data-stu-id="2c2f6-183">Relationships</span></span>
| <span data-ttu-id="2c2f6-184">关系</span><span class="sxs-lookup"><span data-stu-id="2c2f6-184">Relationship</span></span> | <span data-ttu-id="2c2f6-185">类型</span><span class="sxs-lookup"><span data-stu-id="2c2f6-185">Type</span></span>                                |<span data-ttu-id="2c2f6-186">说明</span><span class="sxs-lookup"><span data-stu-id="2c2f6-186">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="2c2f6-187">资源</span><span class="sxs-lookup"><span data-stu-id="2c2f6-187">resource</span></span>      |[<span data-ttu-id="2c2f6-188">governanceResource</span><span class="sxs-lookup"><span data-stu-id="2c2f6-188">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="2c2f6-189">只读。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-189">Read-only.</span></span> <span data-ttu-id="2c2f6-190">旨在请求的资源。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-190">The resource that the request aims to.</span></span> |
|<span data-ttu-id="2c2f6-191">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2c2f6-191">roleDefinition</span></span>|[<span data-ttu-id="2c2f6-192">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2c2f6-192">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="2c2f6-193">只读。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-193">Read-only.</span></span> <span data-ttu-id="2c2f6-194">请求旨在角色定义。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-194">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="2c2f6-195">subject</span><span class="sxs-lookup"><span data-stu-id="2c2f6-195">subject</span></span>       |[<span data-ttu-id="2c2f6-196">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="2c2f6-196">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="2c2f6-197">只读。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-197">Read-only.</span></span> <span data-ttu-id="2c2f6-198">用户/组主体。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-198">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="2c2f6-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c2f6-199">JSON representation</span></span>

<span data-ttu-id="2c2f6-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c2f6-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
