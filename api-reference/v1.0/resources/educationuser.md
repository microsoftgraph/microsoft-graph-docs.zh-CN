---
title: educationUser 资源类型
description: 系统中的用户。 这是特定于教育的用户变体，具有 Microsoft Graph 将从非特定于教育的 `/users` 终结点返回的相同 `id`。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ca45981d2825769f540048a94488dda4ba91c00
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115190"
---
# <a name="educationuser-resource-type"></a>educationUser 资源类型

命名空间：microsoft.graph

系统中的用户。 这是特定于教育的用户变体，具有 Microsoft Graph 将从非特定于教育的 `/users` 终结点返回的相同 `id`。
此对象提供来自核心 [user] 对象的目标属性子集，并添加一组特定于教育的属性，如 `primaryRole`、学生和教师数据。

## <a name="methods"></a>方法

| 方法                                               | 返回类型                  | 说明                                                                   |
| :--------------------------------------------------- | :--------------------------- | :---------------------------------------------------------------------------- |
| [Get educationUser](../api/educationuser-get.md)     | [educationUser]              | 读取 **educationUser** 对象的属性和关系。             |
| [List classes](../api/educationuser-list-classes.md) | [educationClass] 集合  | 获取 **educationClass** 对象集合，用户是该集合的成员。    |
| [List schools](../api/educationuser-list-schools.md) | [educationSchool] 集合 | 获取 **educationSchool** 对象集合，用户是该集合的成员。 |
| [Get user](../api/educationuser-get-user.md)         | [user]                       | 获取与此 **educationUser** 对应的简单目录 **user**。 |
| [Update](../api/educationuser-update.md)             | [educationUser]              | 更新 **educationUser** 对象。                                           |
| [删除](../api/educationuser-delete.md)             | 无                         | 删除 **educationUser** 对象。                                           |

## <a name="properties"></a>属性

| 属性          | 类型                         | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| :---------------- | :--------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled    | 布尔                      | 如果帐户已启用，则为 **true**；否则，为 **false**。 创建用户时此属性是必需的。 支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                    |
| assignedLicenses  | [assignedLicense] collection | 分配给该用户的许可证。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| assignedPlans     | [assignedPlan] collection    | 分配给该用户的计划。只读。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| businessPhones    | String collection            | 用户的电话号码。 **注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。                                                                                                                                                                                                                                                                                                                                                                                                |
| createdBy         | [identitySet]                | 创建了用户的实体。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| department        | String                       | 用户工作部门的名称。支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| displayName       | String                       | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 支持 $filter 和 $orderby。                                                                                                                                                                                                                                                           |
| externalSource    | `educationExternalSource`    | 创建此用户的位置。 可能的值是： `sis` `manual` 。                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| givenName         | String                       | 用户的名。支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| id                | String                       | 用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。                                                                                                                                                                                                                                                                                                                                                                                                          |
| mail              | String                       | 用户的 SMTP 地址；例如，“jeff@contoso.onmicrosoft.com”。 只读。 支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mailingAddress    | [physicalAddress]            | 用户的邮件地址。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| mailNickname      | String                       | 用户的邮件别名。创建用户时必须指定此属性。支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                                           |
| middleName        | String                       | 用户的中间名。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| mobilePhone       | String                       | 用户的主要移动电话号码。                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| passwordPolicies  | String                       | 指定用户的密码策略。 此值是一个枚举，具有一个可能值 “DisableStrongPassword”，允许指定比默认策略弱的密码。 还可以指定 “DisablePasswordExpiration”。 可以同时指定两个值；例如：“DisablePasswordExpiration、DisableStrongPassword”。                                                                                                                                                                      |
| passwordProfile   | [PasswordProfile]            | 指定用户的密码配置文件。 配置文件包含用户的密码。 创建用户时此属性是必需的。 配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。 默认情况下，必须使用强密码。                                                                                                                                                                                                                             |
| preferredLanguage | String                       | 用户的首选语言。 应遵循 ISO 639-1 代码；例如“en-US”。                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| primaryRole       | educationUserRole            | 用户的默认角色。 用户的角色在各课程中可能有所不同。 可能的值是： `student` `teacher` 。 支持 $filter。                                                                                                                                                                                                                                                                                                                                                                             |
| provisionedPlans  | [ProvisionedPlan] collection | 为用户设置的计划。只读。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| residenceAddress  | [physicalAddress]            | 用户所在的地址。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| student           | [educationStudent]           | 如果主要角色为学生，此部分将包含特定于学生的数据。                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| surname           | String                       | 用户的姓氏。支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| teacher           | [educationTeacher]           | 如果主要角色是教师，则此块将包含教师特定数据。                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| usageLocation     | String                       | 两个字母组成的国家/地区代码（ISO 标准 3166）。 鉴于检查服务在国家/地区的可用性的法律要求，这对将分配许可证的用户而言是必需的。 示例包括：“US”、“JP”和“GB”。 不可为 null。 支持 $filter。                                                                                                                                                                                                                                                                |
| userPrincipalName | String                       | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中 domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。 支持 $filter 和 $orderby。 |
| userType          | String                       | 可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。                                                                                                                                                                                                                                                                                                                                                                                                        |

## <a name="relationships"></a>关系

| 关系 | 类型                         | 说明                                    |
| :----------- | :--------------------------- | :--------------------------------------------- |
| classes      | [educationClass] 集合  | 用户所属的课程。 可为 NULL。   |
| schools      | [educationSchool] 集合 | 用户所属的学校。 可为 NULL。   |
| assignments  | [educationAssignment]        | 用户的工作分配列表。 可为 NULL。    |
| user         | [用户]                       | 与此用户对应的目录用户。 |

>[!IMPORTANT]
>**[educationAssignment]** 资源是 /beta 版本资源。 如果使用此资源，请务必定期查看[更改日志](/graph/changelog)。 当 Microsoft Graph API 资源释放到 /v1.0 终结点时，更改日志中会记录该版本。 如果你的应用使用 **educationAssignment** 资源，你将需要声明基本请求 URL，如以下代码块所示：  
>
>```JavaScript
>var v1BaseUrl = "https://graph.microsoft.com/v1.0/education";
>var betaBaseUrl = "https://graph.microsoft.com/beta/education";  // for administrativeUnit and educationOrganization
>```

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["555-555-6568"],
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "preferredLanguage": "string",
  "primaryRole": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"},
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: microsoft.graph.educationUser/assignments:
      Referenced type microsoft.graph.educationAssignment is not defined in the doc set! Potential suggestion: UNKNOWN",
    "Warning: /api-reference/v1.0/resources/educationuser.md/microsoft.graph.educationUser:
      Property 'relatedContacts' found in markdown table but not in resource definition."
  ],
  "tocPath": ""
}-->

[educationuser]: educationuser.md
[educationclass]: educationclass.md
[educationschool]: educationschool.md
[educationassignment]: /graph/api/resources/educationassignment?view=graph-rest-beta
[educationteacher]: educationteacher.md
[educationstudent]: educationstudent.md
[relatedcontact]: relatedcontact.md
[physicaladdress]: physicaladdress.md
[provisionedplan]: provisionedplan.md
[passwordprofile]: passwordprofile.md
[identityset]: identityset.md
[assignedplan]: assignedplan.md
[assignedlicense]: assignedlicense.md
[用户]: user.md
[directoryobject]: directoryobject.md

