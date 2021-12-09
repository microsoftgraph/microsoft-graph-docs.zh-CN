---
title: educationClass 资源类型
description: 表示学校的课程。 **educationClass** 资源对应于 Microsoft 365 组并共享同一 ID。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 973cb6ad47feb4d37030eb42d3bdca131c0bdd01
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390667"
---
# <a name="educationclass-resource-type"></a>educationClass 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校的课程。 **educationClass** 资源当前对应于Microsoft 365 [组并]共享同一 ID。
学生是课程的普通成员，教师是所有者并且具有适当的权限。

> [!IMPORTANT]
> 若要Microsoft 365体验，教师必须是教师和成员集合的成员。

## <a name="methods"></a>方法

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
| [创建 educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | 通过发布到 **作业集合创建新的 educationAssignment。**            |
| [列出作业](../api/educationclass-list-assignments.md)           | [educationAssignment]集合                | 获取 **educationAssignment** 对象集合。                                         |
| [Get group](../api/educationclass-get-group.md)                         | [组]                                        | 获取Microsoft 365 **educationClass** 对应的组。              |
| [创建 educationCategory](../api/educationclass-post-category.md)      | [educationCategory]                            | 为此课程 **创建新的 educationCategory。**                                        |
| [List categories](../api/educationclass-list-categories.md)             | [educationCategory] 集合                 | 获取属于 **此类的 educationCategory** 对象列表。                      |
| [Update](../api/educationclass-update.md)                               | [educationClass]                               | 更新 **educationClass** 对象。                                                         |
| [删除](../api/educationclass-delete.md)                               | 无                                           | 删除 **educationClass** 对象。                                                         |
| [获取增量](../api/educationclass-delta.md)                                 | [educationClass](educationclass.md) 集合 | 获取 **educationClasses 的增量更改**。                                          |

## <a name="properties"></a>属性

| 属性             | 类型                                  | 说明                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                                | 课程的唯一标识符。                                                                                                                                     |
| classCode            | String                                | 学校用于标识课程的课程代码。                                                                                                                 |
| 课程               | [educationCourse](educationcourse.md) | 课程的课程信息。                                                                                                                                     |
| createdBy            | [identitySet]                         | 创建类的实体。                                                                                                                                         |
| description          | String                                | 课程说明。                                                                                                                                            |
| displayName          | 字符串                                | 课程名称。                                                                                                                                                   |
| externalId           | String                                | 来自同步系统的课程 ID。                                                                                                                             |
| externalName         | String                                | 同步系统中的课程名称。                                                                                                                             |
| externalSource       | String                                | 此资源的外部源类型是从外部 (自动确定的 `externalSourceDetail`) 。 可能的值为： `sis`、 `lms`或 `manual`。 |
| externalSourceDetail | 字符串                                | 生成此资源的外部源的名称。                                                                                                   |
| grade                | String                                | 课程的年级。                                                                                                                                            |
| mailNickname         | String                                | 向所有成员发送电子邮件的邮件名称（如果已启用）。                                                                                                      |
| term                 | [educationTerm]                       | 类的术语。                                                                                                                                                  |

## <a name="relationships"></a>关系

| 关系 | 类型                             | 说明                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | [educationAssignment] 集合 | 与此课程关联的所有工作分配。 可为 Null。     |
| members      | [educationUser] 集合       | 课程中的所有用户。 可为 NULL。                         |
| schools      | [educationSchool] 集合     | 与此课程相关的所有学校。 可为 NULL。 |
| teachers     | [educationUser] 集合       | 课程中的所有教师。 可为 Null。                      |

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
[组]: group.md


