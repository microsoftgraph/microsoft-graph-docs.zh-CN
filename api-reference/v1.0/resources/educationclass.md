---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于Microsoft 365组，并共享相同的 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
ms.localizationpriority: medium
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d9853bf9d82240801c9853b69a60b21ad8830709
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366231"
---
# <a name="educationclass-resource-type"></a>educationClass 资源类型

命名空间：microsoft.graph

表示学校的课程。 **educationClass** 资源对应于Microsoft 365组，并共享相同的 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods

| 方法                                                   | 返回类型                                                 | 说明                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [列出 educationClasses](../api/educationclass-list.md)   | [educationClass](../resources/educationclass.md) 集合 | 获取 [educationClass](../resources/educationclass.md) 对象及其属性的列表。     |
| [Create educationClass](../api/educationclass-post.md) | [educationClass](../resources/educationclass.md)            | 创建新的 [educationClass](../resources/educationclass.md) 对象。                                |
| [Get educationClass](../api/educationclass-get.md)       | [educationClass](../resources/educationclass.md)            | 读取 [educationClass](../resources/educationclass.md) 对象的属性和关系。 |
| [更新 educationClass](../api/educationclass-update.md) | [educationClass](../resources/educationclass.md)            | 更新 [educationClass](../resources/educationclass.md) 对象的属性。                 |
| [删除 educationClass](../api/educationclass-delete.md) | 无                                                        | 删除 [educationClass](../resources/educationclass.md) 对象。                                  |
| [Get delta](../api/educationclass-delta.md)                  | [educationClass](educationclass.md) 集合              | 获取 **educationClasses** 的增量更改。                                          |

## <a name="properties"></a>属性

| 属性             | 类型                                           | 说明                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | 对象标识符。 继承自 [entity](../resources/entity.md)。 |
| displayName          | 字符串                                         | 课程名称。                                                 |
| mailNickname         | String                                         | 向所有成员发送电子邮件的邮件名称（如果已启用）。    |
| 说明          | String                                         | 课程说明。                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | 创建了课程的实体                                       |
| classCode            | String                                         | 学校用于标识课程的课程代码。               |
| externalName         | String                                         | 同步系统中的课程名称。                           |
| externalId           | String                                         | 来自同步系统的课程 ID。                           |
| externalSource       | educationExternalSource                        | 此课程的创建方式。 可取值为：`sis`、`manual`。  |
| externalSourceDetail | 字符串                                         | 从中生成此资源的外部源的名称。 |
| grade                | String                                         | 类的等级级别。                                          |
| term                 | [educationTerm](../resources/educationterm.md) | 此课程的学期。                                               |

## <a name="relationships"></a>关系

| 关系 | 类型                                                          | 说明                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| assignments  | [educationAssignment](educationAssignment.md) 集合 | 与此类关联的所有作业。 可为 NULL。     |
| 组        | [组](../resources/group.md)                                | 基础Microsoft 365组对象。                |
| members      | [educationUser](../resources/educationuser.md) 集合     | 课程中的所有用户。 可为 NULL。                         |
| schools      | [educationSchool](../resources/educationschool.md) 集合 | 与此课程相关的所有学校。 可为 NULL。 |
| teachers     | [educationUser](../resources/educationuser.md) 集合     | 课程中的所有教师。 可为 NULL。                      |
|assignmentCategories| [educationCategory](educationcategory.md) 集合 | 与此类关联的所有类别。 可为 NULL。 |
|assignmentDefaults| [educationAssignmentDefaults](educationassignmentdefaults.md) 集合 | 指定类中创建的新作业所尊重的类级默认值。 |
|assignmentSettings| [educationAssignmentSettings](educationassignmentsettings.md) 集合 | 指定类级分配设置。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
