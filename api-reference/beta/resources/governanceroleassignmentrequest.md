---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理角色分配操作的请求。
ms.openlocfilehash: 4b19ed04b4c78fa084c1247fc1798a39b08c3fdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041276"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>governanceRoleAssignmentRequest 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示在 Privilegd 标识管理角色分配操作的请求。

`governanceRoleAssignmentRequest`用于管理角色分配的生命周期的票证建模的实体。 它表示意图/决策的用户和管理员，并且还提供灵活地启用实施定期 schduling、 审批入口和等等，与直接公开`POST`， `PUT`，和`DELETE`操作在`governanceRoleAssignment`。

## <a name="methods"></a>方法

| 方法          |返回类型  |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|获取由 ID 指定的角色分配请求  
|[List](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合|获取角色分配请求的资源。|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|创建管理现有或新角色分配的生命周期的请求。|
|[取消](../api/governanceroleassignmentrequest-cancel.md)|  |取消挂起的角色分配请求。|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|如果请求中的状态，管理员更新对请求的决策`PendingAdminDecision`。|

## <a name="properties"></a>属性
| 属性                  | 类型          |说明|
|:--------------------------|:--------------|:----------|
|id                         |字符串         |角色分配请求的 id。|
|resourceId                 |String         |必需项。 与关联的角色分配请求的资源的 id。|
|roleDefinitionId           |字符串         |必需项。 角色分配请求相关联的角色定义的 id。|
|subjectId                  |字符串         |必需项。 其关联的角色分配请求的主题的 id。|
|type                       |字符串         |必需项。 表示的角色分配操作的类型。 值可以是 <ul><li>`AdminAdd`： 管理员分配给角色; 用户/组</li><li>`UserAdd`： 用户激活合格分配;</li><li> `AdminUpdate`： 管理员更改现有角色分配</li><li>`AdminRemove`： 管理员角色中移除用户/组<li>`UserRemove`： 用户停用活动的工作分配;<li>`UserExtend`： 用户请求扩展其即将过期的分配;</li><li>`AdminExtend`： 管理员扩展即将过期的工作分配。</li><li>`UserRenew`: 续订其过期的分配; 用户申请</li><li>`AdminRenew`： 管理员扩展即将过期的工作分配。</li></ul>|
|assignmentState|字符串  |必需项。 工作分配状态。 值可以是 <ul><li> `Eligible`合格的分配</li><li> `Active`-如果直接分配`Active`的管理员，或激活合格工作分配的用户。</li></ul>|
|requestedDateTime          |DateTimeOffset |只读。 请求创建时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|roleAssignmentStartDateTime|DateTimeOffset |角色分配开始时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|roleAssignmentEndDateTime|DateTimeOffset   |角色分配结束时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|计划                   |[governanceSchedule](governanceschedule.md)|角色分配请求的计划对象。|
|原因                     |字符串         |用户和管理员提供的一条消息时创建有关为什么需要请求。|
|状态                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |角色分配请求的状态。|
|linkedEligibleRoleAssignmentId|字符串        |如果这是角色激活请求，它所表示的 id`eligible assignment`所引用;否则，值为`null`。 |



## <a name="relationships"></a>Relationships
| 关系 | 类型                                |说明|
|:-------------|:----------------------------------|:----------|
|资源      |[governanceResource](../resources/governanceresource.md)            |只读。 旨在请求的资源。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 请求旨在角色定义。 |
|subject       |[governanceSubject](../resources/governancesubject.md)|只读。 用户/组主体。|

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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
  "roleAssignmentStartDateTime": "String (timestamp)",
  "roleAssignmentEndDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
