---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理中对角色分配操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c9ca647c7d2af82f76348fa737d15995d8a2ed96
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217895"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="e1f37-103">privilegedRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1f37-103">privilegedRoleAssignmentRequest resource type</span></span>

<span data-ttu-id="e1f37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1f37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1f37-105">表示在 Privilegd 标识管理中对角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="e1f37-105">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="e1f37-106">`privilegedRoleAssignmentRequest`是用于管理角色分配生命周期的票据建模实体。</span><span class="sxs-lookup"><span data-stu-id="e1f37-106">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="e1f37-107">它表示用户和管理员的意向/决定，还提供了灵活的功能，可以实现定期 schduling、审批门等，与直接`POST`公开和`LIST`运营以及`MY`和`Cancel`上的`governanceRoleAssignment`功能相比。</span><span class="sxs-lookup"><span data-stu-id="e1f37-107">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="e1f37-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e1f37-108">Methods</span></span>

| <span data-ttu-id="e1f37-109">方法</span><span class="sxs-lookup"><span data-stu-id="e1f37-109">Method</span></span>       | <span data-ttu-id="e1f37-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1f37-110">Return Type</span></span> | <span data-ttu-id="e1f37-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1f37-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="e1f37-112">List</span><span class="sxs-lookup"><span data-stu-id="e1f37-112">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="e1f37-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="e1f37-113">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="e1f37-114">列出角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="e1f37-114">List role assignment requests.</span></span>|
|[<span data-ttu-id="e1f37-115">创建</span><span class="sxs-lookup"><span data-stu-id="e1f37-115">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="e1f37-116">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="e1f37-116">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="e1f37-117">创建一个请求，以管理现有或新角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="e1f37-117">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="e1f37-118">Cancel</span><span class="sxs-lookup"><span data-stu-id="e1f37-118">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="e1f37-119">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="e1f37-119">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="e1f37-120">My</span><span class="sxs-lookup"><span data-stu-id="e1f37-120">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="e1f37-121">获取当前 requstor 的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="e1f37-121">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1f37-122">属性</span><span class="sxs-lookup"><span data-stu-id="e1f37-122">Properties</span></span>

| <span data-ttu-id="e1f37-123">属性</span><span class="sxs-lookup"><span data-stu-id="e1f37-123">Property</span></span>     | <span data-ttu-id="e1f37-124">类型</span><span class="sxs-lookup"><span data-stu-id="e1f37-124">Type</span></span>        | <span data-ttu-id="e1f37-125">说明</span><span class="sxs-lookup"><span data-stu-id="e1f37-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1f37-126">id</span><span class="sxs-lookup"><span data-stu-id="e1f37-126">id</span></span>|<span data-ttu-id="e1f37-127">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-127">String</span></span>| <span data-ttu-id="e1f37-128">只读。</span><span class="sxs-lookup"><span data-stu-id="e1f37-128">Read-only.</span></span> <span data-ttu-id="e1f37-129">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="e1f37-129">The id of the role assignment request.</span></span>|
|<span data-ttu-id="e1f37-130">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e1f37-130">assignmentState</span></span>|<span data-ttu-id="e1f37-131">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-131">String</span></span>| <span data-ttu-id="e1f37-132">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="e1f37-132">The state of the assignment.</span></span> <span data-ttu-id="e1f37-133">此值可`Eligible`用于符合条件的`Active`工作分配-如果是由`Active`管理员直接分配的，或者是由用户的符合条件的工作分配激活的。</span><span class="sxs-lookup"><span data-stu-id="e1f37-133">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="e1f37-134">duration</span><span class="sxs-lookup"><span data-stu-id="e1f37-134">duration</span></span>|<span data-ttu-id="e1f37-135">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-135">String</span></span>| <span data-ttu-id="e1f37-136">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="e1f37-136">The duration of a role assignment.</span></span>|
|<span data-ttu-id="e1f37-137">reason</span><span class="sxs-lookup"><span data-stu-id="e1f37-137">reason</span></span>|<span data-ttu-id="e1f37-138">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-138">String</span></span>| <span data-ttu-id="e1f37-139">角色分配的原因。</span><span class="sxs-lookup"><span data-stu-id="e1f37-139">The reason for the role assignment.</span></span>|
|<span data-ttu-id="e1f37-140">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1f37-140">requestedDateTime</span></span>|<span data-ttu-id="e1f37-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1f37-141">DateTimeOffset</span></span>| <span data-ttu-id="e1f37-142">只读。</span><span class="sxs-lookup"><span data-stu-id="e1f37-142">Read-only.</span></span> <span data-ttu-id="e1f37-143">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="e1f37-143">The request create time.</span></span> <span data-ttu-id="e1f37-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e1f37-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e1f37-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e1f37-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e1f37-146">roleId</span><span class="sxs-lookup"><span data-stu-id="e1f37-146">roleId</span></span>|<span data-ttu-id="e1f37-147">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-147">String</span></span>| <span data-ttu-id="e1f37-148">角色的 id。</span><span class="sxs-lookup"><span data-stu-id="e1f37-148">The id of the role.</span></span>|
|<span data-ttu-id="e1f37-149">schedule</span><span class="sxs-lookup"><span data-stu-id="e1f37-149">schedule</span></span>|[<span data-ttu-id="e1f37-150">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e1f37-150">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="e1f37-151">角色分配请求的 schedule 对象。</span><span class="sxs-lookup"><span data-stu-id="e1f37-151">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="e1f37-152">状态</span><span class="sxs-lookup"><span data-stu-id="e1f37-152">status</span></span>|<span data-ttu-id="e1f37-153">String</span><span class="sxs-lookup"><span data-stu-id="e1f37-153">String</span></span>| <span data-ttu-id="e1f37-154">只读。角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="e1f37-154">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="e1f37-155">值可以是`NotStarted``Completed`、、`RequestedApproval``Scheduled``Approved``ApprovalDenied``Revoked``RequestExpired`、、、、、、、、。`ApprovalAborted``Cancelling``Cancelled`</span><span class="sxs-lookup"><span data-stu-id="e1f37-155">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="e1f37-156">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="e1f37-156">ticketNumber</span></span>|<span data-ttu-id="e1f37-157">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-157">String</span></span>| <span data-ttu-id="e1f37-158">角色分配的 ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="e1f37-158">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="e1f37-159">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="e1f37-159">ticketSystem</span></span>|<span data-ttu-id="e1f37-160">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-160">String</span></span>| <span data-ttu-id="e1f37-161">角色分配的 ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="e1f37-161">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="e1f37-162">type</span><span class="sxs-lookup"><span data-stu-id="e1f37-162">type</span></span>|<span data-ttu-id="e1f37-163">字符串</span><span class="sxs-lookup"><span data-stu-id="e1f37-163">String</span></span>| <span data-ttu-id="e1f37-164">表示角色分配上操作的类型。</span><span class="sxs-lookup"><span data-stu-id="e1f37-164">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="e1f37-165">值可以是`AdminAdd`： Administrators 将用户添加到角色;`UserAdd`：用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="e1f37-165">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="e1f37-166">userId</span><span class="sxs-lookup"><span data-stu-id="e1f37-166">userId</span></span>|<span data-ttu-id="e1f37-167">String</span><span class="sxs-lookup"><span data-stu-id="e1f37-167">String</span></span>| <span data-ttu-id="e1f37-168">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="e1f37-168">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1f37-169">关系</span><span class="sxs-lookup"><span data-stu-id="e1f37-169">Relationships</span></span>
| <span data-ttu-id="e1f37-170">关系</span><span class="sxs-lookup"><span data-stu-id="e1f37-170">Relationship</span></span> | <span data-ttu-id="e1f37-171">类型</span><span class="sxs-lookup"><span data-stu-id="e1f37-171">Type</span></span>        | <span data-ttu-id="e1f37-172">说明</span><span class="sxs-lookup"><span data-stu-id="e1f37-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1f37-173">roleInfo</span><span class="sxs-lookup"><span data-stu-id="e1f37-173">roleInfo</span></span>|[<span data-ttu-id="e1f37-174">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="e1f37-174">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="e1f37-175">角色分配请求的 roleInfo 对象。</span><span class="sxs-lookup"><span data-stu-id="e1f37-175">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1f37-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1f37-176">JSON representation</span></span>

<span data-ttu-id="e1f37-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1f37-177">The following is a JSON representation of the resource.</span></span>

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
