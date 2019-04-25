---
title: governanceRoleAssignment 资源类型
description: 表示用户或组对角色的分配。
localization_priority: Normal
ms.openlocfilehash: 77a5238aa337dd8d273d3156d285e081c4bc8875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547436"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment 资源类型
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户或组对角色的分配。

特权标识管理 (PIM) 支持两种类型的工作分配:

1. 主动分配-表示对资源的直接/激活访问。
2. 符合条件的工作分配-表示对资源的特权访问的中间阶段, 在无访问权限和直接访问之间。 管理员可以提前向用户/组`eligible assignment`分配用户/组, 并在需要访问时`activation` , 才能`eligible assignment`在几个小时内获得对该资源的即时访问权限。 激活之后, `active assignment`将为用户/组成员创建, 以指示激活的状态。

## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |读取角色分配实体的属性和关系。|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md)集合|列出资源上的角色分配的集合。 |
|[Export](../api/governanceroleassignment-export.md) | 八位字节流 |在资源上下载角色分配的集合, 并将其另`.csv`存为文件。|

`roleAssignments`实体`POST`集`PUT`上`PATCH`不支持`DELETE` 、、或操作。 上`governanceRoleAssignment`的任何创建、更新和删除操作均由`governanceRoleAssignmentRequest`完成。

## <a name="properties"></a>属性
| 属性  | 类型      |说明|
|:----------|:----------|:----------|
|id         |String     |角色分配的 ID。 它采用 GUID 格式。|
|resourceId |String     |必需。 与角色分配相关联的资源的 ID。 |
|roleDefinitionId|String|必需。 与角色分配相关联的角色定义的 ID。 |
|subjectId|String       |必需。 与角色分配相关联的主题的 ID。 |
|linkedEligibleRoleAssignmentId|String|如果这是`active assignment`并因激活而创建`eligible assignment`, 则表示的`eligible assignment`ID。否则, 值为`null`。 |
|externalId   |String     |外部 ID 用于标识提供程序中的角色分配的资源。|
|startDateTime|DateTimeOffset|角色分配的开始时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|对于非永久角色分配, 这是角色分配将在何时过期的时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|assignmentState|String  |工作分配的状态。 值可以是 <ul><li> `Eligible`对于符合条件的工作分配</li><li> `Active`-如果由管理员直接分配`Active` , 或由用户在符合条件的工作分配上激活。</li></ul>|
|memberType|String      |成员的类型。 值可以是: <ul><li>`Inherited`-角色分配是从父资源作用域继承的</li><li>`Group`-角色分配不是继承的, 而是来自组分配的成员身份</li><li>`User`-角色分配既不继承也不从组分配中继承。</li></ul>|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 与角色分配相关联的资源。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 与角色分配相关联的角色定义。 |
|subject|[governanceSubject](../resources/governancesubject.md)|只读。 与角色分配相关联的主题。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|只读。 如果这是`active assignment`并因激活而创建的`eligible assignment`, 则它表示该`eligible assignment`对象的对象;否则, 值为`null`。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
