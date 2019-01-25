---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理角色分配操作的请求。
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509005"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="73e47-103">privilegedRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="73e47-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73e47-104">表示在 Privilegd 标识管理角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="73e47-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="73e47-105">`privilegedRoleAssignmentRequest`用于管理角色分配的生命周期的票证建模的实体。</span><span class="sxs-lookup"><span data-stu-id="73e47-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="73e47-106">它表示意图/决策的用户和管理员，并且还提供灵活地启用实施定期 schduling、 审批入口和等等，与直接公开`POST`和`LIST`操作以及`MY`和`Cancel`函数上`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="73e47-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="73e47-107">方法</span><span class="sxs-lookup"><span data-stu-id="73e47-107">Methods</span></span>

| <span data-ttu-id="73e47-108">方法</span><span class="sxs-lookup"><span data-stu-id="73e47-108">Method</span></span>       | <span data-ttu-id="73e47-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="73e47-109">Return Type</span></span> | <span data-ttu-id="73e47-110">说明</span><span class="sxs-lookup"><span data-stu-id="73e47-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="73e47-111">List</span><span class="sxs-lookup"><span data-stu-id="73e47-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="73e47-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="73e47-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="73e47-113">列出角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="73e47-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="73e47-114">Create</span><span class="sxs-lookup"><span data-stu-id="73e47-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="73e47-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="73e47-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="73e47-116">创建管理现有或新角色分配的生命周期的请求。</span><span class="sxs-lookup"><span data-stu-id="73e47-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="73e47-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="73e47-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="73e47-118">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="73e47-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="73e47-119">My</span><span class="sxs-lookup"><span data-stu-id="73e47-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="73e47-120">获取当前 requstor 角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="73e47-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="73e47-121">属性</span><span class="sxs-lookup"><span data-stu-id="73e47-121">Properties</span></span>

