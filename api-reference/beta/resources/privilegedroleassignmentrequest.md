---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示 Privilegd Identity Management 中角色分配操作的请求。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: a22049c1f3de095e7146a1e9cd901db8d6f5fd6a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398852"
---
# <a name="privilegedroleassignmentrequest-resource-type-deprecated"></a>privilegedRoleAssignmentRequest 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

表示Privileged Identity Management (PIM) 中角色分配操作的请求。

`privilegedRoleAssignmentRequest` 是票证建模实体，用于管理角色分配的生命周期。 它表示用户和管理员的意图/决策，也提供了实现定期架构、审批门等的灵活性，与直接公开`POST`和`LIST`操作`MY``Cancel`以及函`governanceRoleAssignment`数相比。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  集合|列出角色分配请求。|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|创建一个请求来管理现有或新角色分配的生命周期。|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |取消挂起的角色分配请求。|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |获取当前 requstor 的角色分配请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。 角色分配请求的 ID。|
|assignmentState|字符串| 分配的状态。 如果该值`Eligible`是管理员直接分配`Active`的，也可以是针对符合条件的分配`Active`激活的，或者由用户在符合条件的分配上激活。|
|duration|String| 角色分配的持续时间。|
|reason|字符串| 角色分配的原因。|
|requestedDateTime|DateTimeOffset| 只读。 请求创建时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|roleId|String| 角色的 ID。|
|schedule|[governanceSchedule](governanceschedule.md)| 角色分配请求的计划对象。|
|status|String| 只读。角色分配请求的状态。 值可以是 `NotStarted`，，，`RequestedApproval`，`Scheduled`，`Approved`，`ApprovalDenied`，`ApprovalAborted`，`Cancelling``Cancelled`，，`Revoked`。`RequestExpired``Completed`|
|ticketNumber|字符串| 角色分配的票证编号。 |
|ticketSystem|String| 角色分配的 ticketSystem。|
|type|字符串| 表示角色分配上的操作的类型。 值可以是 `AdminAdd`：管理员将用户添加到角色;`UserAdd`：用户添加角色分配。|
|userId|字符串| 用户的 ID。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| 角色分配请求的 roleInfo 对象。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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


