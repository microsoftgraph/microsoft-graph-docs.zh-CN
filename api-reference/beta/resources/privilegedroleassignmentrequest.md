---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理中对角色分配操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 881f5e47d7a441a297c21a0463e49496aeaf7a07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965731"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a><span data-ttu-id="04762-103">privilegedRoleAssignmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="04762-103">privilegedRoleAssignmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04762-104">表示在 Privilegd 标识管理中对角色分配操作的请求。</span><span class="sxs-lookup"><span data-stu-id="04762-104">Represents the request for role assignment operations in Privilegd Identity Management.</span></span>

<span data-ttu-id="04762-105">`privilegedRoleAssignmentRequest`是用于管理角色分配生命周期的票据建模实体。</span><span class="sxs-lookup"><span data-stu-id="04762-105">`privilegedRoleAssignmentRequest` is a ticket-modeled entity used to manage the lifecycle of role assignments.</span></span> <span data-ttu-id="04762-106">它表示用户和管理员的意向/决定, 还提供了灵活性, 可实现定期 schduling、审批门等, 与直接公开`POST`和`LIST`运营以及`MY`和`Cancel`函数`governanceRoleAssignment`。</span><span class="sxs-lookup"><span data-stu-id="04762-106">It represents the intention/decision of the users and administrators, and also provides the flexibility to enable implementation of recurrent schduling, approval gates, and so on, as compared to directly exposing `POST` and `LIST` operations as well as `MY` and `Cancel` functions on `governanceRoleAssignment`.</span></span>

## <a name="methods"></a><span data-ttu-id="04762-107">方法</span><span class="sxs-lookup"><span data-stu-id="04762-107">Methods</span></span>

| <span data-ttu-id="04762-108">方法</span><span class="sxs-lookup"><span data-stu-id="04762-108">Method</span></span>       | <span data-ttu-id="04762-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="04762-109">Return Type</span></span> | <span data-ttu-id="04762-110">说明</span><span class="sxs-lookup"><span data-stu-id="04762-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="04762-111">List</span><span class="sxs-lookup"><span data-stu-id="04762-111">List</span></span>](../api/privilegedroleassignmentrequest-list.md) | <span data-ttu-id="04762-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="04762-112">[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  collection</span></span>|<span data-ttu-id="04762-113">列出角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="04762-113">List role assignment requests.</span></span>|
|[<span data-ttu-id="04762-114">创建</span><span class="sxs-lookup"><span data-stu-id="04762-114">Create</span></span>](../api/privilegedroleassignmentrequest-post.md)|  [<span data-ttu-id="04762-115">privilegedroleassignmentrequest</span><span class="sxs-lookup"><span data-stu-id="04762-115">privilegedroleassignmentrequest</span></span>](../resources/privilegedroleassignmentrequest.md)|<span data-ttu-id="04762-116">创建一个请求, 以管理现有或新角色分配的生命周期。</span><span class="sxs-lookup"><span data-stu-id="04762-116">Create a request to manage the lifecycle of existing or new role assignment.</span></span>|
|[<span data-ttu-id="04762-117">Cancel</span><span class="sxs-lookup"><span data-stu-id="04762-117">Cancel</span></span>](../api/privilegedroleassignmentrequest-cancel.md)|  |<span data-ttu-id="04762-118">取消挂起的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="04762-118">Cancel a pending role assignment request.</span></span>|
|[<span data-ttu-id="04762-119">My</span><span class="sxs-lookup"><span data-stu-id="04762-119">My</span></span>](../api/privilegedroleassignmentrequest-my.md)|  |<span data-ttu-id="04762-120">获取当前 requstor 的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="04762-120">Get role assignment request for current requstor.</span></span>|

## <a name="properties"></a><span data-ttu-id="04762-121">属性</span><span class="sxs-lookup"><span data-stu-id="04762-121">Properties</span></span>

