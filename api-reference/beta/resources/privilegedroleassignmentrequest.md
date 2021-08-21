---
title: privilegedRoleAssignmentRequest 资源类型
description: 表示在"角色分配 Identity Management"中执行所有操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 59144fd6008e081eb6de29c94626fe5fb2c57af6
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454127"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>privilegedRoleAssignmentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在"角色分配 Identity Management"中执行所有操作的请求。

`privilegedRoleAssignmentRequest` 是一个票证模型实体，用于管理角色分配的生命周期。 它表示用户和管理员的意图/决定，并且提供了实现反复选择、审批入口等的灵活性，与直接公开和操作以及 上的功能 `POST` `LIST` `MY` `Cancel` 相比 `governanceRoleAssignment` 。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)  集合|列出角色分配请求。|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|创建管理现有或新数据库生命周期角色分配。|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |取消挂起角色分配请求。|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |获取角色分配当前 requstor 的请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。 请求角色分配 ID。|
|assignmentState|String| 工作分配的状态。 该值可用于符合条件的分配 - 如果直接由管理员分配，或由用户对符合条件的分配 `Eligible` `Active` `Active` 进行激活。|
|duration|String| 项目持续时间角色分配。|
|reason|String| 失败角色分配。|
|requestedDateTime|DateTimeOffset| 只读。 请求创建时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|roleId|字符串| 角色的 ID。|
|schedule|[governanceSchedule](governanceschedule.md)| 请求的计划角色分配对象。|
|状态|String| 只读。请求角色分配状态。 值可以是 `NotStarted` `Completed` `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` 、、、、、、、、。 `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired`|
|ticketNumber|字符串| 角色分配 的 ticketNumber。 |
|ticketSystem|字符串| 角色分配 的 ticketSystem。|
|type|字符串| 表示对项目执行的操作角色分配。 值可以是 `AdminAdd` ：管理员将用户添加到角色 `UserAdd` ;：用户添加角色分配。|
|userId|字符串| 用户的 ID。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| 请求的 roleInfo 角色分配。|

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


