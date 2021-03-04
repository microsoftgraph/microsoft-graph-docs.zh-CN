---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在"角色分配 Identity Management"中执行所有操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2a976632c038f87a1a3e09c3683ebcdd6d448b35
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443998"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="0972f-103">privilegedRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="0972f-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="0972f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0972f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0972f-105">表示在"角色分配 Identity Management"中执行所有操作的请求。</span><span class="sxs-lookup"><span data-stu-id="0972f-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="0972f-106">`privilegedRoleAssignmentRequest` 是一个票证模型实体，用于管理角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="0972f-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="0972f-107">它表示用户和管理员的意图/决定，还提供了实现反复选择、审批入口等的灵活性，与直接公开和操作以及操作以及功能相比 `POST` `LIST` `MY` `Cancel` `governanceRoleAssignment` 。</span><span class="sxs-lookup"><span data-stu-id="0972f-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="0972f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="0972f-108">Methods</span></span>

| <span data-ttu-id="0972f-109">方法</span><span class="sxs-lookup"><span data-stu-id="0972f-109">Method</span></span>       | <span data-ttu-id="0972f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0972f-110">Return Type</span></span> | <span data-ttu-id="0972f-111">Description</span><span class="sxs-lookup"><span data-stu-id="0972f-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="0972f-112">List</span><span class="sxs-lookup"><span data-stu-id="0972f-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="0972f-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  集合</span><span class="sxs-lookup"><span data-stu-id="0972f-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="0972f-114">列出角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="0972f-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="0972f-115">创建</span><span class="sxs-lookup"><span data-stu-id="0972f-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="0972f-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="0972f-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="0972f-117">创建一个请求，以管理现有或新数据库的角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="0972f-118">Cancel</span><span class="sxs-lookup"><span data-stu-id="0972f-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="0972f-119">取消挂起角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="0972f-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="0972f-120">My</span><span class="sxs-lookup"><span data-stu-id="0972f-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="0972f-121">获取角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="0972f-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="0972f-122">属性</span><span class="sxs-lookup"><span data-stu-id="0972f-122">Properties</span></span>

