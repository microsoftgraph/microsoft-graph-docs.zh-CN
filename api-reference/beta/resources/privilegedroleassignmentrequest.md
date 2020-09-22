---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理中对角色分配操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 5daeeee6f784c31f1e15843a8a1903ca41565118
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070508"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="f4b92-103">privilegedRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4b92-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="f4b92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b92-105">表示在 Privilegd 标识管理中对角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="f4b92-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="f4b92-106">`privilegedRoleAssignmentRequest` 是用于管理角色分配生命周期的票据建模实体。</span><span class="sxs-lookup"><span data-stu-id="f4b92-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="f4b92-107">它表示用户和管理员的意向/决定，还提供了灵活的功能，可以实现定期 schduling、审批门等，与直接公开 `POST` 和 `LIST` 运营以及 `MY` 和 `Cancel` 上的功能相比 `governanceRoleAssignment` 。</span><span class="sxs-lookup"><span data-stu-id="f4b92-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="f4b92-108">方法</span><span class="sxs-lookup"><span data-stu-id="f4b92-108">Methods</span></span>

| <span data-ttu-id="f4b92-109">方法</span><span class="sxs-lookup"><span data-stu-id="f4b92-109">Method</span></span>       | <span data-ttu-id="f4b92-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4b92-110">Return Type</span></span> | <span data-ttu-id="f4b92-111">Description</span><span class="sxs-lookup"><span data-stu-id="f4b92-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="f4b92-112">List</span><span class="sxs-lookup"><span data-stu-id="f4b92-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="f4b92-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  集合</span><span class="sxs-lookup"><span data-stu-id="f4b92-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="f4b92-114">列出角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f4b92-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="f4b92-115">Create</span><span class="sxs-lookup"><span data-stu-id="f4b92-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="f4b92-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="f4b92-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="f4b92-117">创建一个请求，以管理现有或新角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="f4b92-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="f4b92-118">Cancel</span><span class="sxs-lookup"><span data-stu-id="f4b92-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="f4b92-119">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f4b92-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="f4b92-120">My</span><span class="sxs-lookup"><span data-stu-id="f4b92-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="f4b92-121">获取当前 requstor 的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f4b92-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4b92-122">属性</span><span class="sxs-lookup"><span data-stu-id="f4b92-122">Properties</span></span>

