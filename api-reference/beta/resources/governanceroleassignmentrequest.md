---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理中对角色分配操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 611622930d0ff79a2b65589a5029c9eff5e773af
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219233"
---
# <a name="governanceroleassignmentrequest-resource-type"></a><span data-ttu-id="f2e9f-103">governanceRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2e9f-103">governanceRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="f2e9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2e9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2e9f-105">表示在 Privilegd 标识管理中对角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="f2e9f-106">`governanceRoleAssignmentRequest`是用于管理角色分配生命周期的票据建模实体。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-106">`governanceRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="f2e9f-107">它表示用户和管理员的意向/决定，还提供了灵活性，可实现定期 schduling、审批门等实施，与直接`POST`公开、 `PUT`和`DELETE`操作相比。 `governanceRoleAssignment`</span><span class="sxs-lookup"><span data-stu-id="f2e9f-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST`, `PUT`, and `DELETE` operations on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="f2e9f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="f2e9f-108">Methods</span></span>

| <span data-ttu-id="f2e9f-109">方法</span><span class="sxs-lookup"><span data-stu-id="f2e9f-109">Method</span></span>          |<span data-ttu-id="f2e9f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2e9f-110">Return Type</span></span>  |<span data-ttu-id="f2e9f-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2e9f-111">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="f2e9f-112">获取</span><span class="sxs-lookup"><span data-stu-id="f2e9f-112">Get</span></span>](../api/governanceroleassignmentrequest-get.md) | [<span data-ttu-id="f2e9f-113">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2e9f-113">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="f2e9f-114">获取由 ID 指定的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-114">Get a role assignment request specified by ID.</span></span>  
|[<span data-ttu-id="f2e9f-115">List</span><span class="sxs-lookup"><span data-stu-id="f2e9f-115">List</span></span>](../api/governanceroleassignmentrequest-list.md) | <span data-ttu-id="f2e9f-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="f2e9f-116">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="f2e9f-117">获取对资源的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-117">Get role assignment requests on a resource.</span></span>|
|[<span data-ttu-id="f2e9f-118">创建</span><span class="sxs-lookup"><span data-stu-id="f2e9f-118">Create</span></span>](../api/governanceroleassignmentrequest-post.md)|  [<span data-ttu-id="f2e9f-119">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2e9f-119">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="f2e9f-120">创建一个请求，以管理现有或新角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-120">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="f2e9f-121">Cancel</span><span class="sxs-lookup"><span data-stu-id="f2e9f-121">Cancel</span></span>](../api/governanceroleassignmentrequest-cancel.md)|  |<span data-ttu-id="f2e9f-122">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-122">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="f2e9f-123">更新</span><span class="sxs-lookup"><span data-stu-id="f2e9f-123">Update</span></span>](../api/governanceroleassignmentrequest-update.md)| [<span data-ttu-id="f2e9f-124">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2e9f-124">governanceRoleAssignmentRequest</span></span>](../resources/governanceroleassignmentrequest.md)|<span data-ttu-id="f2e9f-125">如果请求处于的`PendingAdminDecision`状态，管理员会根据请求更新决策。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-125">Administrators update the decisions on requests if the requests are in status of `PendingAdminDecision`.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2e9f-126">属性</span><span class="sxs-lookup"><span data-stu-id="f2e9f-126">Properties</span></span>
| <span data-ttu-id="f2e9f-127">属性</span><span class="sxs-lookup"><span data-stu-id="f2e9f-127">Property</span></span>                  | <span data-ttu-id="f2e9f-128">类型</span><span class="sxs-lookup"><span data-stu-id="f2e9f-128">Type</span></span>          |<span data-ttu-id="f2e9f-129">说明</span><span class="sxs-lookup"><span data-stu-id="f2e9f-129">Description</span></span>|
|:--------------------------|:--------------|:----------|
|<span data-ttu-id="f2e9f-130">id</span><span class="sxs-lookup"><span data-stu-id="f2e9f-130">id</span></span>                         |<span data-ttu-id="f2e9f-131">String</span><span class="sxs-lookup"><span data-stu-id="f2e9f-131">String</span></span>         |<span data-ttu-id="f2e9f-132">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-132">The id of the role assignment request.</span></span>|
|<span data-ttu-id="f2e9f-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="f2e9f-133">resourceId</span></span>                 |<span data-ttu-id="f2e9f-134">String</span><span class="sxs-lookup"><span data-stu-id="f2e9f-134">String</span></span>         |<span data-ttu-id="f2e9f-135">必需。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-135">Required.</span></span> <span data-ttu-id="f2e9f-136">与角色分配请求关联的资源的 id。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-136">The id of the resource which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="f2e9f-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f2e9f-137">roleDefinitionId</span></span>           |<span data-ttu-id="f2e9f-138">字符串</span><span class="sxs-lookup"><span data-stu-id="f2e9f-138">String</span></span>         |<span data-ttu-id="f2e9f-139">必需。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-139">Required.</span></span> <span data-ttu-id="f2e9f-140">与角色分配请求关联的角色定义的 id。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-140">The id of the role definition which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="f2e9f-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="f2e9f-141">subjectId</span></span>                  |<span data-ttu-id="f2e9f-142">字符串</span><span class="sxs-lookup"><span data-stu-id="f2e9f-142">String</span></span>         |<span data-ttu-id="f2e9f-143">必需。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-143">Required.</span></span> <span data-ttu-id="f2e9f-144">与角色分配请求相关联的主题的 id。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-144">The id of the subject which the role assignment request is associated with.</span></span>|
|<span data-ttu-id="f2e9f-145">type</span><span class="sxs-lookup"><span data-stu-id="f2e9f-145">type</span></span>                       |<span data-ttu-id="f2e9f-146">字符串</span><span class="sxs-lookup"><span data-stu-id="f2e9f-146">String</span></span>         |<span data-ttu-id="f2e9f-147">必需。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-147">Required.</span></span> <span data-ttu-id="f2e9f-148">表示角色分配上操作的类型。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-148">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="f2e9f-149">值可以是</span><span class="sxs-lookup"><span data-stu-id="f2e9f-149">The value can be</span></span> <ul><li><span data-ttu-id="f2e9f-150">`AdminAdd`：管理员将用户/组分配给角色;</span><span class="sxs-lookup"><span data-stu-id="f2e9f-150">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="f2e9f-151">`UserAdd`：用户激活符合条件的工作分配;</span><span class="sxs-lookup"><span data-stu-id="f2e9f-151">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="f2e9f-152">`AdminUpdate`：管理员更改现有的角色分配</span><span class="sxs-lookup"><span data-stu-id="f2e9f-152">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="f2e9f-153">`AdminRemove`：管理员从角色中删除用户/组;</span><span class="sxs-lookup"><span data-stu-id="f2e9f-153">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="f2e9f-154">`UserRemove`：用户停用活动分配;</span><span class="sxs-lookup"><span data-stu-id="f2e9f-154">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="f2e9f-155">`UserExtend`：用户请求扩展即将过期的工作分配;</span><span class="sxs-lookup"><span data-stu-id="f2e9f-155">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="f2e9f-156">`AdminExtend`：管理员扩展了即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-156">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="f2e9f-157">`UserRenew`：用户请求续订其过期的工作分配;</span><span class="sxs-lookup"><span data-stu-id="f2e9f-157">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="f2e9f-158">`AdminRenew`：管理员扩展了即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-158">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="f2e9f-159">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f2e9f-159">assignmentState</span></span>|<span data-ttu-id="f2e9f-160">字符串</span><span class="sxs-lookup"><span data-stu-id="f2e9f-160">String</span></span>  |<span data-ttu-id="f2e9f-161">必需。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-161">Required.</span></span> <span data-ttu-id="f2e9f-162">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-162">The state of the assignment.</span></span> <span data-ttu-id="f2e9f-163">值可以是</span><span class="sxs-lookup"><span data-stu-id="f2e9f-163">The value can be</span></span> <ul><li> <span data-ttu-id="f2e9f-164">`Eligible`对于符合条件的工作分配</span><span class="sxs-lookup"><span data-stu-id="f2e9f-164">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="f2e9f-165">`Active`-如果由管理员直接分配`Active` ，或由用户在符合条件的工作分配上激活。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-165">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="f2e9f-166">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e9f-166">requestedDateTime</span></span>          |<span data-ttu-id="f2e9f-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e9f-167">DateTimeOffset</span></span> |<span data-ttu-id="f2e9f-168">只读。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-168">Read-only.</span></span> <span data-ttu-id="f2e9f-169">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-169">The request create time.</span></span> <span data-ttu-id="f2e9f-170">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2e9f-171">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f2e9f-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f2e9f-172">schedule</span><span class="sxs-lookup"><span data-stu-id="f2e9f-172">schedule</span></span>                   |[<span data-ttu-id="f2e9f-173">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2e9f-173">governanceSchedule</span></span>](governanceschedule.md)|<span data-ttu-id="f2e9f-174">角色分配请求的 schedule 对象。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-174">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="f2e9f-175">reason</span><span class="sxs-lookup"><span data-stu-id="f2e9f-175">reason</span></span>                     |<span data-ttu-id="f2e9f-176">字符串</span><span class="sxs-lookup"><span data-stu-id="f2e9f-176">String</span></span>         |<span data-ttu-id="f2e9f-177">用户和管理员在创建请求时，提供有关需要的原因的消息。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-177">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="f2e9f-178">状态</span><span class="sxs-lookup"><span data-stu-id="f2e9f-178">status</span></span>                     |[<span data-ttu-id="f2e9f-179">governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="f2e9f-179">governanceRoleAssignmentRequestStatus</span></span>](governanceroleassignmentrequeststatus.md)         |<span data-ttu-id="f2e9f-180">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-180">The status of the role assignment request.</span></span>|
|<span data-ttu-id="f2e9f-181">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="f2e9f-181">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="f2e9f-182">字符串</span><span class="sxs-lookup"><span data-stu-id="f2e9f-182">String</span></span>        |<span data-ttu-id="f2e9f-183">如果这是角色激活请求，则它表示所引用的`eligible assignment` id;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-183">If this is a request for role activation, it represents the id of the `eligible assignment` being referred; Otherwise, the value is `null`.</span></span> |



