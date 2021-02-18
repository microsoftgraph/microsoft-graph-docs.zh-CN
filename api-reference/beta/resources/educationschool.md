---
title: educationSchool 资源类型
description: '学校。 **educationSchool** 资源当前对应于 administrativeUnit 资源并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f8481ad876cd5c4c9a2f1bc8ca67297c647475ba
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292635"
---
# <a name="educationschool-resource-type"></a>educationSchool 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校。 **educationSchool** 资源当前对应于 [administrativeUnit](administrativeunit.md)资源并共享相同的 ID。

此资源是 [educationOrganization](educationorganization.md)的子类型。

## <a name="methods"></a>方法

| 方法                                                                     | 返回类型                                      | 说明                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [获取](../api/educationschool-get.md)                                       | [educationSchool](educationschool.md)            | 读取 **educationSchool** 对象的属性和关系。                         |
| [Add class](../api/educationschool-post-classes.md)                        | [educationClass](educationclass.md)              | 通过发布到课程导航属性，为学校添加一个新的 **educationClass**。  |
| [List classes](../api/educationschool-list-classes.md)                     | [educationClass](educationclass.md) 集合   | 获取 **educationClass** 对象集合。                                               |
| [Remove class](../api/educationschool-delete-classes.md)                   | [educationClass](educationclass.md)              | 通过课程导航属性从学校删除 **educationClass**。       |
| [Add user](../api/educationschool-post-users.md)                           | [educationUser](educationuser.md)                | 通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。 |
| [List users](../api/educationschool-list-users.md)                         | [educationUser](educationuser.md) 集合     | 获取 **educationUser** 对象集合。                                                |
| [Remove user](../api/educationschool-delete-users.md)                      | [educationUser](educationuser.md)                | 通过 **users** 导航属性从学校删除 **educationUser**。      |
| [获取 administrativeUnit](../api/educationschool-get-administrativeunit.md) | [administrativeUnit](administrativeunit.md)      | 获取 **对应于此** **educationSchool 的 administrativeUnit。**                |
| [Update](../api/educationschool-update.md)                                 | [educationSchool](educationschool.md)            | 更新 **educationSchool** 对象。                                                       |
| [删除](../api/educationschool-delete.md)                                 | 无                                             | 删除 **educationSchool** 对象。                                                       |
| [Delta](../api/educationschool-delta.md)                                   | [educationSchool](educationschool.md) 集合 | 获取 **educationSchools 的增量更改**                                            |

## <a name="properties"></a>属性

| 属性             | 类型                                  | 说明                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                                | 该学校的 GUID。                                                                                                                                                 |
| address              | [physicalAddress](physicaladdress.md) | 学校地址。                                                                                                                                               |
| createdBy            | [identitySet](identityset.md)         | 创建了学校的实体。                                                                                                                                       |
| description          | String                                | 学校描述。                                                                                                                                           |
| displayName          | String                                | 学校的显示名称。                                                                                                                                          |
| externalId           | String                                | 同步系统中学校的 ID。                                                                                                                                      |
| externalPrincipalId  | String                                | 同步系统中主体的 ID。                                                                                                                                   |
| externalSource       | String                                | 此资源的外部源类型由 (自动确定 `externalSourceDetail`) 。 可能的值为： `sis`、 `lms`或 `manual`。 |
| externalSourceDetail | String                                | 生成这些资源的外部源的名称。                                                                                                   |
| highestGrade         | String                                | 教授的最高年级。                                                                                                                                                |
| lowestGrade          | String                                | 教授的最低年级。                                                                                                                                                 |
| phone                | String                                | 学校电话号码。                                                                                                                                              |
| principalEmail       | String                                | 主体的电子邮件地址。                                                                                                                                      |
| principalName        | String                                | 主体名称。                                                                                                                                               |
| schoolNumber         | String                                | 学校编号。                                                                                                                                                       |

## <a name="relationships"></a>关系

| 关系 | 类型                                           | 说明                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| classes      | [educationClass](educationclass.md) 集合 | 在学校教授的课程。 可为 NULL。 |
| users        | [educationUser](educationuser.md) 集合   | 学校中的用户。 可为 Null。          |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


