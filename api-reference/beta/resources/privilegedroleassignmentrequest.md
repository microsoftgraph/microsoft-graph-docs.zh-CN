---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理角色分配操作的请求。
localization_priority: Normal
ms.openlocfilehash: bfe3b6802136b2848f36abef08134efd0eb82518
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880127"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="2bd4f-103">privilegedRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bd4f-103">privilegedRoleAssignmentRequest resource type</span></span>

> <span data-ttu-id="2bd4f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bd4f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bd4f-106">表示在 Privilegd 标识管理角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-106">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="2bd4f-107">`privilegedRoleAssignmentRequest`用于管理角色分配的生命周期的票证建模的实体。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-107">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="2bd4f-108">它表示意图/决策的用户和管理员，并且还提供灵活地启用实施定期 schduling、 审批入口和等等，与直接公开`POST`和`LIST`操作以及`MY`和`Cancel`函数上`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-108">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="2bd4f-109">方法</span><span class="sxs-lookup"><span data-stu-id="2bd4f-109">Methods</span></span>

| <span data-ttu-id="2bd4f-110">方法</span><span class="sxs-lookup"><span data-stu-id="2bd4f-110">Method</span></span>       | <span data-ttu-id="2bd4f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2bd4f-111">Return Type</span></span> | <span data-ttu-id="2bd4f-112">说明</span><span class="sxs-lookup"><span data-stu-id="2bd4f-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="2bd4f-113">List</span><span class="sxs-lookup"><span data-stu-id="2bd4f-113">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="2bd4f-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="2bd4f-114">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="2bd4f-115">列出角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-115">List role assignment requests.</span></span>|
|[<span data-ttu-id="2bd4f-116">Create</span><span class="sxs-lookup"><span data-stu-id="2bd4f-116">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="2bd4f-117">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="2bd4f-117">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="2bd4f-118">创建管理现有或新角色分配的生命周期的请求。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-118">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="2bd4f-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="2bd4f-119">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="2bd4f-120">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-120">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="2bd4f-121">My</span><span class="sxs-lookup"><span data-stu-id="2bd4f-121">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="2bd4f-122">获取当前 requstor 角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-122">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="2bd4f-123">属性</span><span class="sxs-lookup"><span data-stu-id="2bd4f-123">Properties</span></span>

| <span data-ttu-id="2bd4f-124">属性</span><span class="sxs-lookup"><span data-stu-id="2bd4f-124">Property</span></span>     | <span data-ttu-id="2bd4f-125">类型</span><span class="sxs-lookup"><span data-stu-id="2bd4f-125">Type</span></span>        | <span data-ttu-id="2bd4f-126">说明</span><span class="sxs-lookup"><span data-stu-id="2bd4f-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bd4f-127">id</span><span class="sxs-lookup"><span data-stu-id="2bd4f-127">id</span></span>|<span data-ttu-id="2bd4f-128">String</span><span class="sxs-lookup"><span data-stu-id="2bd4f-128">String</span></span>| <span data-ttu-id="2bd4f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-129">Read-only.</span></span> <span data-ttu-id="2bd4f-130">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-130">The id of the role assignment request.</span></span>|
|<span data-ttu-id="2bd4f-131">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2bd4f-131">assignmentState</span></span>|<span data-ttu-id="2bd4f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-132">String</span></span>| <span data-ttu-id="2bd4f-133">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-133">The state of the assignment.</span></span> <span data-ttu-id="2bd4f-134">值可以是`Eligible`合格分配`Active`-如果直接分配`Active`由管理员、 或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-134">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="2bd4f-135">duration</span><span class="sxs-lookup"><span data-stu-id="2bd4f-135">duration</span></span>|<span data-ttu-id="2bd4f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-136">String</span></span>| <span data-ttu-id="2bd4f-137">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-137">The duration of a role assignment.</span></span>|
|<span data-ttu-id="2bd4f-138">原因</span><span class="sxs-lookup"><span data-stu-id="2bd4f-138">reason</span></span>|<span data-ttu-id="2bd4f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-139">String</span></span>| <span data-ttu-id="2bd4f-140">角色分配原因。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-140">The reason for the role assignment.</span></span>|
|<span data-ttu-id="2bd4f-141">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bd4f-141">requestedDateTime</span></span>|<span data-ttu-id="2bd4f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bd4f-142">DateTimeOffset</span></span>| <span data-ttu-id="2bd4f-143">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-143">Read-only.</span></span> <span data-ttu-id="2bd4f-144">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-144">The request create time.</span></span> <span data-ttu-id="2bd4f-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2bd4f-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2bd4f-147">roleId</span><span class="sxs-lookup"><span data-stu-id="2bd4f-147">roleId</span></span>|<span data-ttu-id="2bd4f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-148">String</span></span>| <span data-ttu-id="2bd4f-149">角色的 id。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-149">The id of the role.</span></span>|
|<span data-ttu-id="2bd4f-150">计划</span><span class="sxs-lookup"><span data-stu-id="2bd4f-150">schedule</span></span>|[<span data-ttu-id="2bd4f-151">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2bd4f-151">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="2bd4f-152">角色分配请求的计划对象。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-152">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="2bd4f-153">status</span><span class="sxs-lookup"><span data-stu-id="2bd4f-153">status</span></span>|<span data-ttu-id="2bd4f-154">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-154">String</span></span>| <span data-ttu-id="2bd4f-155">读取 only.The 角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-155">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="2bd4f-156">值可以是`NotStarted`，`Completed`，`RequestedApproval`，`Scheduled`，`Approved`，`ApprovalDenied`，`ApprovalAborted`，`Cancelling`，`Cancelled`，`Revoked`，`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-156">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="2bd4f-157">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="2bd4f-157">ticketNumber</span></span>|<span data-ttu-id="2bd4f-158">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-158">String</span></span>| <span data-ttu-id="2bd4f-159">角色分配 ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-159">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="2bd4f-160">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="2bd4f-160">ticketSystem</span></span>|<span data-ttu-id="2bd4f-161">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-161">String</span></span>| <span data-ttu-id="2bd4f-162">角色分配 ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-162">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="2bd4f-163">type</span><span class="sxs-lookup"><span data-stu-id="2bd4f-163">type</span></span>|<span data-ttu-id="2bd4f-164">字符串</span><span class="sxs-lookup"><span data-stu-id="2bd4f-164">String</span></span>| <span data-ttu-id="2bd4f-165">表示的角色分配操作的类型。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-165">Representing the the type of the operation on the role assignment.</span></span> <span data-ttu-id="2bd4f-166">值可以是`AdminAdd`： 管理员将用户添加到角色;`UserAdd`： 用户将添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-166">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="2bd4f-167">userId</span><span class="sxs-lookup"><span data-stu-id="2bd4f-167">userId</span></span>|<span data-ttu-id="2bd4f-168">String</span><span class="sxs-lookup"><span data-stu-id="2bd4f-168">String</span></span>| <span data-ttu-id="2bd4f-169">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-169">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bd4f-170">Relationships</span><span class="sxs-lookup"><span data-stu-id="2bd4f-170">Relationships</span></span>
| <span data-ttu-id="2bd4f-171">关系</span><span class="sxs-lookup"><span data-stu-id="2bd4f-171">Relationship</span></span> | <span data-ttu-id="2bd4f-172">类型</span><span class="sxs-lookup"><span data-stu-id="2bd4f-172">Type</span></span>        | <span data-ttu-id="2bd4f-173">Description</span><span class="sxs-lookup"><span data-stu-id="2bd4f-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bd4f-174">roleInfo</span><span class="sxs-lookup"><span data-stu-id="2bd4f-174">roleInfo</span></span>|[<span data-ttu-id="2bd4f-175">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="2bd4f-175">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="2bd4f-176">角色分配请求 roleInfo 对象。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-176">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bd4f-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bd4f-177">JSON representation</span></span>

<span data-ttu-id="2bd4f-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bd4f-178">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
