---
title: governanceRoleAssignmentRequest 资源类型
description: 表示在 Priviledged Identity Management 中对角色分配操作的请求。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 4dd6c1c5911193306c6a0925bfec1d642a00a81c
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397584"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>governanceRoleAssignmentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示Privileged Identity Management中角色分配操作的请求。

`governanceRoleAssignmentRequest` 是票证建模实体，用于管理角色分配的生命周期。 它表示用户和管理员的意图/决策，也提供了实现定期架构、审批门等的灵活性，与直接公开`POST``PUT`和`DELETE`操作`governanceRoleAssignment`相比。

## <a name="methods"></a>方法

| 方法          |返回类型  |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|获取 ID 指定的角色分配请求。  
|[List](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)  集合|获取资源上的角色分配请求。|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|创建一个请求来管理现有或新角色分配的生命周期。|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |取消挂起的角色分配请求。|
|[更新](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|如果请求处于状态，管理员将更新有关请求的决定 `PendingAdminDecision`。|

## <a name="properties"></a>属性
| 属性                  | 类型          |说明|
|:--------------------------|:--------------|:----------|
|id                         |String         |角色分配请求的标识符。|
|resourceId                 |String         |必填。 与角色分配请求关联的 Azure 资源的唯一标识符。 Azure 资源可以包括订阅、资源组、虚拟机和SQL数据库。|
|roleDefinitionId           |字符串         |必填。 角色分配请求关联的 Azure 角色定义的标识符。|
|subjectId                  |String         |必填。 角色分配请求与之关联的主体或主体的唯一标识符。 主体可以是用户、组或服务主体。|
|type                       |String        |必填。 表示角色分配上的操作的类型。 可能的值是： `AdminAdd` 、、 `AdminUpdate` `UserAdd` 、、 `UserRemove` `AdminRemove` 、 `UserExtend` 、 `AdminExtend` 、 `UserRenew` `AdminRenew`|
|assignmentState|String  |必填。 分配的状态。 可能的值为： `Eligible` (符合条件的分配) 、  `Active` (是否直接分配) 、 `Active` 管理员 (或用户) 在符合条件的分配上激活。|
|requestedDateTime          |DateTimeOffset |只读。 请求创建时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|schedule                   |[governanceSchedule](governanceschedule.md)|角色分配请求的计划对象。|
|reason                     |字符串         |用户和管理员在创建有关为何需要它的请求时提供的消息。|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |角色分配请求的状态。|
|linkedEligibleRoleAssignmentId|String        |如果这是角色激活请求，则表示被引用的 `eligible assignment` ID;否则，值为 `null`. |

|成员|说明|
|:---|:---|
|AdminAdd|管理员将用户/组分配给角色。|
|UserAdd|用户激活符合条件的分配。|
|AdminUpdate|管理员更改现有角色分配。|
|AdminRemove|管理员从角色中删除用户/组。|
|UserRemove|用户停用活动分配。|
|UserExtend|用户请求延长其即将到期的分配。|
|AdminExtend|管理员会延长即将过期的分配。|
|UserRenew|用户请求续订其过期的分配。|
|AdminRenew|管理员会延长即将过期的分配。|



## <a name="relationships"></a>关系
| 关系 | 类型                                |说明|
|:-------------|:----------------------------------|:----------|
|资源      |[governanceResource](../resources/governanceresource.md)            |只读。 请求所针对的资源。 |
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


