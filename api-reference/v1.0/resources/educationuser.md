---
title: educationUser 资源类型
description: 表示系统中的用户。 这是用户的特定于教育的变体，其 ID 与 Microsoft Graph 从非教育特定/用户终结点返回的 ID 相同。
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dbd01d673242a7d12ca4b73e054feae13170c74c
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685227"
---
# <a name="educationuser-resource-type"></a>educationUser 资源类型

命名空间：microsoft.graph

系统中的用户。 这是用户的特定于教育的变体，其 **ID** 与 Microsoft Graph 从非教育特定`/users`终结点返回的 ID 相同。 此对象提供来自核心 [用户](../resources/user.md) 对象的属性的目标子集，并添加一组特定于教育的属性，例如 **primaryRole**、 **学生** 和 **教师** 数据。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods

| 方法                                                           | 返回类型                                                 | 说明                                                                                        |
| :--------------------------------------------------------------- | :---------------------------------------------------------- | :------------------------------------------------------------------------------------------------- |
| [列出 educationUsers](../api/educationuser-list.md)              | [educationUser](../resources/educationuser.md) 集合   | 获取 [educationUser](../resources/educationuser.md) 对象及其属性的列表。     |
| [Create educationUser](../api/educationuser-post.md)             | [educationUser](../resources/educationuser.md)              | 创建新的 [educationUser](../resources/educationuser.md) 对象。                                |
| [Get educationUser](../api/educationuser-get.md)                 | [educationUser](../resources/educationuser.md)              | 读取 [educationUser](../resources/educationuser.md) 对象的属性和关系。 |
| [更新 educationUser](../api/educationuser-update.md)           | [educationUser](../resources/educationuser.md)              | 更新 [educationUser](../resources/educationuser.md) 对象的属性。                 |
| [删除 educationUser](../api/educationuser-delete.md)           | 无                                                        | 删除 [educationUser](../resources/educationuser.md) 对象。                                   |
| [delta](../api/educationuser-delta.md)                           | [educationUser](../resources/educationuser.md) 集合   | 获取对资源集合的增量更改。                                                |
| [列出 taughtClasses](../api/educationuser-list-taughtclasses.md) | [educationClass](../resources/educationclass.md) 集合 | 从 **taughtClasses** 导航属性获取 **educationClass** 资源。                       |

## <a name="properties"></a>属性