## <a name="relationships"></a><span data-ttu-id="f2e9f-184">关系</span><span class="sxs-lookup"><span data-stu-id="f2e9f-184">Relationships</span></span>
| <span data-ttu-id="f2e9f-185">关系</span><span class="sxs-lookup"><span data-stu-id="f2e9f-185">Relationship</span></span> | <span data-ttu-id="f2e9f-186">类型</span><span class="sxs-lookup"><span data-stu-id="f2e9f-186">Type</span></span>                                |<span data-ttu-id="f2e9f-187">说明</span><span class="sxs-lookup"><span data-stu-id="f2e9f-187">Description</span></span>|
|:-------------|:----------------------------------|:----------|
|<span data-ttu-id="f2e9f-188">资源</span><span class="sxs-lookup"><span data-stu-id="f2e9f-188">resource</span></span>      |[<span data-ttu-id="f2e9f-189">governanceResource</span><span class="sxs-lookup"><span data-stu-id="f2e9f-189">governanceResource</span></span>](../resources/governanceresource.md)            |<span data-ttu-id="f2e9f-190">只读。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-190">Read-only.</span></span> <span data-ttu-id="f2e9f-191">请求的目标资源。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-191">The resource that the request aims to.</span></span> |
|<span data-ttu-id="f2e9f-192">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f2e9f-192">roleDefinition</span></span>|[<span data-ttu-id="f2e9f-193">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f2e9f-193">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="f2e9f-194">只读。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-194">Read-only.</span></span> <span data-ttu-id="f2e9f-195">请求所针对的角色定义。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-195">The role definition that the request aims to.</span></span> |
|<span data-ttu-id="f2e9f-196">subject</span><span class="sxs-lookup"><span data-stu-id="f2e9f-196">subject</span></span>       |[<span data-ttu-id="f2e9f-197">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="f2e9f-197">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="f2e9f-198">只读。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-198">Read-only.</span></span> <span data-ttu-id="f2e9f-199">User/group 主体。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-199">The user/group principal.</span></span>|

### <a name="json-representation"></a><span data-ttu-id="f2e9f-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2e9f-200">JSON representation</span></span>

<span data-ttu-id="f2e9f-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2e9f-201">Here is a JSON representation of the resource.</span></span>

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