| <span data-ttu-id="0972f-123">属性</span><span class="sxs-lookup"><span data-stu-id="0972f-123">Property</span></span>     | <span data-ttu-id="0972f-124">类型</span><span class="sxs-lookup"><span data-stu-id="0972f-124">Type</span></span>        | <span data-ttu-id="0972f-125">说明</span><span class="sxs-lookup"><span data-stu-id="0972f-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0972f-126">id</span><span class="sxs-lookup"><span data-stu-id="0972f-126">id</span></span>|<span data-ttu-id="0972f-127">String</span><span class="sxs-lookup"><span data-stu-id="0972f-127">String</span></span>| <span data-ttu-id="0972f-128">只读。</span><span class="sxs-lookup"><span data-stu-id="0972f-128">Read-only.</span></span> <span data-ttu-id="0972f-129">请求角色分配 ID。</span><span class="sxs-lookup"><span data-stu-id="0972f-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="0972f-130">assignmentState</span><span class="sxs-lookup"><span data-stu-id="0972f-130">assignmentState</span></span>|<span data-ttu-id="0972f-131">String</span><span class="sxs-lookup"><span data-stu-id="0972f-131">String</span></span>| <span data-ttu-id="0972f-132">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="0972f-132">The state of the assignment.</span></span> <span data-ttu-id="0972f-133">该值可用于符合条件的分配-如果直接由管理员分配，或由用户激活在符合条件的分配 `Eligible` `Active` `Active` 上。</span><span class="sxs-lookup"><span data-stu-id="0972f-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="0972f-134">duration</span><span class="sxs-lookup"><span data-stu-id="0972f-134">duration</span></span>|<span data-ttu-id="0972f-135">String</span><span class="sxs-lookup"><span data-stu-id="0972f-135">String</span></span>| <span data-ttu-id="0972f-136">任务的持续时间角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="0972f-137">reason</span><span class="sxs-lookup"><span data-stu-id="0972f-137">reason</span></span>|<span data-ttu-id="0972f-138">String</span><span class="sxs-lookup"><span data-stu-id="0972f-138">String</span></span>| <span data-ttu-id="0972f-139">导致角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="0972f-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="0972f-140">requestedDateTime</span></span>|<span data-ttu-id="0972f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0972f-141">DateTimeOffset</span></span>| <span data-ttu-id="0972f-142">只读。</span><span class="sxs-lookup"><span data-stu-id="0972f-142">Read-only.</span></span> <span data-ttu-id="0972f-143">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="0972f-143">The request create time.</span></span> <span data-ttu-id="0972f-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0972f-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0972f-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0972f-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0972f-146">roleId</span><span class="sxs-lookup"><span data-stu-id="0972f-146">roleId</span></span>|<span data-ttu-id="0972f-147">String</span><span class="sxs-lookup"><span data-stu-id="0972f-147">String</span></span>| <span data-ttu-id="0972f-148">角色的 ID。</span><span class="sxs-lookup"><span data-stu-id="0972f-148">The id of the role.</span></span>|
|<span data-ttu-id="0972f-149">schedule</span><span class="sxs-lookup"><span data-stu-id="0972f-149">schedule</span></span>|[<span data-ttu-id="0972f-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0972f-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="0972f-151">请求的计划角色分配对象。</span><span class="sxs-lookup"><span data-stu-id="0972f-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="0972f-152">status</span><span class="sxs-lookup"><span data-stu-id="0972f-152">status</span></span>|<span data-ttu-id="0972f-153">String</span><span class="sxs-lookup"><span data-stu-id="0972f-153">String</span></span>| <span data-ttu-id="0972f-154">只读。请求角色分配状态。</span><span class="sxs-lookup"><span data-stu-id="0972f-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="0972f-155">值可以是 `NotStarted` ， `Completed` ， ， ， ， `RequestedApproval` ， ， ， `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` 。</span><span class="sxs-lookup"><span data-stu-id="0972f-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="0972f-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="0972f-156">ticketNumber</span></span>|<span data-ttu-id="0972f-157">String</span><span class="sxs-lookup"><span data-stu-id="0972f-157">String</span></span>| <span data-ttu-id="0972f-158">票证的 ticketNumber 角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="0972f-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="0972f-159">ticketSystem</span></span>|<span data-ttu-id="0972f-160">String</span><span class="sxs-lookup"><span data-stu-id="0972f-160">String</span></span>| <span data-ttu-id="0972f-161">用于此角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="0972f-162">type</span><span class="sxs-lookup"><span data-stu-id="0972f-162">type</span></span>|<span data-ttu-id="0972f-163">String</span><span class="sxs-lookup"><span data-stu-id="0972f-163">String</span></span>| <span data-ttu-id="0972f-164">表示对象上的操作角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="0972f-165">值可以是 `AdminAdd` ：管理员将用户添加到角色 `UserAdd` ;：用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="0972f-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="0972f-166">userId</span><span class="sxs-lookup"><span data-stu-id="0972f-166">userId</span></span>|<span data-ttu-id="0972f-167">String</span><span class="sxs-lookup"><span data-stu-id="0972f-167">String</span></span>| <span data-ttu-id="0972f-168">用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="0972f-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0972f-169">关系</span><span class="sxs-lookup"><span data-stu-id="0972f-169">Relationships</span></span>
| <span data-ttu-id="0972f-170">关系</span><span class="sxs-lookup"><span data-stu-id="0972f-170">Relationship</span></span> | <span data-ttu-id="0972f-171">类型</span><span class="sxs-lookup"><span data-stu-id="0972f-171">Type</span></span>        | <span data-ttu-id="0972f-172">说明</span><span class="sxs-lookup"><span data-stu-id="0972f-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0972f-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="0972f-173">roleInfo</span></span>|[<span data-ttu-id="0972f-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="0972f-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="0972f-175">请求的 roleInfo 角色分配对象。</span><span class="sxs-lookup"><span data-stu-id="0972f-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0972f-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0972f-176">JSON representation</span></span>

<span data-ttu-id="0972f-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0972f-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->


