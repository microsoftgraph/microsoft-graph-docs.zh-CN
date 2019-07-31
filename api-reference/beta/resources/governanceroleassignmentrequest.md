---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在 Privilegd 标识管理中对角色分配操作的请求。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 37dd85cc903fd57c640f9515329edca37396aa07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005966"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>governanceRoleAssignmentRequest 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 Privilegd 标识管理中对角色分配操作的请求。

`governanceRoleAssignmentRequest`是用于管理角色分配生命周期的票据建模实体。 它代表用户和管理员的意向/决定, 还提供了灵活性, 可实现定期 schduling、审批门等实施, 与直接公开`POST`、 `PUT`和`DELETE`操作相比`governanceRoleAssignment`。

## <a name="methods"></a>方法

| 方法          |返回类型  |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|获取由 ID 指定的角色分配请求。  
|[List](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合|获取对资源的角色分配请求。|
|[创建](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|创建一个请求, 以管理现有或新角色分配的生命周期。|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |取消挂起的角色分配请求。|
|[更新](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|如果请求处于的`PendingAdminDecision`状态, 管理员会根据请求更新决策。|

## <a name="properties"></a>属性
| 属性                  | 类型          |说明|
|:--------------------------|:--------------|:----------|
|id                         |String         |角色分配请求的 id。|
|resourceId                 |String         |必需。 与角色分配请求关联的资源的 id。|
|roleDefinitionId           |String         |必需。 与角色分配请求关联的角色定义的 id。|
|subjectId                  |String         |必需。 与角色分配请求相关联的主题的 id。|
|type                       |String         |必需。 表示角色分配上操作的类型。 值可以是 <ul><li>`AdminAdd`: 管理员将用户/组分配给角色;</li><li>`UserAdd`: 用户激活符合条件的工作分配;</li><li> `AdminUpdate`: 管理员更改现有的角色分配</li><li>`AdminRemove`: 管理员从角色中删除用户/组;<li>`UserRemove`: 用户停用活动分配;<li>`UserExtend`: 用户请求扩展即将过期的工作分配;</li><li>`AdminExtend`: 管理员扩展了即将过期的工作分配。</li><li>`UserRenew`: 用户请求续订其过期的工作分配;</li><li>`AdminRenew`: 管理员扩展了即将过期的工作分配。</li></ul>|
|assignmentState|String  |必需。 工作分配的状态。 值可以是 <ul><li> `Eligible`对于符合条件的工作分配</li><li> `Active`-如果由管理员直接分配`Active` , 或由用户在符合条件的工作分配上激活。</li></ul>|
|requestedDateTime          |DateTimeOffset |只读。 请求创建时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|schedule                   |[governanceSchedule](governanceschedule.md)|角色分配请求的 schedule 对象。|
|在于                     |String         |用户和管理员在创建请求时, 提供有关需要的原因的消息。|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |角色分配请求的状态。|
|linkedEligibleRoleAssignmentId|String        |如果这是角色激活请求, 则它表示所引用的`eligible assignment` id;否则, 值为`null`。 |



## <a name="relationships"></a>关系
| 关系 | 类型                                |说明|
|:-------------|:----------------------------------|:----------|
|资源      |[governanceResource](../resources/governanceresource.md)            |只读。 请求的目标资源。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 请求所针对的角色定义。 |
|subject       |[governanceSubject](../resources/governancesubject.md)|只读。 User/group 主体。|

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
