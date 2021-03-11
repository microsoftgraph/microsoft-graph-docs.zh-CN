---
title: educationAssignment 资源类型
description: '**educationAssignment** 资源表示作为学习的一部分分配给课堂中学生或团队成员的任务或工作单位。 只有教师或团队所有者才能创建作业。 作业包含教师希望学生处理的工作讲义和任务。 每个学生作业都有一个关联的提交，其中包含其教师要求其提交的任何工作。 教师可以将分数和反馈添加到学生提交的提交中。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6cbeb1ac7f7462716afbe9b2e7f98cece48a479b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722459"
---
# <a name="educationassignment-resource-type"></a>educationAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**educationAssignment** 资源表示作为学习的一部分分配给课堂中学生或团队成员的任务或工作单位。 只有教师或团队所有者才能创建作业。 作业包含教师希望学生处理的工作讲义和任务。 每个学生作业都有一 [个关联的提交](educationsubmissionresource.md) ，其中包含其教师要求其提交的任何工作。 教师可以将分数和反馈添加到学生提交的提交中。

创建工作分配时，它的状态为"草稿"。 学生看不到作业，并且不会创建提交。 可以使用发布操作更改工作分配 [的状态](../api/educationassignment-publish.md) 。 不能使用 PATCH 请求更改分配状态。

分配 API 在类命名空间中公开。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出资源](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md) 集合| 获取 **educationAssignmentResource** 对象集合。|
|[列出提交](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md) 集合| 获取 **educationSubmission** 对象集合。|
|[List categories](../api/educationassignment-list-categories.md) |[educationCategory](educationcategory.md) 集合| 获取 **educationCategory** 对象集合。|
|[创建作业资源](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| 通过发布到 **资源集合创建新的 educationAssignmentResource。**|
|[获取作业](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |读取 **educationAssignment 对象的属性和** 关系。|
|[更新](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |更新 **educationAssignment** 对象。 |
|[删除](../api/educationassignment-delete.md) | 无 |删除 **educationAssignment** 对象。 |
|[添加类别](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | 为此作业 **分配属于课程的 educationCategory。**|
|[删除类别](../api/educationassignment-remove-category.md) |无| 从此 **作业中删除属于课程的 educationCategory。**|
|[附加比分](../api/educationassignment-put-rubric.md)|无|将现有 **educationRubric** 附加到此作业。|
|[删除分卡](../api/educationassignment-delete-rubric.md)|无|从此 **作业分离 educationRubric。**|
|[发布](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|将 **educationAssignment** 对象的状态从草稿更改为已发布。|
|[获取资源文件夹 URL](../api/educationassignment-getresourcesfolderurl.md)| string| 应放置基于文件的资源的 OneDrive 文件夹作为工作分配资源的一部分。 文件必须位于此文件夹中，以作为资源添加。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|
|addedStudentAction|String|控制作业发布后添加的学生的作业行为的可选字段。 如果未指定，则默认为 `none` 值。 当前仅支持两个值： `none` 或 `assignIfOpen` 。|
|allowLateSubmissions|布尔| 标识学生是否可以在截止日期之后提交。 如果在创建过程中未指定此属性，则此属性默认为 true。 |
|allowStudentsToAddResourcesToSubmission|布尔| 标识学生是否可以将自己的资源添加到提交中，或者是否只能修改教师添加的资源。 |
|assignDateTime|DateTimeOffset|工作分配应处于活动状态的日期。  如果将来，在此日期之前不会向学生显示作业。  **时间戳类型表示** 使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| 发布作业后，哪些用户或整个类应接收提交对象。 |
|assignedDateTime|DateTimeOffset|将作业发布到学生和作业的时间显示在学生时间线上。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|classId|String| 此工作分配所属的类。 |
|closeDateTime|DateTimeOffset| 工作分配将关闭提交的日期。 这是一个可选字段，如果分配不允许LateSubmissions 或 closeDateTime 与 dueDateTime 相同，则该字段可能为空。 但如果指定，则 closeDateTime 必须大于或等于 dueDateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](identityset.md)| 创建工作分配的人。 |
|createdDateTime|DateTimeOffset|创建工作分配的时刻。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|displayName|String|工作分配的名称。|
|dueDateTime|DateTimeOffset|学生作业截止日期。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|评分|[educationAssignmentGradeType](educationassignmentgradetype.md)|如何对工作分配进行评分。 |
|instructions|[itemBody](itembody.md)| 工作分配的说明。  这一显示名称告诉学生要做什么。 |
|lastModifiedBy|[identitySet](identityset.md)| 上次修改工作分配的人。 |
|lastModifiedDateTime|DateTimeOffset|上次修改工作分配的时刻。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|notificationChannelUrl|String|用于指定要发布工作分配发布通知[](channel.md)的通道的 URL 的可选字段。 如果未指定或为空，则默认为 `General` 通道。 此字段仅适用于 **assignTo** 值为 [educationAssignmentClassRecipient 的工作分配](educationassignmentclassrecipient.md)。 发布分配后，不允许更新 **notificationChannelUrl。**|
|状态|string| 工作分配 **的状态**。  无法修补此值。  可取值为：`draft`、`scheduled`、`published`、`assigned`。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md) 集合| 学习与此分配关联的对象。  只有教师可以修改此列表。 可为 NULL。|
|提交|[educationSubmission](educationsubmission.md) 集合| 发布后，每个学生都有一个表示他们的工作和成绩的提交对象。  只读。 可为 NULL。|
|categories|[educationCategory](educationcategory.md) 集合| 设置后，使用户能够轻松查找给定类型的工作分配。  只读。 可为 NULL。|
|rubric|[educationRubric](educationrubric.md)|设置后，附加到此工作分配的评分标准。|

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
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "closeDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "notificationChannelUrl": null,
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