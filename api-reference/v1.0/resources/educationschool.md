---
title: educationSchool 资源类型
description: '一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  '
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 01f6bd1f7ebc77d90cb6fbdbf5d4daf22f9dda0a7bdb663516fc51933afc8ca1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184905"
---
# <a name="educationschool-resource-type"></a>educationSchool 资源类型

命名空间：microsoft.graph

一种表示学校的资源，用于管理所表示学校的课程、教师和学生。

继承自 [educationOrganization](../resources/educationorganization.md)。

## <a name="methods"></a>方法

| 方法                                                     | 返回类型                                                   | 说明                                                                                            |
| :--------------------------------------------------------- | :------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------- |
| [列出 educationSchools](../api/educationschool-list.md)    | [educationSchool](../resources/educationschool.md) 集合 | 获取 [educationSchool 对象](../resources/educationschool.md) 及其属性的列表。     |
| [Create educationSchool](../api/educationschool-post.md) | [educationSchool](../resources/educationschool.md)            | 创建新的 [educationSchool](../resources/educationschool.md) 对象。                                |
| [获取 educationSchool](../api/educationschool-get.md)       | [educationSchool](../resources/educationschool.md)            | 读取 [educationSchool 对象的属性和](../resources/educationschool.md) 关系。 |
| [更新 educationSchool](../api/educationschool-update.md) | [educationSchool](../resources/educationschool.md)            | 更新 [educationSchool 对象](../resources/educationschool.md) 的属性。                 |
| [删除 educationSchool](../api/educationschool-delete.md) | 无                                                          | 删除 [educationSchool](../resources/educationschool.md) 对象。                                  |
| [delta](../api/educationschool-delta.md)                   | [educationSchool](../resources/educationschool.md) 集合 | 获取资源集合的增量更改。                                                    |

## <a name="properties"></a>属性

| 属性             | 类型                                               | 说明                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| address              | [physicalAddress](../resources/physicaladdress.md) | 学校地址。                                                                                                                                               |
| createdBy            | [identitySet](../resources/identityset.md)         | 创建了学校的实体。                                                                                                                                       |
| 说明          | String                                             | 学校描述。 继承自 [educationOrganization](../resources/educationorganization.md)。                                                             |
| displayName          | String                                             | 学校的显示名称。 继承自 [educationOrganization](../resources/educationorganization.md)。                                                            |
| externalId           | String                                             | 同步系统中学校的 ID。                                                                                                                                      |
| externalPrincipalId  | String                                             | 同步系统中主体的 ID。                                                                                                                                   |
| externalSource       | educationExternalSource                            | 创建组织的来源。 继承自 [educationOrganization](../resources/educationorganization.md)。 可取值为：`sis`、`manual`。 |
| externalSourceDetail | String                                             | 生成此资源的外部源的名称。                                                                                                   |
| highestGrade         | String                                             | 教授的最高年级。                                                                                                                                                |
| id                   | String                                             | 对象标识符。 继承自 [实体](../resources/entity.md)。                                                                                                   |
| lowestGrade          | String                                             | 教授的最低年级。                                                                                                                                                 |
| phone                | String                                             | 学校电话号码。                                                                                                                                              |
| principalEmail       | String                                             | 主体的电子邮件地址。                                                                                                                                      |
| principalName        | String                                             | 主体名称。                                                                                                                                               |
| schoolNumber         | String                                             | 学校编号。                                                                                                                                                       |

## <a name="relationships"></a>关系

| 关系       | 类型                                                        | 说明                                       |
| :----------------- | :---------------------------------------------------------- | :------------------------------------------------ |
| administrativeUnit | [administrativeUnit](../resources/administrativeunit.md)    | 此学校的基础 administrativeUnit。 |
| classes            | [educationClass](../resources/educationclass.md) 集合 | 在学校教授的课程。 可为 NULL。           |
| users              | [educationUser](../resources/educationuser.md) 集合   | 学校中的用户。 可为 Null。                    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSchool",
  "baseType": "microsoft.graph.educationOrganization",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
