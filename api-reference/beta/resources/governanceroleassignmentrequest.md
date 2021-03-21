---
title: governanceRoleAssignmentRequest 资源类型
description: 代表在"角色分配 Identity Management"中执行安全操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e96a0009c6108a77383fe770a6351d7b64efd6f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961277"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>governanceRoleAssignmentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在"角色分配 Identity Management"中执行所有操作的请求。

`governanceRoleAssignmentRequest` 是一个票证模型实体，用于管理角色分配的生命周期。 它表示用户和管理员的意图/决定，并且提供了实现反复选择、审批入口等的灵活性，与直接公开 、 和 操作相比 `POST` `PUT` `DELETE` `governanceRoleAssignment` 。

## <a name="methods"></a>Methods

| 方法          |返回类型  |说明|
|:------------|:--------|:--------|
|[获取](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|获取角色分配 ID 指定的请求。  
|[列表](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  集合|获取角色分配请求。|
|[创建](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|创建管理现有或新数据库生命周期角色分配。|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |取消挂起角色分配请求。|
|[更新](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|如果请求的状态为 ，则管理员更新对请求的决策 `PendingAdminDecision` 。|

## <a name="properties"></a>属性
| 属性                  | 类型          |说明|
|:--------------------------|:--------------|:----------|
|id                         |String         |请求角色分配 ID。|
|resourceId                 |String         |必填。 与请求关联的角色分配的 ID。|
|roleDefinitionId           |String         |必填。 与请求关联的角色角色分配的 ID。|
|subjectId                  |String         |必填。 与请求关联的角色分配的 ID。|
|type                       |String        |必填。 表示对项目执行的操作角色分配。 可能的值是 `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminExtend` `UserRenew` ：、、、、。 `AdminRenew`|
|assignmentState|String  |必填。 工作分配的状态。 可能的值包括： (符合条件的分配) 、 (（如果管理员直接分配 `Eligible`  `Active`) 、 (或由用户) 在符合条件的分配上激活 `Active` ）。|
|requestedDateTime          |DateTimeOffset |只读。 请求创建时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|schedule                   |[governanceSchedule](governanceschedule.md)|请求的计划角色分配对象。|
|reason                     |String         |创建请求时由用户和管理员提供的消息，说明为什么需要该请求。|
|状态                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |请求角色分配状态。|
|linkedEligibleRoleAssignmentId|String        |如果这是角色激活请求，则它表示所引用 `eligible assignment` 的 ID;否则，值为 `null` 。 |

|成员|说明|
|:---|:---|
|AdminAdd|管理员将用户/组分配给角色。|
|UserAdd|用户激活符合条件的分配。|
|AdminUpdate|管理员更改现有角色分配。|
|AdminRemove|管理员从角色中删除用户/组。|
|UserRemove|用户停用活动分配。|
|UserExtend|用户请求延长其过期分配。|
|AdminExtend|管理员延长即将过期的工作分配。|
|UserRenew|用户请求续订其已过期的工作分配。|
|AdminRenew|管理员延长即将过期的工作分配。|



## <a name="relationships"></a>关系
| 关系 | 类型                                |说明|
|:-------------|:----------------------------------|:----------|
|资源      |[governanceResource](../resources/governanceresource.md)            |只读。 请求的目标资源。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 请求的目标角色定义。 |
|subject       |[governanceSubject](../resources/governancesubject.md)|只读。 用户/组主体。|

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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


