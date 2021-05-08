---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Microsoft 365 组并共享同一 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 528ea878ad5ed507c83a750d617209b4cde3d589
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231516"
---
# <a name="educationclass-resource-type"></a>educationClass 资源类型

命名空间：microsoft.graph

表示学校的课程。 **educationClass** 资源对应于 Microsoft 365 组并共享同一 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

| 方法                                                   | 返回类型                                                 | 说明                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [列出 educationClasses](../api/educationclass-list.md)   | [educationClass](../resources/educationclass.md) 集合 | 获取 [educationClass 对象](../resources/educationclass.md) 及其属性的列表。     |
| [Create educationClass](../api/educationclass-post.md) | [educationClass](../resources/educationclass.md)            | 创建新的 [educationClass](../resources/educationclass.md) 对象。                                |
| [Get educationClass](../api/educationclass-get.md)       | [educationClass](../resources/educationclass.md)            | 读取 [educationClass](../resources/educationclass.md) 对象的属性和关系。 |
| [更新 educationClass](../api/educationclass-update.md) | [educationClass](../resources/educationclass.md)            | 更新 [educationClass 对象](../resources/educationclass.md) 的属性。                 |
| [删除 educationClass](../api/educationclass-delete.md) | 无                                                        | 删除 [educationClass](../resources/educationclass.md) 对象。                                  |
| [增量](../api/educationclass-delta.md)                  | [educationClass](../resources/educationclass.md) 集合 | 获取资源集合的增量更改。                                                  |

## <a name="properties"></a>属性

| 属性             | 类型                                           | 说明                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | 对象标识符。 继承自 [实体](../resources/entity.md)。 |
| displayName          | String                                         | 课程名称。                                                 |
| mailNickname         | String                                         | 向所有成员发送电子邮件的邮件名称（如果已启用）。    |
| 说明          | String                                         | 课程说明。                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | 创建了课程的实体                                       |
| classCode            | String                                         | 学校用于标识课程的课程代码。               |
| externalName         | String                                         | 同步系统中的课程名称。                           |
| externalId           | String                                         | 来自同步系统的课程 ID。                           |
| externalSource       | educationExternalSource                        | 此课程的创建方式。 可取值为：`sis`、`manual`。  |
| externalSourceDetail | String                                         | 生成此资源的外部源的名称。 |
| grade                | String                                         | 课程的年级。                                          |
| term                 | [educationTerm](../resources/educationterm.md) | 此课程的学期。                                               |

## <a name="relationships"></a>关系

| 关系 | 类型                                                          | 说明                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| group        | [组](../resources/group.md)                                | 组Microsoft 365对象。                |
| members      | [educationUser](../resources/educationuser.md) 集合     | 课程中的所有用户。 可为 NULL。                         |
| schools      | [educationSchool](../resources/educationschool.md) 集合 | 与此课程相关的所有学校。 可为 NULL。 |
| teachers     | [educationUser](../resources/educationuser.md) 集合     | 课程中的所有教师。 可为 Null。                      |

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
