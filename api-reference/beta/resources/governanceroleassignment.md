---
title: governanceRoleAssignment 资源类型
description: 代表向角色分配的用户或组。
ms.openlocfilehash: 3b0520f4641c961358b2db990914fbdf8de254f8
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191135"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment 资源类型
> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表向角色分配的用户或组。

特权标识管理 (PIM) 支持两种类型的工作分配：

1. 活动的工作分配-表示激活直接/资源访问权限。
2. 合格的工作分配的资源，之间没有访问和直接访问代表中间阶段的访问权限。 管理员可以分配给用户/组`eligible assignment`提前，每当和需要访问时，`activation`上`eligible assignment`需要几个小时才能资源即时访问。 激活之后，`active assignment`将创建为以指示的激活的状态的用户/组成员。

## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |读取属性和角色分配实体的关系。|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md)集合|列出角色分配对资源的集合。 |
|[Export](../api/governanceroleassignment-export.md) | 八进制流 |下载的资源角色分配集合，并将另存为`.csv`文件。|

不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`roleAssignments`实体集。 任何创建、 更新和删除操作，在`governanceRoleAssignment`通过完成`governanceRoleAssignmentRequest`。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |字符串     |角色分配的 ID。 处于 GUID 格式。|
|resourceId |String     |必需。 资源的角色分配相关联的 ID。 |
|roleDefinitionId|字符串|必需。 角色分配相关联的角色定义的 ID。 |
|subjectId|字符串       |必需。 该角色分配相关联的主题的 ID。 |
|linkedEligibleRoleAssignmentId|字符串|如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表该 ID `eligible assignment`;否则，值为`null`。 |
|externalId   |String     |外部 ID 用于标识提供程序中的角色分配的资源。|
|startDateTime|DateTimeOffset|角色分配的开始时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|对于非永久角色分配，这是时将过期的角色分配的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|assignmentState|字符串  |工作分配状态。 值可以是 <ul><li> `Eligible`合格的分配</li><li> `Active`-如果直接分配`Active`的管理员，或激活合格工作分配的用户。</li></ul>|
|memberType|字符串      |成员的类型。 值可以是： <ul><li>`Inherited`-角色分配继承自父资源范围</li><li>`Group`-角色分配不继承的但来自的组分配成员身份</li><li>`User`-既不继承的角色分配和从组工作分配。</li></ul>|


## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 与角色分配关联的资源。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 与角色分配相关联的角色定义。 |
|subject|[governanceSubject](../resources/governancesubject.md)|只读。 主题的角色分配相关联。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|只读。 如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表的`eligible assignment`;否则，值为`null`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
