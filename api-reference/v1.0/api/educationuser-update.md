---
title: 更新 educationUser
description: 更新 educationUser 对象的属性。
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 002b61a29a245902e458a70c03aacc4982b9d2ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024596"
---
# <a name="update-educationuser"></a>更新 educationUser

命名空间：microsoft.graph

更新 [educationUser 对象](../resources/educationuser.md) 的属性。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  不支持。  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性             | 类型                                                               | 说明                                                                                                                                                                                                                                                                                                                                                 |
| :------------------- | :----------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled       | 布尔                                                            | 如果帐户已启用，则为 **true**；否则，为 **false**。 创建用户时此属性是必需的。 支持 $filter。                                                                                                                                                                                                                               |
| assignedLicenses     | [assignedLicense](../resources/assignedlicense.md) collection      | 分配给该用户的许可证。不可为 null。                                                                                                                                                                                                                                                                                                   |
| assignedPlans        | [assignedPlan](../resources/assignedplan.md) collection            | 分配给该用户的计划。只读。不可为 null。                                                                                                                                                                                                                                                                                           |
| businessPhones       | String collection                                                  | 用户的电话号码。 **注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。                                                                                                                                                                                                                           |
| createdBy            | [identitySet](../resources/identityset.md)                         | 创建了用户的实体。                                                                                                                                                                                                                                                                                                                                |
| department           | String                                                             | 用户工作部门的名称。支持 $filter。                                                                                                                                                                                                                                                                                      |
| displayName          | String                                                             | 用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 支持 $filter 和 $orderby。                                                                                      |
| externalSource       | educationExternalSource                                            | 创建此用户的位置。 可取值为：`sis`、`manual`。                                                                                                                                                                                                                                                                                     |
| externalSourceDetail | String                                                             | 生成此资源的外部源的名称。                                                                                                                                                                                                                                                                                          |
| givenName            | String                                                             | 用户的名。支持 $filter。                                                                                                                                                                                                                                                                                                  |
| mail                 | String                                                             | 用户的 SMTP 地址；例如，“jeff@contoso.onmicrosoft.com”。 只读。 支持 $filter。                                                                                                                                                                                                                                                    |
| mailingAddress       | [physicalAddress](../resources/physicaladdress.md)                 | 用户的邮件地址。                                                                                                                                                                                                                                                                                                                                       |
| mailNickname         | String                                                             | 用户的邮件别名。创建用户时必须指定此属性。支持 $filter。                                                                                                                                                                                                                                                      |
| middleName           | String                                                             | 用户的中间名。                                                                                                                                                                                                                                                                                                                                    |
| mobilePhone          | String                                                             | 用户的主要移动电话号码。                                                                                                                                                                                                                                                                                                         |
| onPremisesInfo       | [educationOnPremisesInfo](../resources/educationonpremisesinfo.md) | 用于将用户与 AAD对应的 Active Directory 关联的其他信息。                                                                                                                                                                                                                                                               |
| passwordPolicies     | String                                                             | 指定用户的密码策略。 此值是一个枚举，具有一个可能值 “DisableStrongPassword”，允许指定比默认策略弱的密码。 还可以指定 “DisablePasswordExpiration”。 可以同时指定两个值；例如：“DisablePasswordExpiration、DisableStrongPassword”。 |
| passwordProfile      | [passwordProfile](../resources/passwordprofile.md)                 | 指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。                                                         |
| preferredLanguage    | String                                                             | 用户的首选语言。 应遵循 ISO 639-1 代码；例如“en-US”。                                                                                                                                                                                                                                                                    |
| primaryRole          | educationUserRole                                                  | 用户的默认角色。 用户的角色在各课程中可能有所不同。 可能的值是：`student`、`teacher`、`none`、`unknownFutureValue`。                                                                                                                                                                                                |
| provisionedPlans     | [provisionedPlan](../resources/provisionedplan.md) 集合      | 为用户设置的计划。只读。不可为 null。                                                                                                                                                                                                                                                                                       |
| residenceAddress     | [physicalAddress](../resources/physicaladdress.md)                 | 用户所在的地址。                                                                                                                                                                                                                                                                                                                                   |
| student              | [educationStudent](../resources/educationstudent.md)               | 如果主要角色为学生，此部分将包含特定于学生的数据。                                                                                                                                                                                                                                                                              |
| surname              | String                                                             | 用户的姓氏。支持 $filter。                                                                                                                                                                                                                                                                                            |
| teacher              | [educationTeacher](../resources/educationteacher.md)               | 如果主要角色是教师，则此块将包含特定于教师的数据。                                                                                                                                                                                                                                                                              |
| usageLocation        | String                                                             | 两个字母组成的国家/地区代码（ISO 标准 3166）。 鉴于检查服务在国家/地区的可用性的法律要求，这对将分配许可证的用户而言是必需的。 示例包括：“US”、“JP”和“GB”。 不可为 null。 支持 $filter。                                                                                           |
| userPrincipalName    | String                                                             | 用户的用户主体名称 (UPN)。                                                                                                                                                                                                                                                                                                                  |
| userType             | String                                                             | 可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。                                                                                                                                                                                                                                   |

## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
