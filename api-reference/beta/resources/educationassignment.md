---
title: educationAssignment 资源类型
description: '**EducationAssignment**资源表示分配给课程中的学生或团队成员的任务或工作单元, 作为其研究的一部分。 只有教师或团队所有者可以创建工作分配。 工作分配包含教师希望学生处理的讲义和任务。 每个学生工作分配都有一个关联的提交, 其中包含其所要求的任何教师所要启用的任何工作。 教师可以将分数和反馈添加到学生打开的提交中。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1f343edec96af2e51d1bb643abb0652425c54624
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173046"
---
# <a name="educationassignment-resource-type"></a>educationAssignment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**EducationAssignment**资源表示分配给课程中的学生或团队成员的任务或工作单元, 作为其研究的一部分。 只有教师或团队所有者可以创建工作分配。 工作分配包含教师希望学生处理的讲义和任务。 每个学生工作分配都有一个关联的[提交](educationsubmissionresource.md), 其中包含其所要求的任何教师所要启用的任何工作。 教师可以将分数和反馈添加到学生打开的提交中。

在创建工作分配时, 该工作分配处于草稿状态。 学生无法看到工作分配和提交不会被创建。 您可以使用 "[发布](../api/educationassignment-publish.md)" 操作更改工作分配的状态。 不能使用修补程序请求更改工作分配状态。

在类命名空间中公开分配 Api。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出资源](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md)集合| 获取**educationAssignmentResource**对象集合。|
|[列表提交](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md)集合| 获取**educationSubmission**对象集合。|
|[List categories](../api/educationassignment-list-categories.md) |[educationCategory](educationcategory.md)集合| 获取**educationCategory**对象集合。|
|[创建作业资源](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| 通过发布到 resources 集合创建新的**educationAssignmentResource** 。|
|[获取作业](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |读取**educationAssignment**对象的属性和关系。|
|[更新](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |更新**educationAssignment**对象。 |
|[删除](../api/educationassignment-delete.md) | 无 |删除**educationAssignment**对象。 |
|[添加类别](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | 将属于该类的**educationCategory**分配给此工作分配。|
|[删除类别](../api/educationassignment-remove-category.md) |无| 从此工作分配中删除属于该类的**educationCategory** 。|
|[附加 rubric](../api/educationassignment-put-rubric.md)|无|将现有**educationRubric**附加到此工作分配。|
|[删除 rubric](../api/educationassignment-delete-rubric.md)|无|将**educationRubric**与此工作分配分离。|
|[发布](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|将**educationAssignment**对象的状态从 "草稿" 更改为 "已发布"。|
|[获取资源文件夹 URL](../api/educationassignment-getresourcesfolderurl.md)| string| 应将基于文件的资源的 OneDrive 文件夹放置为工作分配资源的一部分。 文件必须位于此文件夹中才能作为资源添加。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|
|allowLateSubmissions|Boolean| 确定学生是否可以在截止日期后提交。 如果在创建过程中未指定此属性, 则该属性的默认值为 true。 |
|allowStudentsToAddResourcesToSubmission|Boolean| 确定学生是否可以将自己的资源添加到提交中, 或者是否只能修改教师添加的资源。 |
|assignDateTime|DateTimeOffset|工作分配应变为活动状态的日期。  如果将来, 在此日期之前, 不会向学生显示工作分配。  **时间戳**类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| 发布工作分配后, 哪些用户或整个类应接收提交对象。 |
|assignedDateTime|DateTimeOffset|将工作分配发布给学生和工作分配的时间显示在学生日程表上。  时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|classId|String| 此工作分配所属的类。 |
|createdBy|[identitySet](identityset.md)| 工作分配的创建执行者。 |
|createdDateTime|DateTimeOffset|创建工作分配的时刻。  时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|displayName|String|工作分配的名称。|
|dueDateTime|DateTimeOffset|学生工作分配到期的日期。  时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|评分|[educationAssignmentGradeType](educationassignmentgradetype.md)|将如何对工作分配进行评分。 |
|指令|[itemBody](itembody.md)| 有关分配的说明。  这与显示名称一起告诉学生要执行的操作。 |
|lastModifiedBy|[identitySet](identityset.md)| 上次修改工作分配的作者。 |
|lastModifiedDateTime|DateTimeOffset|上次修改工作分配的时刻。  时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|状态|string| **工作分配**的状态。  您不能修补此值。  可取值为：`draft`、`published`、`assigned`。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md)集合| 学习与此工作分配相关联的对象。  只有教师可以修改此列表。 可为 Null。|
|提交|[educationSubmission](educationsubmission.md)集合| 发布后, 每个学生都有一个提交对象代表其工作和评分。  只读。 可为 Null。|
|categories|[educationCategory](educationcategory.md)集合| 设置后, 用户可以轻松地找到给定类型的工作分配。  只读。 可为 Null。|
|rubric|[educationRubric](educationrubric.md)|设置时, 评分 rubric 附加到此工作分配。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
