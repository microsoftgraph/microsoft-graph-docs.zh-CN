---
title: educationSchool 资源类型
description: '一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 407f29c7d8f9468c5e9b1da1badad294cb655121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531512"
---
# <a name="educationschool-resource-type"></a>educationSchool 资源类型

命名空间：microsoft.graph

一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  

## <a name="methods"></a>Methods

| 方法                                                   | 返回类型                                    | 说明                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [Get](../api/educationschool-get.md)                     | [educationSchool](educationschool.md)          | 读取 **educationSchool** 对象的属性和关系。                         |
| [Add class](../api/educationschool-post-classes.md)      | [educationClass](educationclass.md)            | 通过发布到课程导航属性，为学校添加一个新的 **educationClass**。  |
| [List classes](../api/educationschool-list-classes.md)   | [educationClass](educationclass.md) 集合 | 获取 **educationClass** 对象集合。                                               |
| [Remove class](../api/educationschool-delete-classes.md) | [educationClass](educationclass.md)            | 通过课程导航属性从学校删除 **educationClass**。       |
| [Add user](../api/educationschool-post-users.md)         | [educationUser](educationuser.md)              | 通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。 |
| [List users](../api/educationschool-list-users.md)       | [educationUser](educationuser.md) 集合   | 获取 **educationUser** 对象集合。                                                |
| [Remove user](../api/educationschool-delete-users.md)    | [educationUser](educationuser.md)              | 通过 **users** 导航属性从学校删除 **educationUser**。      |
| [Update](../api/educationschool-update.md)               | [educationSchool](educationschool.md)          | 更新 **educationSchool** 对象。                                                       |
| [删除](../api/educationschool-delete.md)               | 无                                           | 删除 **educationSchool** 对象。                                                       |

## <a name="properties"></a>属性

| 属性            | 类型                                  | 说明                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| id                  | String                                | 该学校的 GUID。                                                               |
| displayName         | 字符串                                | 学校的显示名称。                                                        |
| 说明         | 字符串                                | 学校描述。                                                         |
| 状态              | string                                | 只读。 可能的值包括 `inactive`、`active`、`expired`、`deleteable`。 |
| externalSource      | educationExternalSource               | 只读。  可能的值包括 `sis`、`manual`、`unknownFutureValue`。        |
| principalEmail      | 字符串                                | 主体的电子邮件地址。                                                    |
| principalName       | 字符串                                | 主体名称。                                                             |
| externalPrincipalId | 字符串                                | 同步系统中主体的 ID。                                                 |
| highestGrade        | 字符串                                | 教授的最高年级。                                                              |
| lowestGrade         | 字符串                                | 教授的最低年级。                                                               |
| schoolNumber        | 字符串                                | 学校编号。                                                                     |
| externalId          | String                                | 同步系统中学校的 ID。                                                    |
| phone               | String                                | 学校电话号码。                                                            |
| address             | [physicalAddress](physicaladdress.md) | 学校地址。                                                             |
| createdBy           | [identitySet](identityset.md)         | 创建了学校的实体。                                                     |

## <a name="relationships"></a>关系

| 关系 | 类型                                           | 说明                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| classes      | [educationClass](educationclass.md) 集合 | 在学校教授的课程。 可为 NULL。 |
| users        | [educationUser](educationuser.md) 集合   | 学校中的用户。 可为 Null。          |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
