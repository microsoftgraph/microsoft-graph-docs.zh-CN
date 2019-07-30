---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理中对角色分配操作的请求。
localization_priority: Normal
ms.openlocfilehash: 3a828bc14def823aeba6e06f2efe924c67ba5052
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931877"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="3be8f-103">governanceRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="3be8f-103">governanceRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be8f-104">表示在 Privilegd 标识管理中对角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="3be8f-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="3be8f-105">`governanceRoleAssignmentRequest`是用于管理角色分配生命周期的票据建模实体。</span><span class="sxs-lookup"><span data-stu-id="3be8f-105">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="3be8f-106">它代表用户和管理员的意向/决定, 还提供了灵活性, 可实现定期 schduling、审批门等实施, 与直接公开`POST`、 `PUT`和`DELETE`操作相比`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="3be8f-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="3be8f-107">方法</span><span class="sxs-lookup"><span data-stu-id="3be8f-107">Methods</span></span>

| <span data-ttu-id="3be8f-108">方法</span><span class="sxs-lookup"><span data-stu-id="3be8f-108">Method</span></span>          |<span data-ttu-id="3be8f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3be8f-109">Return Type</span></span>  |<span data-ttu-id="3be8f-110">说明</span><span class="sxs-lookup"><span data-stu-id="3be8f-110">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="3be8f-111">Get</span><span class="sxs-lookup"><span data-stu-id="3be8f-111">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="3be8f-112">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="3be8f-112">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="3be8f-113">获取由 ID 指定的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="3be8f-113">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="3be8f-114">List</span><span class="sxs-lookup"><span data-stu-id="3be8f-114">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="3be8f-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="3be8f-115">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="3be8f-116">获取对资源的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="3be8f-116">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="3be8f-117">创建</span><span class="sxs-lookup"><span data-stu-id="3be8f-117">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="3be8f-118">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="3be8f-118">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="3be8f-119">创建一个请求, 以管理现有或新角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="3be8f-119">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="3be8f-120">Cancel</span><span class="sxs-lookup"><span data-stu-id="3be8f-120">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="3be8f-121">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="3be8f-121">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="3be8f-122">更新</span><span class="sxs-lookup"><span data-stu-id="3be8f-122">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="3be8f-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="3be8f-123">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="3be8f-124">如果请求处于的`PendingAdminDecision`状态, 管理员会根据请求更新决策。</span><span class="sxs-lookup"><span data-stu-id="3be8f-124">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="3be8f-125">属性</span><span class="sxs-lookup"><span data-stu-id="3be8f-125">Properties</span></span>
| <span data-ttu-id="3be8f-126">属性</span><span class="sxs-lookup"><span data-stu-id="3be8f-126">Property</span></span>                  | <span data-ttu-id="3be8f-127">类型</span><span class="sxs-lookup"><span data-stu-id="3be8f-127">Type</span></span>          |<span data-ttu-id="3be8f-128">说明</span><span class="sxs-lookup"><span data-stu-id="3be8f-128">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="3be8f-129">id</span><span class="sxs-lookup"><span data-stu-id="3be8f-129">id</span></span>                         |<span data-ttu-id="3be8f-130">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-130">String</span></span>         |<span data-ttu-id="3be8f-131">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="3be8f-131">The id of the role assignment request.</span></span>|
|<span data-ttu-id="3be8f-132">resourceId</span><span class="sxs-lookup"><span data-stu-id="3be8f-132">resourceId</span></span>                 |<span data-ttu-id="3be8f-133">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-133">String</span></span>         |<span data-ttu-id="3be8f-134">必需。</span><span class="sxs-lookup"><span data-stu-id="3be8f-134">Required.</span></span> <span data-ttu-id="3be8f-135">与角色分配请求关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="3be8f-135">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="3be8f-136">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3be8f-136">roleDefinitionId</span></span>           |<span data-ttu-id="3be8f-137">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-137">String</span></span>         |<span data-ttu-id="3be8f-138">必需。</span><span class="sxs-lookup"><span data-stu-id="3be8f-138">Required.</span></span> <span data-ttu-id="3be8f-139">与角色分配请求关联的角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="3be8f-139">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="3be8f-140">subjectId</span><span class="sxs-lookup"><span data-stu-id="3be8f-140">subjectId</span></span>                  |<span data-ttu-id="3be8f-141">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-141">String</span></span>         |<span data-ttu-id="3be8f-142">必需。</span><span class="sxs-lookup"><span data-stu-id="3be8f-142">Required.</span></span> <span data-ttu-id="3be8f-143">与角色分配请求相关联的主题的 id。</span><span class="sxs-lookup"><span data-stu-id="3be8f-143">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="3be8f-144">type</span><span class="sxs-lookup"><span data-stu-id="3be8f-144">type</span></span>                       |<span data-ttu-id="3be8f-145">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-145">String</span></span>         |<span data-ttu-id="3be8f-146">必需。</span><span class="sxs-lookup"><span data-stu-id="3be8f-146">Required.</span></span> <span data-ttu-id="3be8f-147">表示角色分配上操作的类型。</span><span class="sxs-lookup"><span data-stu-id="3be8f-147">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="3be8f-148">值可以是</span><span class="sxs-lookup"><span data-stu-id="3be8f-148">The value can be</span></span> <ul><li><span data-ttu-id="3be8f-149">`AdminAdd`: 管理员将用户/组分配给角色;</span><span class="sxs-lookup"><span data-stu-id="3be8f-149">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="3be8f-150">`UserAdd`: 用户激活符合条件的工作分配;</span><span class="sxs-lookup"><span data-stu-id="3be8f-150">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="3be8f-151">`AdminUpdate`: 管理员更改现有的角色分配</span><span class="sxs-lookup"><span data-stu-id="3be8f-151">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="3be8f-152">`AdminRemove`: 管理员从角色中删除用户/组;</span><span class="sxs-lookup"><span data-stu-id="3be8f-152">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="3be8f-153">`UserRemove`: 用户停用活动分配;</span><span class="sxs-lookup"><span data-stu-id="3be8f-153">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="3be8f-154">`UserExtend`: 用户请求扩展即将过期的工作分配;</span><span class="sxs-lookup"><span data-stu-id="3be8f-154">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="3be8f-155">`AdminExtend`: 管理员扩展了即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="3be8f-155">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="3be8f-156">`UserRenew`: 用户请求续订其过期的工作分配;</span><span class="sxs-lookup"><span data-stu-id="3be8f-156">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="3be8f-157">`AdminRenew`: 管理员扩展了即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="3be8f-157">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="3be8f-158">assignmentState</span><span class="sxs-lookup"><span data-stu-id="3be8f-158">assignmentState</span></span>|<span data-ttu-id="3be8f-159">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-159">String</span></span>  |<span data-ttu-id="3be8f-160">必需。</span><span class="sxs-lookup"><span data-stu-id="3be8f-160">Required.</span></span> <span data-ttu-id="3be8f-161">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="3be8f-161">The state of the assignment.</span></span> <span data-ttu-id="3be8f-162">值可以是</span><span class="sxs-lookup"><span data-stu-id="3be8f-162">The value can be</span></span> <ul><li> <span data-ttu-id="3be8f-163">`Eligible`对于符合条件的工作分配</span><span class="sxs-lookup"><span data-stu-id="3be8f-163">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="3be8f-164">`Active`-如果由管理员直接分配`Active` , 或由用户在符合条件的工作分配上激活。</span><span class="sxs-lookup"><span data-stu-id="3be8f-164">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="3be8f-165">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="3be8f-165">requestedDateTime</span></span>          |<span data-ttu-id="3be8f-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be8f-166">DateTimeOffset</span></span> |<span data-ttu-id="3be8f-167">只读。</span><span class="sxs-lookup"><span data-stu-id="3be8f-167">Read-only.</span></span> <span data-ttu-id="3be8f-168">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="3be8f-168">The request create time.</span></span> <span data-ttu-id="3be8f-169">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3be8f-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3be8f-170">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3be8f-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3be8f-171">schedule</span><span class="sxs-lookup"><span data-stu-id="3be8f-171">schedule</span></span>                   |[<span data-ttu-id="3be8f-172">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3be8f-172">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="3be8f-173">角色分配请求的 schedule 对象。</span><span class="sxs-lookup"><span data-stu-id="3be8f-173">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="3be8f-174">在于</span><span class="sxs-lookup"><span data-stu-id="3be8f-174">reason</span></span>                     |<span data-ttu-id="3be8f-175">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-175">String</span></span>         |<span data-ttu-id="3be8f-176">用户和管理员在创建请求时, 提供有关需要的原因的消息。</span><span class="sxs-lookup"><span data-stu-id="3be8f-176">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="3be8f-177">status</span><span class="sxs-lookup"><span data-stu-id="3be8f-177">status</span></span>                     |[<span data-ttu-id="3be8f-178">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="3be8f-178">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="3be8f-179">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="3be8f-179">The status of the role assignment request.</span></span>|
|<span data-ttu-id="3be8f-180">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="3be8f-180">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="3be8f-181">String</span><span class="sxs-lookup"><span data-stu-id="3be8f-181">String</span></span>        |<span data-ttu-id="3be8f-182">如果这是角色激活请求, 则它表示所引用的`eligible assignment` id;否则, 值为`null`。</span><span class="sxs-lookup"><span data-stu-id="3be8f-182">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="3be8f-183">关系</span><span class="sxs-lookup"><span data-stu-id="3be8f-183">Relationships</span></span>
| <span data-ttu-id="3be8f-184">关系</span><span class="sxs-lookup"><span data-stu-id="3be8f-184">Relationship</span></span> | <span data-ttu-id="3be8f-185">类型</span><span class="sxs-lookup"><span data-stu-id="3be8f-185">Type</span></span>                                |<span data-ttu-id="3be8f-186">说明</span><span class="sxs-lookup"><span data-stu-id="3be8f-186">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="3be8f-187">资源</span><span class="sxs-lookup"><span data-stu-id="3be8f-187">resource</span></span>      |[<span data-ttu-id="3be8f-188">governanceResource</span><span class="sxs-lookup"><span data-stu-id="3be8f-188">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="3be8f-189">只读。</span><span class="sxs-lookup"><span data-stu-id="3be8f-189">Read-only.</span></span> <span data-ttu-id="3be8f-190">请求的目标资源。</span><span class="sxs-lookup"><span data-stu-id="3be8f-190">The resource that the request aims to.</span></span> |
|<span data-ttu-id="3be8f-191">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be8f-191">roleDefinition</span></span>|[<span data-ttu-id="3be8f-192">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3be8f-192">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="3be8f-193">只读。</span><span class="sxs-lookup"><span data-stu-id="3be8f-193">Read-only.</span></span> <span data-ttu-id="3be8f-194">请求所针对的角色定义。</span><span class="sxs-lookup"><span data-stu-id="3be8f-194">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="3be8f-195">subject</span><span class="sxs-lookup"><span data-stu-id="3be8f-195">subject</span></span>       |[<span data-ttu-id="3be8f-196">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="3be8f-196">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="3be8f-197">只读。</span><span class="sxs-lookup"><span data-stu-id="3be8f-197">Read-only.</span></span> <span data-ttu-id="3be8f-198">User/group 主体。</span><span class="sxs-lookup"><span data-stu-id="3be8f-198">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="3be8f-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3be8f-199">JSON representation</span></span>

<span data-ttu-id="3be8f-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3be8f-200">Here is a JSON representation of the resource.</span></span>

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