| <span data-ttu-id="73e47-122">属性</span><span class="sxs-lookup"><span data-stu-id="73e47-122">Property</span></span>     | <span data-ttu-id="73e47-123">类型</span><span class="sxs-lookup"><span data-stu-id="73e47-123">Type</span></span>        | <span data-ttu-id="73e47-124">说明</span><span class="sxs-lookup"><span data-stu-id="73e47-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73e47-125">id</span><span class="sxs-lookup"><span data-stu-id="73e47-125">id</span></span>|<span data-ttu-id="73e47-126">String</span><span class="sxs-lookup"><span data-stu-id="73e47-126">String</span></span>| <span data-ttu-id="73e47-127">只读。</span><span class="sxs-lookup"><span data-stu-id="73e47-127">Read-only.</span></span> <span data-ttu-id="73e47-128">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="73e47-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="73e47-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="73e47-129">assignmentState</span></span>|<span data-ttu-id="73e47-130">String</span><span class="sxs-lookup"><span data-stu-id="73e47-130">String</span></span>| <span data-ttu-id="73e47-131">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="73e47-131">The state of the assignment.</span></span> <span data-ttu-id="73e47-132">值可以是`Eligible`合格分配`Active`-如果直接分配`Active`由管理员、 或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="73e47-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="73e47-133">duration</span><span class="sxs-lookup"><span data-stu-id="73e47-133">duration</span></span>|<span data-ttu-id="73e47-134">String</span><span class="sxs-lookup"><span data-stu-id="73e47-134">String</span></span>| <span data-ttu-id="73e47-135">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="73e47-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="73e47-136">Reason</span><span class="sxs-lookup"><span data-stu-id="73e47-136">reason</span></span>|<span data-ttu-id="73e47-137">String</span><span class="sxs-lookup"><span data-stu-id="73e47-137">String</span></span>| <span data-ttu-id="73e47-138">角色分配原因。</span><span class="sxs-lookup"><span data-stu-id="73e47-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="73e47-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="73e47-139">requestedDateTime</span></span>|<span data-ttu-id="73e47-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73e47-140">DateTimeOffset</span></span>| <span data-ttu-id="73e47-141">只读。</span><span class="sxs-lookup"><span data-stu-id="73e47-141">Read-only.</span></span> <span data-ttu-id="73e47-142">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="73e47-142">The request create time.</span></span> <span data-ttu-id="73e47-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="73e47-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73e47-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="73e47-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="73e47-145">roleId</span><span class="sxs-lookup"><span data-stu-id="73e47-145">roleId</span></span>|<span data-ttu-id="73e47-146">String</span><span class="sxs-lookup"><span data-stu-id="73e47-146">String</span></span>| <span data-ttu-id="73e47-147">角色的 id。</span><span class="sxs-lookup"><span data-stu-id="73e47-147">The id of the role.</span></span>|
|<span data-ttu-id="73e47-148">Schedule</span><span class="sxs-lookup"><span data-stu-id="73e47-148">schedule</span></span>|[<span data-ttu-id="73e47-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="73e47-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="73e47-150">角色分配请求的计划对象。</span><span class="sxs-lookup"><span data-stu-id="73e47-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="73e47-151">status</span><span class="sxs-lookup"><span data-stu-id="73e47-151">status</span></span>|<span data-ttu-id="73e47-152">String</span><span class="sxs-lookup"><span data-stu-id="73e47-152">String</span></span>| <span data-ttu-id="73e47-153">读取 only.The 角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="73e47-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="73e47-154">值可以是`NotStarted`，`Completed`，`RequestedApproval`，`Scheduled`，`Approved`，`ApprovalDenied`，`ApprovalAborted`，`Cancelling`，`Cancelled`，`Revoked`，`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="73e47-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="73e47-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="73e47-155">ticketNumber</span></span>|<span data-ttu-id="73e47-156">String</span><span class="sxs-lookup"><span data-stu-id="73e47-156">String</span></span>| <span data-ttu-id="73e47-157">角色分配 ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="73e47-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="73e47-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="73e47-158">ticketSystem</span></span>|<span data-ttu-id="73e47-159">String</span><span class="sxs-lookup"><span data-stu-id="73e47-159">String</span></span>| <span data-ttu-id="73e47-160">角色分配 ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="73e47-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="73e47-161">type</span><span class="sxs-lookup"><span data-stu-id="73e47-161">type</span></span>|<span data-ttu-id="73e47-162">字符串</span><span class="sxs-lookup"><span data-stu-id="73e47-162">String</span></span>| <span data-ttu-id="73e47-163">表示的角色分配操作的类型。</span><span class="sxs-lookup"><span data-stu-id="73e47-163">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="73e47-164">值可以是`AdminAdd`： 管理员将用户添加到角色;`UserAdd`： 用户将添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="73e47-164">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="73e47-165">userId</span><span class="sxs-lookup"><span data-stu-id="73e47-165">userId</span></span>|<span data-ttu-id="73e47-166">String</span><span class="sxs-lookup"><span data-stu-id="73e47-166">String</span></span>| <span data-ttu-id="73e47-167">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="73e47-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73e47-168">关系</span><span class="sxs-lookup"><span data-stu-id="73e47-168">Relationships</span></span>
| <span data-ttu-id="73e47-169">关系</span><span class="sxs-lookup"><span data-stu-id="73e47-169">Relationship</span></span> | <span data-ttu-id="73e47-170">类型</span><span class="sxs-lookup"><span data-stu-id="73e47-170">Type</span></span>        | <span data-ttu-id="73e47-171">说明</span><span class="sxs-lookup"><span data-stu-id="73e47-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73e47-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="73e47-172">roleInfo</span></span>|[<span data-ttu-id="73e47-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="73e47-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="73e47-174">角色分配请求 roleInfo 对象。</span><span class="sxs-lookup"><span data-stu-id="73e47-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73e47-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73e47-175">JSON representation</span></span>

<span data-ttu-id="73e47-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73e47-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
