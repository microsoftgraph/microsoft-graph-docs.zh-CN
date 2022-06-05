---
title: educationAssignment 资源类型
description: 是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。
ms.localizationpriority: medium
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b67f68e8b4923cea18318c344c879c2d3f90204c
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899992"
---
# <a name="educationassignment-resource-type"></a>educationAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

是指将任务或工作单元分配给课程中的学生或团队成员，作为其学习的一部分。 

只有教师或团队所有者才能创建 **作业**。 **作业** 包含教师希望学生处理的讲义和任务。 每个学生 **作业** 都有一个关联 [的提交](educationsubmissionresource.md) ，其中包含其教师要求上交的任何工作。 教师可以向学生上交的 **提交** 添加分数和反馈。

创建 **分配** 时，它处于“草稿”状态。 学生看不到 **作业** ，无法创建 **提交** 。 可以使用 [发布](../api/educationassignment-publish.md)操作更改 **分配** 的状态。 不能使用 PATCH 请求更改 **分配** 状态。

**分配** API 在类命名空间中公开。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建作业资源](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| 通过发布到资源集合来创建新的 **educationAssignmentResource** 。|
|[获取作业](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |读取 **educationAssignment** 对象的属性和关系。|
|[更新](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |更新 **educationAssignment** 对象。 |
|[删除](../api/educationassignment-delete.md) | 无 |删除 **educationAssignment** 对象。 |
|[发布](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|将 **educationAssignment** 对象的状态从草稿更改为已发布。|
|[设置工作分配资源文件夹](../api/educationassignment-setupresourcesfolder.md)| string| 在预定义的位置) 下创建 SharePoint 文件夹 (以将文件作为分配资源上传。|
|[设置工作分配反馈资源文件夹](../api/educationassignment-setupfeedbackresourcesfolder.md)|[educationAssignment](../resources/educationassignment.md)|创建 SharePoint 文件夹以上传给定 [educationSubmission](../resources/educationsubmission.md) 的反馈文件。|
|[列出资源](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md) 集合| 获取 **educationAssignmentResource** 对象集合。|
|[列出提交](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md) 集合| 获取 **educationSubmission** 对象集合。|
|[List categories](../api/educationassignment-list-categories.md) |[educationCategory](educationcategory.md) 集合| 获取 **educationCategory** 对象集合。|
|[添加类别](../api/educationassignment-post-categories.md) |[educationCategory](educationcategory.md) | 将属于该类 **的 educationCategory** 分配给此作业。|
|[删除类别](../api/educationassignment-remove-category.md) |无| 从此 **作业** 中删除属于该类 **的 educationCategory**。|
|[附加 rubric](../api/educationassignment-put-rubric.md)|无|将现有 **educationRubric** 附加到此 **作业**。|
|[删除 rubric](../api/educationassignment-delete-rubric.md)|无|将 **educationRubric** 与此 **作业** 分离。|
|[Get delta](../api/educationassignment-delta.md)|[educationAssignment](../resources/educationassignment.md) 集合|获取新创建或更新 **的分配** 的列表，而无需对集合执行完整读取。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|
|addedStudentAction|String|用于控制在作业发布后添加 **的学生的****作业** 行为的可选字段。 如果未指定，则 `none` 默认为值。 目前仅支持两个值： `none` 或 `assignIfOpen`。|
|addToCalendarAction| educationAddToCalendarOptions|用于控制在作业发布时将 **作业** 添加到学生和教师 **日历的****作业** 行为的可选字段。 可能的值是： `none`、 `studentsAndPublisher`、 `studentsAndTeamOwners`、 `unknownFutureValue`和 `studentsOnly`。 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取以下值 (此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的) ： `studentsOnly` 默认值为 `none`。|
|allowLateSubmissions|Boolean| 标识学生是否可以在截止日期后提交。 如果在创建过程中未指定此属性，则默认为 true。 |
|allowStudentsToAddResourcesToSubmission|Boolean| 确定学生是否可以将自己的资源添加到 **提交** 中，或者是否只能修改教师添加的资源。 |
|assignDateTime|DateTimeOffset|**分配** 应处于活动状态的日期。  如果将来，直到此日期才会向学生显示 **作业** 。  **时间戳** 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| 发布 **分配** 后，哪些用户或整个类应接收 **提交** 对象。 |
|assignedDateTime|DateTimeOffset|**作业** 发布给学生的那一刻，**作业** 显示在学生日程表上。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|classId|String| 此 **分配** 所属的类。 |
|closeDateTime|DateTimeOffset| 将关闭 **分配** 以 **供提交的** 日期。 如果 **分配** 不允许LateSubmissions或 closeDateTime 与 dueDateTime 相同，则此字段可以为 null。 但如果指定，则 closeDateTime 必须大于或等于 dueDateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|createdBy|[identitySet](identityset.md)| 创建 **分配** 的人员。 |
|createdDateTime|DateTimeOffset|创建 **分配** 的那一刻。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|displayName|String|**分配** 的名称。|
|dueDateTime|DateTimeOffset|学生 **作业** 截止日期。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|feedbackResourcesFolderUrl|String|存储此 **分配** 的所有反馈文件资源的文件夹 URL。|
|分级|[educationAssignmentGradeType](educationassignmentgradetype.md)|如何对 **分配** 进行分级。 |
|指示|[itemBody](itembody.md)| **有关分配** 的说明。  这连同显示名称一起告诉学生该怎么做。 |
|lastModifiedBy|[identitySet](identityset.md)| 上次修改 **分配** 的人员。 |
|lastModifiedDateTime|DateTimeOffset|上次修改 **分配** 的那一刻。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|notificationChannelUrl|String|用于指定用于发布 **分配** 发布通知的 [通道](channel.md)的 URL 的可选字段。 如果未指定或为 null，则 `General` 默认为通道。 此字段仅适用于 **assignTo** 值为 [educationAssignmentClassRecipient](educationassignmentclassrecipient.md) 的 **作业**。 发布 **分配** 后，不允许更新 **notificationChannelUrl**。|
|状态|string| **工作分配** 的状态。  无法修补此值。  可能的值是：`draft`、`scheduled`、`published`、`assigned`。|
|WebUrl|string| 给定 **分配** 的深层链接 URL。|
|resourcesFolderUrl|string| 存储此 **分配** 的所有文件资源的文件夹 URL。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationAssignmentResource](educationassignmentresource.md) 集合| 学习与此 **分配** 关联的对象。  只有教师才能修改此列表。 可为 Null。|
|提交|[educationSubmission](educationsubmission.md) 集合| 发布后，每个表示其工作和成绩的学生都有一个 **提交** 对象。  只读。 可为 Null。|
|类别|[educationCategory](educationcategory.md) 集合| 设置后，用户可以轻松查找给定类型的 **分配** 。  只读。 可为 Null。|
|量规|[educationRubric](educationrubric.md)|设置后，附加到此 **分配** 的分级红标。|

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
