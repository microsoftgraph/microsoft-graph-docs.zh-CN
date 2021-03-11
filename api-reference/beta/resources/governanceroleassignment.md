---
title: governanceRoleAssignment 资源类型
description: 表示将用户或组分配至角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6d9e1b56a503ffdf1bde6bde6a583b78f8a34851
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722305"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment 资源类型

命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示将用户或组分配至角色。

PRIVILEGEd Identity Management (PIM) 支持两种类型的分配：

1. 活动分配 - 表示对资源的直接/激活访问。
2. 符合条件的分配 - 表示对资源的特权访问的中间阶段，介于无访问和直接访问之间。 管理员可以提前将用户/组分配给用户/组，只要需要访问权限，就可以在几个小时内立即访问 `eligible assignment` `activation` `eligible assignment` 资源。 激活后 `active assignment` ，将为用户/组的成员创建一个指示激活状态。

## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:------------|:--------|:--------|
|[获取](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |读取实体的属性角色分配关系。|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|列出资源上的角色分配集合。 |
|[Export](../api/governanceroleassignment-export.md) | octet-stream |下载资源上的角色分配集合并另存为 `.csv` 文件。|

实体 `POST` 集不支持 ，，或 `PUT` `PATCH` `DELETE` `roleAssignments` 操作。 任何创建、更新和删除操作 `governanceRoleAssignment` 都由 `governanceRoleAssignmentRequest` .

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |id of the 角色分配. 它采用 GUID 格式。|
|resourceId |String     |必填。 与其关联的角色分配的 ID。 |
|roleDefinitionId|String|必填。 角色定义与角色分配的 ID。 |
|subjectId|String       |必填。 与其关联的角色分配的 ID。 |
|linkedEligibleRoleAssignmentId|String|如果这是由于激活 `active assignment` 而创建的，则它表示该 `eligible assignment` `eligible assignment` ID;否则，值为 `null` 。 |
|externalId   |String     |用于标识提供程序中的外部角色分配 ID。|
|startDateTime|DateTimeOffset|开始时间的角色分配。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|对于非永久角色分配，此时角色分配过期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|assignmentState|String  |工作分配的状态。 值可以是 <ul><li> `Eligible` 对于符合条件的分配</li><li> `Active` - 如果由管理员直接分配，或由用户在符合条件的分配 `Active` 上激活。</li></ul>|
|memberType|String      |成员的类型。 值可以是： <ul><li>`Inherited` - 角色分配父资源作用域继承的资源</li><li>`Group`- 角色分配继承，但来自组分配的成员身份</li><li>`User` - 角色分配既不继承也不从组分配继承。</li></ul>|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 与项目关联的角色分配。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 与角色关联的角色角色分配。 |
|subject|[governanceSubject](../resources/governancesubject.md)|只读。 与主题关联的角色分配。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|只读。 如果这是一 `active assignment` 个由于激活而创建的， `eligible assignment` 则它表示该对象 `eligible assignment` ;否则，值为 `null` 。 |

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


