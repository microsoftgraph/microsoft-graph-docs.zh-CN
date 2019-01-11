---
title: educationAssignment 资源类型
description: '**EducationAssignment**资源表示任务或工作分配给类中的学生或团队成员属于其研究单位。 只有教师或团队所有者可以创建工作分配。 分配包含讲义和教师希望学生处理的任务。 每个学生工作分配的包含其教师要求打开任何工作关联的提交。 教师可以向打开由学生提交添加分数和反馈。'
localization_priority: Normal
ms.openlocfilehash: d9d7b11dcd476f0fdd2bbb24364dd0e1e026f200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812451"
---
# <a name="educationassignment-resource-type"></a>educationAssignment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**EducationAssignment**资源表示任务或工作分配给类中的学生或团队成员属于其研究单位。 只有教师或团队所有者可以创建工作分配。 分配包含讲义和教师希望学生处理的任务。 每个学生工作分配的包含其教师要求打开任何工作关联的[提交](educationsubmissionresource.md)。 教师可以向打开由学生提交添加分数和反馈。

创建一个工作分配后，它是草稿状态。 学生无法查看工作分配并不会创建提交。 可以使用[发布](../api/educationassignment-publish.md)操作来更改工作分配的状态。 不能使用 PATCH 请求更改的工作分配状态。

工作分配 Api 公开类命名空间中。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取工作分配](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |读取属性和**educationAssignment**对象的关系。|
|[创建工作分配资源](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| 通过发布到 resources 集合中创建新**educationAssignmentResource** 。|
|[列表资源](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md)集合| 获取**educationAssignmentResource**对象集合。|
|[列表提交](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md)集合| 获取**educationSubmission**对象集合。|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |更新**educationAssignment**对象。 |
|[删除](../api/educationassignment-delete.md) | 无 |删除**educationAssignment**对象。 |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|从草稿发布更改**educationAssignment**对象的状态。|
|[获取资源文件夹的 URL](../api/educationassignment-getresourcesfolderurl.md)| string| 向其中应放置基于文件的资源的工作分配资源的一部分 OneDrive 文件夹。 文件必须位于此文件夹添加为资源。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|
|allowLateSubmissions|布尔| 标识是否学生可以提交后到期日期。 如果在创建期间未指定此属性，则默认为 true。 |
|allowStudentsToAddResourcesToSubmission|布尔| 标识学生是否可以将自己的资源添加到提交或如果他们只能修改添加教师资源。 |
|assignDateTime|DateTimeOffset|当工作分配应处于活动状态日期。  如果将来，工作分配时不显示到学生此日期之前。  **时间戳**类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| 哪些用户或整个类应收到提交对象后发布工作分配。 |
|assignedDateTime|DateTimeOffset|工作分配发布到学生和工作分配的时刻显示学生日程表上。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|classId|字符串| 此工作分配所属的类。 |
|createdBy|[identitySet](identityset.md)| 工作分配的创建者。 |
|createdDateTime|DateTimeOffset|矩何时创建工作分配。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|displayName|字符串|工作分配的名称。|
|dueDateTime|DateTimeOffset|学生工作分配的到期日期。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|分级|[educationAssignmentGradeType](educationassignmentgradetype.md)|如何将评分工作分配。 |
|说明|[itemBody](itembody.md)| 工作分配的说明。  这的显示名称以及要执行的操作告知学生。 |
|lastModifiedBy|[identitySet](identityset.md)| 用户上次修改工作分配。 |
|lastModifiedDateTime|DateTimeOffset|上次修改工作分配的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|status|string| **工作分配**状态。  您可以不修补程序此值。  可取值为：`draft`、`published`、`assigned`。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md)集合| 学习与此工作分配关联的对象。  仅教师可以修改此列表。 可为 Null。|
|提交|[educationSubmission](educationsubmission.md)集合| 发布后，没有表示其工作和薪等级每个学生的提交对象。  只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
