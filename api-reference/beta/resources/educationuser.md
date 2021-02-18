---
title: educationUser 资源类型
description: 系统中的用户。 这是特定于教育的用户变体，具有 Microsoft Graph 将从非特定于教育的 `/users` 终结点返回的相同 `id`。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 22cdd5acc53de06458dd6ce986d635fc5ade2900
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292992"
---
# <a name="educationuser-resource-type"></a>educationUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

系统中的用户。 这是标准用户资源特定于教育的变体，与[]Microsoft Graph 从非教育特定的终结点返回的变量 `id` `/users` 相同。

此对象提供核心用户对象中属性的目标 [子集，并] 添加一组特定于教育的属性，例如 ， 和 `primaryRole` `student` `teacher` 。

## <a name="methods"></a>方法

| 方法                                               | 返回类型                                  | 说明                                                                   |
| :--------------------------------------------------- | :------------------------------------------- | :---------------------------------------------------------------------------- |
| [Get educationUser](../api/educationuser-get.md)     | [educationUser]                              | 读取 **educationUser** 对象的属性和关系。             |
| [List classes](../api/educationuser-list-classes.md) | [educationClass] 集合                  | 获取 **educationClass** 对象集合，用户是该集合的成员。    |
| [List schools](../api/educationuser-list-schools.md) | [educationSchool] 集合                 | 获取 **educationSchool** 对象集合，用户是该集合的成员。 |
| [Get user](../api/educationuser-get-user.md)         | [user]                                       | 获取与此 **educationUser** 对应的简单目录 **user**。 |
| [Update](../api/educationuser-update.md)             | [educationUser]                              | 更新 **educationUser** 对象。                                           |
| [删除](../api/educationuser-delete.md)             | 无                                         | 删除 **educationUser** 对象。                                           |
| [Delta](../api/educationuser-delta.md)               | [educationUser](educationuser.md) 集合 | 获取 **educationUsers 的增量更改**。                               |

## <a name="properties"></a>属性

