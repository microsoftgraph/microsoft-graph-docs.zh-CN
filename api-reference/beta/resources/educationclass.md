---
title: educationClass 资源类型
description: 表示学校的课程。 **educationClass** 资源对应于Microsoft 365组，并共享相同的 ID。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 50302c03f9ccd1bd1b1ea38717be539a0731941b
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685093"
---
# <a name="educationclass-resource-type"></a>educationClass 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校的课程。 **educationClass** 资源当前对应于Microsoft 365 [组]，并共享相同的 ID。
学生是班级的普通成员，教师是所有者，具有适当的权利。

> [!IMPORTANT]
> 若要Microsoft 365经验才能正常工作，教师必须是教师和成员集合的成员。

## <a name="methods"></a>Methods

| 方法                                                                  | 返回类型                                    | 说明                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [Get educationClass](../api/educationclass-get.md)                      | [educationClass]                               | 读取 **educationClass** 对象的属性和关系。                        |
| [Add member](../api/educationclass-post-members.md)                     | [educationUser]                                | 通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。  |
| [List members](../api/educationclass-list-members.md)                   | [educationUser] 集合                     | 获取 **educationUser** 对象集合。                                               |
| [Remove student](../api/educationclass-delete-members.md)               | [educationUser]                                | 通过成员导航属性从课程删除 **educationUser**。       |
| [List schools](../api/educationclass-list-schools.md)                   | [educationSchool] 集合                   | 获取 **educationSchool** 对象集合。                                             |
| [Add teacher](../api/educationclass-post-teachers.md)                   | [educationUser]                                | 通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。 |
| [List teachers](../api/educationclass-list-teachers.md)                 | [educationUser] 集合                     | 获取课程的教师列表。                                                     |
| [Remove teacher](../api/educationclass-delete-teachers.md)              | [educationUser]                                | 通过教师导航属性从课程删除 **educationUser**。      |
| [创建 educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | 通过发布到作业集合来创建新的 **educationAssignment** 。            |
| [列出作业](../api/educationclass-list-assignments.md)           | [educationAssignmentcollection]                | 获取 **educationAssignment** 对象集合。                                         |
| [Get group](../api/educationclass-get-group.md)                         | [group]                                        | 获取与此 **educationClass** 对应的Microsoft 365 **组**。              |
| [创建 educationCategory](../api/educationclass-post-category.md)      | [educationCategory]                            | 为此类创建新的 **educationCategory** 。                                        |
| [List categories](../api/educationclass-list-categories.md)             | [educationCategory] 集合                 | 获取属于此类的 **educationCategory 对象的** 列表。                      |
| [Update](../api/educationclass-update.md)                               | [educationClass]                               | 更新 **educationClass** 对象。                                                         |
| [Delete](../api/educationclass-delete.md)                               | 无                                           | 删除 **educationClass** 对象。                                                         |
| [获取增量](../api/educationclass-delta.md)                                 | [educationClass](educationclass.md) 集合 | 获取 **educationClasses** 的增量更改。                                          |

## <a name="properties"></a>属性

| 属性             | 类型                                  | 说明                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                                | 课程的唯一标识符。                                                                                                                                     |
| classCode            | String                                | 学校用于标识课程的课程代码。                                                                                                                 |
| 课程               | [educationCourse](educationcourse.md) | 类的课程信息。                                                                                                                                     |
| createdBy            | [identitySet]                         | 创建类的实体。                                                                                                                                         |
| 说明          | String                                | 课程说明。                                                                                                                                            |
| displayName          | 字符串                                | 课程名称。                                                                                                                                                   |
| externalId           | String                                | 来自同步系统的课程 ID。                                                                                                                             |
| externalName         | String                                | 同步系统中的课程名称。                                                                                                                             |
| externalSource       | 字符串                                | 此资源的外部源的类型是从) 自动确定 `externalSourceDetail` 的 (生成的。 可能的值为： `sis`、 `lms`或 `manual`。 |
| externalSourceDetail | String                                | 从中生成此资源的外部源的名称。                                                                                                   |
| grade                | String                                | 类的等级级别。                                                                                                                                            |
| mailNickname         | String                                | 向所有成员发送电子邮件的邮件名称（如果已启用）。                                                                                                      |
| term                 | [educationTerm]                       | 类的术语。                                                                                                                                                  |

## <a name="relationships"></a>关系

| 关系 | 类型                             | 说明                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | [educationAssignment] 集合 | 与此类关联的所有作业。 可为 Null。     |
| members      | [educationUser] 集合       | 课程中的所有用户。 可为 NULL。                         |
| schools      | [educationSchool] 集合     | 与此课程相关的所有学校。 可为 NULL。 |
| teachers     | [educationUser] 集合       | 课程中的所有教师。 可为 NULL。                      |
|assignmentCategories| [educationCategory](educationcategory.md) 集合 | 与此类关联的所有类别。 可为 NULL。 |
|assignmentDefaults| [educationAssignmentDefaults](educationassignmentdefaults.md) 集合 | 指定类中创建的新作业所尊重的类级默认值。 |
|assignmentSettings| [educationAssignmentSettings](educationassignmentsettings.md) 集合 | 指定类级分配设置。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "classCode": "String",
  "course": { "@odata.type": "microsoft.graph.educationCourse" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "grade": "string",
  "id": "String (identifier)",
  "mailNickname": "String",
  "term": { "@odata.type": "microsoft.graph.educationTerm" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.educationClass",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[identityset]: identityset.md
[group]: group.md


