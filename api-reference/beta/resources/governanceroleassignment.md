---
title: governanceRoleAssignment 资源类型
description: 表示向角色分配用户或组。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 048eaf2c208911714f0f880a02b37cc77cbc0966
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453840"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment 资源类型

命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示向角色分配用户或组。

Privileged Identity Management (PIM) 支持两种类型的分配：

1. 活动分配 - 表示对资源的直接/激活访问。
2. 符合条件的分配 - 表示资源特权访问的中间阶段，介于无访问和直接访问之间。 管理员可以提前将用户/组分配给 ，并且只要需要访问权限，就可以在 上获取对资源的即时访问权限 `eligible assignment` `activation` `eligible assignment` 几个小时。 激活后 `active assignment` ，将为用户/组的成员创建 以指示激活状态。

## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |读取实体的属性和角色分配关系。|
|[列出](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|列出资源上的角色分配集合。 |
|[Export](../api/governanceroleassignment-export.md) | octet-stream |下载资源上的角色分配集合，并另存为 `.csv` 文件。|

实体集不支持任何 、、 `POST` `PUT` 或 `PATCH` `DELETE` `roleAssignments` 操作。 对 执行的任何创建、更新和删除 `governanceRoleAssignment` 操作都由 完成 `governanceRoleAssignmentRequest` 。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |id of the 角色分配. 它采用 GUID 格式。|
|resourceId |String     |必填。 与项目关联的角色分配的 ID。 |
|roleDefinitionId|String|必填。 角色定义的 ID，角色分配角色定义。 |
|subjectId|字符串       |必填。 与用户关联的角色分配的 ID。 |
|linkedEligibleRoleAssignmentId|String|如果这是 和 由于 激活而创建的 ，则它表示 的 `active assignment` `eligible assignment` `eligible assignment` ID;否则，值为 `null` 。 |
|externalId   |String     |用于标识提供程序中应用程序角色分配外部 ID。|
|startDateTime|DateTimeOffset|会议开始时间角色分配。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|对于非永久角色分配，此时间将角色分配过期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|assignmentState|String  |工作分配的状态。 该值可用于符合条件的分配，或者如果该值是由管理员直接分配，或者由用户对符合条件的分配 `Eligible` `Active` `Active` 进行激活。|
|memberType|字符串      |成员的类型。 该值可以是： (如果 角色分配 继承自父资源范围) ，则 (如果 角色分配 不是继承的，但来自组分配) 的成员身份;如果 角色分配 既不继承也不从组分配) 继承 (。 `Inherited` `Group` `User`|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 与项目关联的角色分配。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 与角色关联的角色角色分配。 |
|subject|[governanceSubject](../resources/governancesubject.md)|只读。 与项目关联的角色分配。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|只读。 如果这是 和 由于 激活而创建的 ，则它表示 的 `active assignment` `eligible assignment` 对象 `eligible assignment` ;否则，值为 `null` 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