| 属性             | 类型                                                               | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :------------------- | :----------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | Boolean                                                            | 启用帐户时为 `True`，否则为 `false`。 创建用户时此属性是必需的。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedLicenses     | [assignedLicense](../resources/assignedlicense.md) collection      | 分配给该用户的许可证。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| assignedPlans        | [assignedPlan](../resources/assignedplan.md) collection            | 分配给该用户的计划。只读。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| businessPhones       | String collection                                                  | 用户的电话号码。 **注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。                                                                                                                                                                                                                                                                                                                                                                                                        |
| createdBy            | [identitySet](../resources/identityset.md)                         | 创建用户的实体。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| department           | String                                                             | 用户工作部门的名称。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| displayName          | String                                                             | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 支持 `$filter` 和 `$orderby`。                                                                                                                                                                                                                                                               |
| externalSource       | educationExternalSource                                            | 创建此用户的位置。 可取值为：`sis`、`manual`。                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| externalSourceDetail | String                                                             | 从中生成此资源的外部源的名称。                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| givenName            | String                                                             | 用户的名。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| id                   | 字符串                                                             | 对象标识符。 继承自 [entity](../resources/entity.md)。                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| mail                 | String                                                             | 用户的 SMTP 地址，例如， `jeff@contoso.onmicrosoft.com`。 只读。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | 用户的邮件地址。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| mailNickname         | String                                                             | 用户的邮件别名。 创建用户时必须指定此属性。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| middleName           | String                                                             | 用户的中间名。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| mobilePhone          | String                                                             | 用户的主要移动电话号码。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | 用于将Azure Active Directory用户与其 Active Directory 对应用户关联的其他信息。                                                                                                                                                                                                                                                                                                                                                                                                                          |
| passwordPolicies     | String                                                             | 指定用户的密码策略。 此值表示枚举，其中一个可能 `DisableStrongPassword`为枚举值，允许指定超过默认策略的密码。 `DisablePasswordExpiration` 也可以指定 。 两者可以一起指定;例如： `DisablePasswordExpiration, DisableStrongPassword`.                                                                                                                                                                              |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | 指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。                                                                                                                                                                                                                                      |
| preferredLanguage    | String                                                             | 例如 `en-US`，应遵循 ISO 639-1 代码的用户首选语言。                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| primaryRole          | educationUserRole                                                  | 用户的默认角色。 用户的角色在各课程中可能有所不同。 可能的值是：`student`、`teacher`、`none`、`unknownFutureValue`。                                                                                                                                                                                                                                                                                                                                                                             |
| provisionedPlans     | [provisionedPlan](../resources/provisionedplan.md) 集合      | 为用户设置的计划。只读。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| relatedContacts      | [relatedContact] 集合                                        | 与用户关联的相关记录。 只读。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | 用户所在的地址。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| showInAddressList    | Boolean                                                            | `True`如果Outlook全局地址列表应包含此用户，则为 >;否则为 `false`。 如果未设置，则将其视为 `true`。 对于通过邀请管理器邀请的用户，此属性将设置为 `false`。                                                                                                                                                                                                                                                                                                               |
| student              | [educationStudent](../resources/educationstudent.md)               | 如果主要角色为学生，此部分将包含特定于学生的数据。                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| surname              | String                                                             | 用户的姓氏。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | 如果主要角色是教师，则此块将包含教师特定的数据。                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| usageLocation        | String                                                             | 两个字母组成的国家/地区代码（ISO 标准 3166）。 鉴于检查服务在国家/地区的可用性的法律要求，这对将分配许可证的用户而言是必需的。 示例包括： `US`、 `JP`和 `GB`。 不可为 null。 支持 `$filter`。                                                                                                                                                                                                                                                                      |
| userPrincipalName    | String                                                             | 用户的用户主体名称 (UPN)。 UPN 是基于 Internet 标准 RFC 822 的用户的 Internet 样式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 `alias@domain`，域必须存在于租户的已验证域集合中。 创建用户时此属性是必需的。 可以从 [组织的](organization.md) **verifiedDomains** 属性访问租户的已验证域。 支持 `$filter` 和 `$orderby`。 |
| userType             | String                                                             | 可用于对目录中的用户类型进行分类的字符串值，例如`Member``Guest`。 支持 `$filter`。                                                                                                                                                                                                                                                                                                                                                                                                              |

> [!IMPORTANT]
> 使用委派权限范围时，Microsoft Graph将仅返回一组有限的属性：**id**、**primaryRole**、**accountEnabled**、**displayName**、**givenName**、**surname**、**userPrincipalName**、**userType**、**onPremisesInfo**、**student/externalId**、**teacher/externalId**。 如果应用程序需要其他属性，则必须使用应用程序权限范围。

## <a name="relationships"></a>关系


| 关系  | 类型                                                          | 说明                                    |
| :------------ | :------------------------------------------------------------ | :--------------------------------------------- |
| assignments   | [educationAssignment](../resources/educationassignment.md) 集合   | 属于用户的分配。   |
| classes       | [educationClass](../resources/educationclass.md) 集合   | 用户所属的课程。 可为 NULL。   |
| schools       | [educationSchool](../resources/educationschool.md) 集合 | 用户所属的学校。 可为 NULL。   |
| taughtClasses | [educationClass](../resources/educationclass.md) 集合   | 用户是教师的课程。       |
| 用户          | [user](../resources/user.md)                                  | 与此用户对应的目录用户。 |
|rubrics|[educationRubric](educationrubric.md) 集合|设置后，附加到分配的分级红宝石。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "String (identifier)",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": "Boolean",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": ["String"],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo"
  }
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
[user]: user.md
[directoryobject]: directoryobject.md