| 属性             | 类型                         | 说明                                                                                                                                                                                   |
| :------------------- | :--------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                       | 用户的唯一标识符。继承自 [directoryObject]。键。不可为 null。只读。                                                                                           |
| accountEnabled       | Boolean                      | 如果帐户已启用，则为 **true**；否则，为 **false**。 创建用户时此属性是必需的。 支持 \$ 筛选器。                                                                |
| assignedLicenses     | [assignedLicense] collection | 分配给该用户的许可证。不可为 null。                                                                                                                                     |
| assignedPlans        | [assignedPlan] collection    | 分配给该用户的计划。只读。不可为 null。                                                                                                                             |
| businessPhones       | String collection            | 用户的电话号码。 **注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。                                                             |
| createdBy            | [identitySet]                | 创建了用户的实体。                                                                                                                                                                  |
| department           | String                       | 用户工作部门的名称。 支持 \$ 筛选器。                                                                                                                       |
| displayName          | String                       | 用户通讯簿中显示的名称。 支持 $filter 和 $orderby。                                                                                                           |
| externalSource       | String                       | 此资源的外部源类型由 (自动确定 `externalSourceDetail`) 。 可能的值为： `sis`、 `lms`或 `manual`。                          |
| externalSourceDetail | String                       | 生成这些资源的外部源的名称。                                                                                                                            |
| givenName            | String                       | 用户的名。 支持 \$ 筛选器。                                                                                                                                   |
| mail                 | String                       | 用户的 SMTP 地址；例如，“jeff@contoso.onmicrosoft.com”。 只读。 支持 \$ 筛选器。                                                                                     |
| mailNickname         | String                       | 用户的邮件别名。 创建用户时必须指定此属性。 支持 \$ 筛选器。                                                                                       |
| mailingAddress       | [physicalAddress]            | 用户的邮件地址。 注意 `type` ： `postOfficeBox` 并且不支持资源 `educationUser` 。                                                                                       |
| middleName           | String                       | 用户的中间名。                                                                                                                                                                      |
| mobilePhone          | String                       | 用户的主要移动电话号码。                                                                                                                                           |
| onPremisesInfo       | [educationOnPremisesInfo]    | 用于将 AAD 用户与它的 Active Directory 对应项关联的其他信息。                                                                                                 |
| passwordPolicies     | String                       | 指定用户的密码策略。 有关其他 [详细信息，] 请参阅标准用户资源。                                                                                                |
| passwordProfile      | [passwordProfile]            | 指定用户的密码配置文件。 配置文件包含用户的密码。 创建用户时此属性是必需的。 有关其他 [详细信息，] 请参阅标准用户资源。 |
| preferredLanguage    | String                       | 用户的首选语言。 应遵循 ISO 639-1 代码；例如“en-US”。                                                                                                      |
| primaryRole          | string                       | 用户的默认角色。 用户的角色在各课程中可能有所不同。 可取值为：`student`、`teacher`、`faculty`。 支持 \$ 筛选器。                                  |
| provisionedPlans     | [provisionedPlan] 集合 | 为用户设置的计划。只读。不可为 null。                                                                                                                         |
| relatedContacts      | [relatedContact] 集合  | 与用户相关的记录。 可能的关系是 `parent` ， ， ， ， ， `relative` `aide` `doctor` `guardian` `child` ， `other``unknownFutureValue`                                    |
| residenceAddress     | [physicalAddress]            | 用户所在的地址。 注意 `type` ： `postOfficeBox` 并且不支持资源 `educationUser` 。                                                                                   |
| student              | [educationStudent]           | 如果主要角色为学生，此部分将包含特定于学生的数据。                                                                                                                |
| surname              | String                       | 用户的姓氏。 支持 \$ 筛选器。                                                                                                                             |
| teacher              | [educationTeacher]           | 如果主要角色是教师，则此块将包含教师特定数据。                                                                                                                |
| usageLocation        | String                       | ISO [3166 Alpha-2] (两个字母的国家/) 。 对于将分配许可证的用户，此为必需项。 不可为 null。 支持 \$ 筛选器。                                                            |
| userPrincipalName    | String                       | 用户主体名称 (用户的 UPN) 名称。 支持 $filter 和 $orderby。 有关其他 [详细信息，] 请参阅标准用户资源。                                                               |
| userType             | String                       | 可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。 支持 \$ 筛选器。                                                                    |

> [!IMPORTANT]
> 使用委派权限范围时，Graph 将仅返回一组有限的属性： `id` ， `primaryRole` ， `accountEnabled` ， `displayName` `givenName` `surname` `userPrincipalName` `userType` `onPremisesInfo` 。 `student/externalId` `teacher/externalId` 如果应用程序需要其他属性，则必须使用应用程序权限范围。

## <a name="relationships"></a>关系

| 关系  | 类型                         | 说明                                  |
| :------------ | :--------------------------- | :------------------------------------------- |
| assignments   | [educationAssignment]        | 用户的工作分配列表。 可为 Null。  |
| classes       | [educationClass] 集合  | 用户所属的课程。 可为 NULL。 |
| schools       | [educationSchool] 集合 | 用户所属的学校。 可为 NULL。 |
| taughtClasses | [educationClass] 集合  | 用户是教师的班级。     |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "accountEnabled": true,
  "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
  "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
  "businessPhones": ["String"],
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "department": "String",
  "displayName": "String",
  "externalSource": "string",
  "givenName": "String",
  "id": "String (identifier)",
  "mail": "String",
  "mailNickname": "String",
  "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "middleName": "String",
  "mobilePhone": "String",
  "officeLocation": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  },
  "passwordPolicies": "String",
  "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
  "preferredLanguage": "String",
  "primaryRole": "string",
  "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
  "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
  "student": { "@odata.type": "microsoft.graph.educationStudent" },
  "surname": "String",
  "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]

}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: educationassignment.md
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[user]: user.md
[directoryobject]: directoryobject.md
[educationonpremisesinfo]: educationonpremisesinfo.md
[iso 3166 alpha-2]: https://www.iso.org/obp/ui/#search
[rfc 822]: https://tools.ietf.org/html/rfc822


