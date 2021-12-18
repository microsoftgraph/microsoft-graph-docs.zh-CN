---
title: educationAssignment 资源类型
description: 是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 30d6d5bd5239748b10dc9aab0b2c4acd3f676e70
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567368"
---
# <a name="educationassignment-resource-type"></a>educationAssignment 资源类型

命名空间：microsoft.graph

是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。 

只有教师或团队所有者才能创建 **作业**。 **作业** 包含教师希望学生处理的工作讲义和任务。 每个 **学生** 作业都有 [一个关联的](educationsubmissionresource.md) 提交，其中包含其教师要求提交的任何工作。 教师可以将分数和 **反馈添加到学生** 提交的提交中。

创建 **工作分配** 时，它的状态为"草稿"。 学生看不到作业 **，****并且** 不会创建提交。 可以使用发布 **操作更改工作**[分配的状态。](../api/educationassignment-publish.md) 你不能使用 PATCH 请求 **更改分配状态** 。

分配 API 在类命名空间中公开。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建作业资源](../api/educationassignment-post-resource.md) |[educationAssignmentResource](educationassignmentresource.md)| 通过发布到 **资源集合创建新的 educationAssignmentResource。**|
|[获取作业](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |读取 **educationAssignment** 对象的属性和关系。|
|[更新](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |更新 **educationAssignment** 对象。 |
|[删除](../api/educationassignment-delete.md) | 无 |删除 **educationAssignment** 对象。 |
|[发布](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|将 **educationAssignment** 对象的状态从草稿更改为已发布。|
|[设置工作分配资源文件夹](../api/educationassignment-setupresourcesfolder.md)| string| 在SharePoint位置 (创建一个) 文件夹，以将文件作为分配资源上载。|
|[列出资源](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md) 集合| 获取 **educationAssignmentResource** 对象集合。|
|[列出提交](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md) 集合| 获取 **educationSubmission** 对象集合。|
|[List categories](../api/educationassignment-list-categories.md) |[educationCategory](educationcategory.md) 集合| 获取 **educationCategory** 对象集合。|
|[添加类别](../api/educationassignment-post-categories.md) |[educationCategory](educationcategory.md) | 将 **属于课程的 educationCategory** 分配给此作业。|
|[删除类别](../api/educationassignment-remove-category.md) |无| 从此作业中删除属于课程的 **educationCategory。**|
|[附加度分](../api/educationassignment-put-rubric.md)|无|将现有 **educationRubric** 附加到此作业。|
|[删除 rubric](../api/educationassignment-delete-rubric.md)|无|从此 **作业分离 educationRubric。**|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 只读。|
|addedStudentAction|String|可选字段，用于 **控制在** 作业发布后添加的学生 **的作业** 行为。 如果未指定，则默认为 `none` value。 当前仅支持两个值： `none` 或 `assignIfOpen` 。|
|addToCalendarAction| educationAddToCalendarOptions|可选字段，用于控制 **发布** 作业时将作业添加到学生和教师日历 **的作业** 行为。 可能的值是 `none` `studentsAndPublisher` ：、、、 `studentsAndTeamOwners` `unknownFutureValue` 和 `studentsOnly` 。 请注意，必须使用此可变化枚举 (请求) 获取以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `studentsOnly` ： 。 默认值为 `none`。|
|allowLateSubmissions|布尔值| 标识学生是否可以在截止日期后提交。 如果在创建过程中未指定此属性，则默认为 true。 |
|allowStudentsToAddResourcesToSubmission|布尔值| 标识学生是否可以将自己的资源 **添加到提交中** ，或是否只能修改教师添加的资源。 |
|assignDateTime|DateTimeOffset|工作分配 **应** 处于活动状态的日期。  如果将来 **，在此日期** 之前不会向学生显示作业。  **时间戳类型表示** 使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| 发布作业后，哪些用户或整个类应 **接收提交** 对象。 |
|assignedDateTime|DateTimeOffset|将 **作业发布到学生** 时， **作业显示在学生** 时间线上。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|classId|String| 此工作分配 **所属的** 类。 |
|closeDateTime|DateTimeOffset| 工作 **分配** 将关闭提交 **的日期**。 这是一个可选字段，如果分配不允许LateSubmissions，或者 closeDateTime 与 dueDateTime 相同，该字段可能为 null。  但如果指定，则 closeDateTime 必须大于或等于 dueDateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](identityset.md)| Who创建了 **工作分配**。 |
|createdDateTime|DateTimeOffset|创建 **工作分配的** 时刻。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|displayName|String|工作分配 **的名称**。|
|dueDateTime|DateTimeOffset|学生 **作业截止日期** 。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|一个|[educationAssignmentGradeType](educationassignmentgradetype.md)|如何 **对** 作业进行评分。 |
|instructions|[itemBody](itembody.md)| 工作分配的说明。  这一显示名称告知学生要执行哪些工作。 |
|lastModifiedBy|[identitySet](identityset.md)| Who上次修改了 **工作分配**。 |
|lastModifiedDateTime|DateTimeOffset|上次 **修改工作** 分配的时刻。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|notificationChannelUrl|String|可选字段，用于指定发布 [工作](channel.md) 分配发布通知 **的通道** 的 URL。 如果未指定或为空，则默认为 `General` 频道。 此字段仅适用于 **assignTo** **值为**[educationAssignmentClassRecipient 的作业](educationassignmentclassrecipient.md)。 在发布分配后，不允许更新 **notificationChannelUrl。**|
|状态|string| 工作分配 **的状态**。  无法修补此值。  可能的值是：`draft`、`scheduled`、`published`、`assigned`。|
|webUrl|string| 给定工作分配的深层链接 **URL。**|
|resourcesFolderUrl|string| 存储此分配的所有文件资源 **的文件夹** URL。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md) 集合| Learning分配关联的对象。  只有教师可以修改此列表。 可为 NULL。|
|提交|[educationSubmission](educationsubmission.md) 集合| 发布后，每个 **学生都有一** 个表示他们的工作和成绩的提交对象。  只读。 可为 NULL。|
|categories|[educationCategory](educationcategory.md) 集合| 设置后，使用户能够轻松查找 **给定** 类型的工作分配。  只读。 可为 NULL。|
|rubric|[educationRubric](educationrubric.md)|设置时，评分标准附加到 **此分配**。|

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
  "addToCalendarAction": "string",  
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
  "notificationChannelUrl": "string",
  "status": "string",
  "webUrl": "string",
  "resourcesFolderUrl": "string"
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
