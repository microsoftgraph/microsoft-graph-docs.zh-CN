---
title: 更新用户
description: 更新 user 对象的属性。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 98b69fc8cb5275055e3c990ddb9bd2bbe443a0a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961173"
---
# <a name="update-user"></a>更新用户

命名空间：microsoft.graph

更新 user 对象的属性。 并非所有属性都可以在没有管理员角色的情况下由具有其默认权限的成员或来宾用户更新。 [比较成员和来宾默认](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) 权限，查看其可管理的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite、User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | User.ReadWrite    |
|应用程序 | User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All |

>[!NOTE]
> - 更新 **passwordProfile** 属性时，需要以下权限：Directory.AccessAsUser.All。
> - 如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。 有关详细信息，请参阅 [Azure AD 内置角色帮助人员（密码）](/azure/active-directory/roles/permissions-reference)。  这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。
> - 个人 Microsoft 帐户必须绑定到 AAD 租户，才能使用 User.ReadWrite 对个人 Microsoft 帐户的委派权限更新配置文件。
> - 更新 **identities** 属性需要 User.ManageIdentities.All 权限。 此外，不允许将 [B2C 本地帐户](../resources/objectidentity.md)添加到现有 **user** 对象，除非 **user** 对象已包含本地帐户标识。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a>请求标头
| 标头       | 值|
|:-----------|:------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|aboutMe|String|任意形式的文本输入字段，用于介绍用户自身。|
|accountEnabled|Boolean| 启用帐户时为 `true`，否则为 `false`。 创建用户时此属性是必需的。    |
| ageGroup | [ageGroup](../resources/user.md#agegroup-values) | 设置用户的年龄组。 允许的值：`null`、`minor`、`notAdult` 和 `adult`。 请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。 |
|birthday|DateTimeOffset|用户的生日。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|businessPhones| String collection | 用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。|
|城市|String|用户所在的城市。|
| companyName | String | 与用户关联的公司名称。 此属性可用于描述外部用户所属的公司。 公司名称的最大长度为 64 个字符。 |
| consentProvidedForMinor | [consentProvidedForMinor](../resources/user.md#consentprovidedforminor-values) | 设置是否已获得未成年人的同意。 允许的值：`null`、`granted`、`denied` 和 `notRequired`。 请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。 |
|country|String|用户所在的国家/地区;例如， `US` 或 `UK`。|
|department|String|用户工作部门的名称。|
|displayName|String|用户通讯簿中显示的名称。 这通常是用户名字、中间名首字母和姓氏的组合。 此属性在创建用户时是必需的，并且在更新过程中不能清除。 支持 `$filter` 和 `$orderby`。|
| employeeId | String | 由组织分配给该用户的员工标识符。 |
|givenName|String|用户的名。|
|hireDate|DateTimeOffset|用户的雇佣日期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|interests|String collection|用户介绍自身兴趣的列表。|
|jobTitle|String|用户的职务。|
|mail|String|用户的 SMTP 地址，例如， `jeff@contoso.onmicrosoft.com`。 对此属性的更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。 <br><br>支持 `$filter`。|
|mailNickname|String|用户的邮件别名。 创建用户时必须指定此属性。|
|mobilePhone|String|用户的主要移动电话号码。|
|mySite|String|用户个人网站的 URL。|
|officeLocation|String|用户公司地点的办公室位置。|
|onPremisesImmutableId|String|此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。 如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。 **重要说明：** 指定此属性时不能使用 **$** 和 **_** 字符。                            |
|otherMails|String |用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。|
|passwordPolicies|String|指定用户的密码策略。 此值表示枚举，其中一个可能 `DisableStrongPassword`为枚举值，允许指定超过默认策略的密码。 `DisablePasswordExpiration` 也可以指定 。 可同时指定两者;例如： `DisablePasswordExpiration, DisableStrongPassword`。|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|指定用户的密码配置文件。 配置文件包含用户的密码。 创建用户时此属性是必需的。 配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。 默认情况下，必须使用强密码。 这不能用于联合用户。|
|pastProjects|String collection|供用户枚举其过去项目的列表。|
|postalCode|String|用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。|
|preferredLanguage|String|用户的首选语言。 应遵循 ISO 639-1 代码;例如， `en-US`。|
|responsibilities|String collection|供用户枚举其职责的列表。|
|schools|String collection|供用户枚举其学习过的学校列表。|
|skills|String collection|供用户枚举其技能的列表。|
|state|String|用户地址中的省/市/自治区或省。|
|streetAddress|String|用户公司地点的街道地址。|
|surname|String|用户的姓氏。|
|usageLocation|String|两个字母的国家/地区代码（ISO 标准 3166）。 为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。  示例包括： `US`、 `JP`和 `GB`。 不可为 null。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。 支持 `$filter` 和 `$orderby`。
|userType|String|可用于对目录中的用户类型进行分类的字符串值，例如`Member``Guest`。          |

> [!NOTE] 
> 以下属性无法使用仅限应用程序上下文进行更新：**aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools**, and **skills**。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="example-1-update-properties-of-the-signed-in-user"></a>示例 1：更新已登录用户的属性

#### <a name="request"></a>请求

以下示例显示了一个请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
以下示例显示了相应的响应。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a>示例 2：更新指定用户的属性

#### <a name="request"></a>请求

以下示例显示了一个请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例显示了相应的响应。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