| <span data-ttu-id="04762-122">属性</span><span class="sxs-lookup"><span data-stu-id="04762-122">Property</span></span>     | <span data-ttu-id="04762-123">类型</span><span class="sxs-lookup"><span data-stu-id="04762-123">Type</span></span>        | <span data-ttu-id="04762-124">说明</span><span class="sxs-lookup"><span data-stu-id="04762-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04762-125">id</span><span class="sxs-lookup"><span data-stu-id="04762-125">id</span></span>|<span data-ttu-id="04762-126">String</span><span class="sxs-lookup"><span data-stu-id="04762-126">String</span></span>| <span data-ttu-id="04762-127">只读。</span><span class="sxs-lookup"><span data-stu-id="04762-127">Read-only.</span></span> <span data-ttu-id="04762-128">角色分配请求的 id。</span><span class="sxs-lookup"><span data-stu-id="04762-128">The id of the role assignment request.</span></span>|
|<span data-ttu-id="04762-129">assignmentState</span><span class="sxs-lookup"><span data-stu-id="04762-129">assignmentState</span></span>|<span data-ttu-id="04762-130">String</span><span class="sxs-lookup"><span data-stu-id="04762-130">String</span></span>| <span data-ttu-id="04762-131">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="04762-131">The state of the assignment.</span></span> <span data-ttu-id="04762-132">此值可`Eligible`用于符合条件的`Active`工作分配-如果是由`Active`管理员直接分配的, 或者是由用户的符合条件的工作分配激活的。</span><span class="sxs-lookup"><span data-stu-id="04762-132">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span>|
|<span data-ttu-id="04762-133">duration</span><span class="sxs-lookup"><span data-stu-id="04762-133">duration</span></span>|<span data-ttu-id="04762-134">String</span><span class="sxs-lookup"><span data-stu-id="04762-134">String</span></span>| <span data-ttu-id="04762-135">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="04762-135">The duration of a role assignment.</span></span>|
|<span data-ttu-id="04762-136">在于</span><span class="sxs-lookup"><span data-stu-id="04762-136">reason</span></span>|<span data-ttu-id="04762-137">String</span><span class="sxs-lookup"><span data-stu-id="04762-137">String</span></span>| <span data-ttu-id="04762-138">角色分配的原因。</span><span class="sxs-lookup"><span data-stu-id="04762-138">The reason for the role assignment.</span></span>|
|<span data-ttu-id="04762-139">requestedDateTime</span><span class="sxs-lookup"><span data-stu-id="04762-139">requestedDateTime</span></span>|<span data-ttu-id="04762-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04762-140">DateTimeOffset</span></span>| <span data-ttu-id="04762-141">只读。</span><span class="sxs-lookup"><span data-stu-id="04762-141">Read-only.</span></span> <span data-ttu-id="04762-142">请求创建时间。</span><span class="sxs-lookup"><span data-stu-id="04762-142">The request create time.</span></span> <span data-ttu-id="04762-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="04762-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="04762-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="04762-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="04762-145">roleId</span><span class="sxs-lookup"><span data-stu-id="04762-145">roleId</span></span>|<span data-ttu-id="04762-146">String</span><span class="sxs-lookup"><span data-stu-id="04762-146">String</span></span>| <span data-ttu-id="04762-147">角色的 id。</span><span class="sxs-lookup"><span data-stu-id="04762-147">The id of the role.</span></span>|
|<span data-ttu-id="04762-148">schedule</span><span class="sxs-lookup"><span data-stu-id="04762-148">schedule</span></span>|[<span data-ttu-id="04762-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="04762-149">governanceSchedule</span></span>](governanceschedule.md)| <span data-ttu-id="04762-150">角色分配请求的 schedule 对象。</span><span class="sxs-lookup"><span data-stu-id="04762-150">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="04762-151">status</span><span class="sxs-lookup"><span data-stu-id="04762-151">status</span></span>|<span data-ttu-id="04762-152">String</span><span class="sxs-lookup"><span data-stu-id="04762-152">String</span></span>| <span data-ttu-id="04762-153">只读。角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="04762-153">Read-only.The status of the role assignment request.</span></span> <span data-ttu-id="04762-154">值可以是`NotStarted``Completed`、、`RequestedApproval``Scheduled``Approved``ApprovalDenied``Revoked``RequestExpired`、、、、、、、、。`ApprovalAborted``Cancelling``Cancelled`</span><span class="sxs-lookup"><span data-stu-id="04762-154">The value can be `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.</span></span>|
|<span data-ttu-id="04762-155">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="04762-155">ticketNumber</span></span>|<span data-ttu-id="04762-156">String</span><span class="sxs-lookup"><span data-stu-id="04762-156">String</span></span>| <span data-ttu-id="04762-157">角色分配的 ticketNumber。</span><span class="sxs-lookup"><span data-stu-id="04762-157">The ticketNumber for the role assignment.</span></span> |
|<span data-ttu-id="04762-158">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="04762-158">ticketSystem</span></span>|<span data-ttu-id="04762-159">String</span><span class="sxs-lookup"><span data-stu-id="04762-159">String</span></span>| <span data-ttu-id="04762-160">角色分配的 ticketSystem。</span><span class="sxs-lookup"><span data-stu-id="04762-160">The ticketSystem for the role assignment.</span></span>|
|<span data-ttu-id="04762-161">type</span><span class="sxs-lookup"><span data-stu-id="04762-161">type</span></span>|<span data-ttu-id="04762-162">字符串</span><span class="sxs-lookup"><span data-stu-id="04762-162">String</span></span>| <span data-ttu-id="04762-163">表示角色分配上操作的类型。</span><span class="sxs-lookup"><span data-stu-id="04762-163">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="04762-164">值可以是`AdminAdd`: Administrators 将用户添加到角色;`UserAdd`: 用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="04762-164">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span>|
|<span data-ttu-id="04762-165">userId</span><span class="sxs-lookup"><span data-stu-id="04762-165">userId</span></span>|<span data-ttu-id="04762-166">String</span><span class="sxs-lookup"><span data-stu-id="04762-166">String</span></span>| <span data-ttu-id="04762-167">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="04762-167">The id of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04762-168">关系</span><span class="sxs-lookup"><span data-stu-id="04762-168">Relationships</span></span>
| <span data-ttu-id="04762-169">关系</span><span class="sxs-lookup"><span data-stu-id="04762-169">Relationship</span></span> | <span data-ttu-id="04762-170">类型</span><span class="sxs-lookup"><span data-stu-id="04762-170">Type</span></span>        | <span data-ttu-id="04762-171">说明</span><span class="sxs-lookup"><span data-stu-id="04762-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04762-172">roleInfo</span><span class="sxs-lookup"><span data-stu-id="04762-172">roleInfo</span></span>|[<span data-ttu-id="04762-173">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="04762-173">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="04762-174">角色分配请求的 roleInfo 对象。</span><span class="sxs-lookup"><span data-stu-id="04762-174">The roleInfo object of the role assignment request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04762-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04762-175">JSON representation</span></span>

<span data-ttu-id="04762-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04762-176">The following is a JSON representation of the resource.</span></span>

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