| <span data-ttu-id="f4b92-123">属性</span><span class="sxs-lookup"><span data-stu-id="f4b92-123">Property</span></span>     | <span data-ttu-id="f4b92-124">类型</span><span class="sxs-lookup"><span data-stu-id="f4b92-124">Type</span></span>        | <span data-ttu-id="f4b92-125">说明</span><span class="sxs-lookup"><span data-stu-id="f4b92-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4b92-126">id</span><span class="sxs-lookup"><span data-stu-id="f4b92-126">id</span></span>|<span data-ttu-id="f4b92-127">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-127">String</span></span>| <span data-ttu-id="f4b92-128">只读。</span><span class="sxs-lookup"><span data-stu-id="f4b92-128">Read-only.</span></span> <span data-ttu-id="f4b92-129">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="f4b92-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="f4b92-130">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f4b92-130">assignmentState</span></span>|<span data-ttu-id="f4b92-131">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-131">String</span></span>| <span data-ttu-id="f4b92-132">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="f4b92-132">The state of the assignment.</span></span> <span data-ttu-id="f4b92-133">此值可 `Eligible` 用于符合条件的工作分配 `Active` -如果是由管理员直接分配的 `Active` ，或者是由用户的符合条件的工作分配激活的。</span><span class="sxs-lookup"><span data-stu-id="f4b92-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="f4b92-134">duration</span><span class="sxs-lookup"><span data-stu-id="f4b92-134">duration</span></span>|<span data-ttu-id="f4b92-135">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-135">String</span></span>| <span data-ttu-id="f4b92-136">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="f4b92-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="f4b92-137">reason</span><span class="sxs-lookup"><span data-stu-id="f4b92-137">reason</span></span>|<span data-ttu-id="f4b92-138">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-138">String</span></span>| <span data-ttu-id="f4b92-139">角色分配的原因。</span><span class="sxs-lookup"><span data-stu-id="f4b92-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="f4b92-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b92-140">requestedDateTime</span></span>|<span data-ttu-id="f4b92-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b92-141">DateTimeOffset</span></span>| <span data-ttu-id="f4b92-142">只读。</span><span class="sxs-lookup"><span data-stu-id="f4b92-142">Read-only.</span></span> <span data-ttu-id="f4b92-143">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="f4b92-143">The request create time.</span></span> <span data-ttu-id="f4b92-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f4b92-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4b92-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f4b92-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f4b92-146">roleId</span><span class="sxs-lookup"><span data-stu-id="f4b92-146">roleId</span></span>|<span data-ttu-id="f4b92-147">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-147">String</span></span>| <span data-ttu-id="f4b92-148">角色的 id。</span><span class="sxs-lookup"><span data-stu-id="f4b92-148">The id of the role.</span></span>|
|<span data-ttu-id="f4b92-149">schedule</span><span class="sxs-lookup"><span data-stu-id="f4b92-149">schedule</span></span>|[<span data-ttu-id="f4b92-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f4b92-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="f4b92-151">角色分配请求的 schedule 对象。</span><span class="sxs-lookup"><span data-stu-id="f4b92-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="f4b92-152">状态</span><span class="sxs-lookup"><span data-stu-id="f4b92-152">status</span></span>|<span data-ttu-id="f4b92-153">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-153">String</span></span>| <span data-ttu-id="f4b92-154">只读。角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="f4b92-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="f4b92-155">值可以是、、、、、、、、、 `NotStarted` `Completed` `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` 、 `RequestExpired` 。</span><span class="sxs-lookup"><span data-stu-id="f4b92-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="f4b92-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="f4b92-156">ticketNumber</span></span>|<span data-ttu-id="f4b92-157">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-157">String</span></span>| <span data-ttu-id="f4b92-158">角色分配的 ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="f4b92-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="f4b92-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="f4b92-159">ticketSystem</span></span>|<span data-ttu-id="f4b92-160">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-160">String</span></span>| <span data-ttu-id="f4b92-161">角色分配的 ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="f4b92-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="f4b92-162">type</span><span class="sxs-lookup"><span data-stu-id="f4b92-162">type</span></span>|<span data-ttu-id="f4b92-163">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-163">String</span></span>| <span data-ttu-id="f4b92-164">表示角色分配上操作的类型。</span><span class="sxs-lookup"><span data-stu-id="f4b92-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="f4b92-165">值可以是 `AdminAdd` ： Administrators 将用户添加到角色; `UserAdd` ：用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="f4b92-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="f4b92-166">userId</span><span class="sxs-lookup"><span data-stu-id="f4b92-166">userId</span></span>|<span data-ttu-id="f4b92-167">String</span><span class="sxs-lookup"><span data-stu-id="f4b92-167">String</span></span>| <span data-ttu-id="f4b92-168">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="f4b92-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4b92-169">关系</span><span class="sxs-lookup"><span data-stu-id="f4b92-169">Relationships</span></span>
| <span data-ttu-id="f4b92-170">关系</span><span class="sxs-lookup"><span data-stu-id="f4b92-170">Relationship</span></span> | <span data-ttu-id="f4b92-171">类型</span><span class="sxs-lookup"><span data-stu-id="f4b92-171">Type</span></span>        | <span data-ttu-id="f4b92-172">说明</span><span class="sxs-lookup"><span data-stu-id="f4b92-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4b92-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="f4b92-173">roleInfo</span></span>|[<span data-ttu-id="f4b92-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f4b92-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="f4b92-175">角色分配请求的 roleInfo 对象。</span><span class="sxs-lookup"><span data-stu-id="f4b92-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4b92-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4b92-176">JSON representation</span></span>

<span data-ttu-id="f4b92-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4b92-177">The following is a JSON representation of the resource.</span></span>

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


