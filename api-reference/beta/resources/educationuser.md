---
title: educationUser 资源类型
description: 系统中的用户。 这是特定于教育的用户变体，具有 Microsoft Graph 将从非特定于教育的 `/users` 终结点返回的相同 `id`。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 21119c6a99420c0b3b8b9a941f73cc4de1a2c121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990773"
---
# <a name="educationuser-resource-type"></a>educationUser 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

系统中的用户。 这是特定于教育的用户变体，具有 Microsoft Graph 将从非特定于教育的 `/users` 终结点返回的相同 `id`。
此对象提供来自核心 [user](user.md) 对象的目标属性子集，并添加一组特定于教育的属性，如 `primaryRole`、学生和教师数据。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get educationUser](../api/educationuser-get.md) | [educationUser](educationuser.md) |读取 **educationUser** 对象的属性和关系。|
|[List classes](../api/educationuser-list-classes.md) |[educationClass](educationclass.md) 集合| 获取 **educationClass** 对象集合，用户是该集合的成员。|
|[List schools](../api/educationuser-list-schools.md) |[educationSchool](educationschool.md) 集合| 获取 **educationSchool** 对象集合，用户是该集合的成员。|
|[Get user](../api/educationuser-get-user.md) |[user](user.md)| 获取与此 **educationUser** 对应的简单目录 **user**。|
|[Update](../api/educationuser-update.md) | [educationUser](educationuser.md)   |更新 **educationUser** 对象。 |
|[Delete](../api/educationuser-delete.md) | 无 |删除 **educationUser** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 如果帐户已启用，则为 **true**；否则，为 **false**。 创建用户时此属性是必需的。 支持 $filter。    |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|分配给该用户的许可证。不可为 null。            |
|assignedPlans|[assignedPlan](assignedplan.md) 集合|分配给该用户的计划。只读。不可为 null。 |
|businessPhones|String collection|用户的电话号码。 **注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。|
|createdBy|[identitySet](identityset.md)| 创建了用户的实体。 |
|department|字符串|用户工作部门的名称。支持 $filter。|
|displayName|String|用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 支持 $filter 和 $orderby。|
|externalSource|`educationExternalSource`| 创建此用户的位置。 可取值为：`sis`、`manual`、`unkownFutureValue`。|
|givenName|字符串|用户的名字。支持 $filter。|
|id|String|用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。|
|mail|String|用户的 SMTP 地址；例如，“jeff@contoso.onmicrosoft.com”。 只读。 支持 $filter。|
|mailingAddress|[physicalAddress](physicaladdress.md)| 用户的邮件地址。|
|mailNickname|字符串|用户的邮件别名。创建用户时必须指定此属性。支持 $filter。|
|middleName| String | 用户的中间名。|
|mobilePhone|String|用户的主要移动电话号码。|
|passwordPolicies|String|指定用户的密码策略。 此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。 另外，还可以指定“DisablePasswordExpiration”。 可以同时指定两个值；例如：“DisablePasswordExpiration、DisableStrongPassword”。|
|passwordProfile|[PasswordProfile](passwordprofile.md)|指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。|
|preferredLanguage|String|用户的首选语言。 应遵循 ISO 639-1 代码；例如“en-US”。|
|primaryRole|string| 用户的默认角色。 用户的角色在各课程中可能有所不同。 可取值为：`student`、`teacher`、`enum_sentinel`。 支持 $filter。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) 集合|为用户预配的计划。只读。不可为 null。 |
|residenceAddress|[physicalAddress](physicaladdress.md)| 用户所在的地址。|
|student|[educationStudent](educationstudent.md)| 如果主要角色为学生，此部分将包含特定于学生的数据。|
|surname|字符串|用户的姓氏。支持 $filter。|
|teacher|[educationTeacher](educationteacher.md)| 如果主要角色为教师，此部分将包含特定于教师的数据。|
|usageLocation|String|两个字母组成的国家/地区代码（ISO 标准 3166）。 鉴于检查服务在国家/地区的可用性的法律要求，这对将分配许可证的用户而言是必需的。 示例包括：“US”、“JP”和“GB”。 不可为 null。 支持 $filter。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。
|userType|字符串|可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。          |

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) 集合| 用户所属的课程。 可为 NULL。|
|schools|[educationSchool](educationschool.md) 集合| 用户所属的学校。 可为 NULL。|
|assignments| [educationAssignment](educationassignment.md)| 用户的分配列表。 可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "primaryRole": "string",
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
