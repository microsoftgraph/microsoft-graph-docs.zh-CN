---
title: governanceRoleAssignment 资源类型
description: 表示将用户或组分配给角色。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 76aaa6e63b9c44e1bc3db1ccf6e8351a5796051f
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399458"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment 资源类型

命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示将用户或组分配给角色。

Privileged Identity Management (PIM) 支持两种类型的分配：

1. 活动分配 - 表示对资源的直接/激活访问。
2. 符合条件的分配 - 表示在无访问权限和直接访问之间对资源进行特权访问的中间阶段。 管理员可以提前分配用户/组 `eligible assignment` ，并且只要需要访问权限， `activation` 就需要在该用户上 `eligible assignment` 获取对资源的即时访问几个小时。 激活后，将为用户/组成员创建一个 `active assignment` 指示已激活状态的用户/组成员。

## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |读取角色分配实体的属性和关系。|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|列出资源上的角色分配的集合。 |
|[Export](../api/governanceroleassignment-export.md) | octet-stream |下载资源上的角色分配集合并另存为 `.csv` 文件。|

`PUT`实体`POST`集不`roleAssignments`支持、`PATCH`或`DELETE`支持操作。 Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |字符串     |角色分配的 ID。 它采用 GUID 格式。|
|resourceId |String     |必填。 与角色分配关联的资源的 ID。 |
|roleDefinitionId|String|必填。 与角色分配关联的角色定义的 ID。 |
|subjectId|String       |必填。 与角色分配关联的主题的 ID。 |
|linkedEligibleRoleAssignmentId|String|如果这是 `active assignment` 由于激活而创建的 `eligible assignment`，则表示该对象的 `eligible assignment`ID：否则，值为 `null`. |
|externalId   |String     |用于标识提供程序中的角色分配的资源的外部 ID。|
|startDateTime|DateTimeOffset|角色分配的开始时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|对于非永久性角色分配，这是角色分配过期的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|assignmentState|字符串  |分配的状态。 该值可以 `Eligible` 用于符合条件的分配，或者 `Active` 是管理员直接分配 `Active` 的，也可以是用户在符合条件的分配上激活的。|
|memberType|String      |成员的类型。 值可以是： `Inherited` (角色分配是否继承自父资源范围) ， `Group` (角色分配不是继承的，而是来自组分配) `User` 的成员身份;如果角色分配既不继承，也不从组分配) 继承，则 (。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 与角色分配关联的资源。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 与角色分配关联的角色定义。 |
|subject|[governanceSubject](../resources/governancesubject.md)|只读。 与角色分配关联的主题。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|只读。 如果这是 `active assignment` 由于激活而创建的 `eligible assignment`，则表示该对象的 `eligible assignment`对象：否则，值为 `null`. |

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


