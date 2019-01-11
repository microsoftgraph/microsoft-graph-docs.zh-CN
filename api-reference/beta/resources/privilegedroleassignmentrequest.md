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
# <a name="privilegedroleassignmentrequest-resource-type"></a>privilegedRoleAssignmentRequest 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示在 Privilegd 标识管理角色分配操作的请求。

`privilegedRoleAssignmentRequest`用于管理角色分配的生命周期的票证建模的实体。 它表示意图/决策的用户和管理员，并且还提供灵活地启用实施定期 schduling、 审批入口和等等，与直接公开`POST`和`LIST`操作以及`MY`和`Cancel`函数上`governanceRoleAssignment`。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)集合|列出角色分配请求。|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|创建管理现有或新角色分配的生命周期的请求。|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |取消挂起的角色分配请求。|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |获取当前 requstor 角色分配请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。 角色分配请求的 id。|
|assignmentState|字符串| 工作分配状态。 值可以是`Eligible`合格分配`Active`-如果直接分配`Active`由管理员、 或激活合格工作分配的用户。|
|duration|字符串| 角色分配的持续时间。|
|原因|字符串| 角色分配原因。|
|requestedDateTime|DateTimeOffset| 此为只读属性。 请求创建时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|roleId|字符串| 角色的 id。|
|计划|[governanceSchedule](governanceschedule.md)| 角色分配请求的计划对象。|
|status|字符串| 读取 only.The 角色分配请求的状态。 值可以是`NotStarted`，`Completed`，`RequestedApproval`，`Scheduled`，`Approved`，`ApprovalDenied`，`ApprovalAborted`，`Cancelling`，`Cancelled`，`Revoked`，`RequestExpired`。|
|ticketNumber|字符串| 角色分配 ticketNumber。 |
|ticketSystem|字符串| 角色分配 ticketSystem。|
|type|字符串| 表示的角色分配操作的类型。 值可以是`AdminAdd`： 管理员将用户添加到角色;`UserAdd`： 用户将添加角色分配。|
|userId|String| 用户的 id。|

## <a name="relationships"></a>Relationships
| 关系 | 类型        | Description |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| 角色分配请求 roleInfo 对象。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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
