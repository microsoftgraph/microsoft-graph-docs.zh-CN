---
title: 更新用户
description: 更新 user 对象的属性。
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d21f2a4e25ff42f37df238fc2304d52f825c40f4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334483"
---
# <a name="update-user"></a>更新用户

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [user](../resources/user.md) 对象的属性。 并非所有属性都可以在没有管理员角色的情况下由具有其默认权限的成员或来宾用户更新。 [比较成员和来宾默认](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) 权限，查看其可管理的属性。

## <a name="permissions"></a>权限
若要调用此 API，需要以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite、User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | User.ReadWrite    |
|应用程序 | User.ReadWrite.All、User.ManageIdentities.All、Directory.ReadWrite.All |

>[!NOTE]
> - 如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。 有关详细信息，请参阅 [Azure AD 内置角色帮助人员（密码）](/azure/active-directory/roles/permissions-reference)。  这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。 只有分配了 Directory.AccessAsUser.All 权限的全局管理员才能为更多特权管理员更新这些属性。
> - 个人 Microsoft 帐户必须绑定到 AAD 租户，才能使用 User.ReadWrite 对个人 Microsoft 帐户的委派权限更新配置文件。
> - 更新 **标识** 属性需要 User.ManageIdentities.All 权限。此外，不允许将 [B2C 本地帐户](../resources/objectidentity.md)添加到现有 **用户** 对象，除非 **用户** 对象已包含本地帐户标识。

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
|accountEnabled|Boolean| 启用帐户时为 `true`，否则为 `false`。 创建用户时此属性是必需的。 分配了 _Directory.AccessAsUser.All_ 委派权限的全局管理员可以更新租户中所有管理员的 **accountEnabled** 状态。|
| ageGroup | [ageGroup](../resources/user.md#agegroup-values) | 设置用户的年龄组。 允许的值：`null`、`Minor`、`NotAdult` 和 `Adult`。 请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。 |
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|分配给该用户的许可证。不可为 null。            |
|birthday|DateTimeOffset|用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|businessPhones| String collection | 用户的电话号码。 **注意：** 虽然这是一个字符串集合，但只能为此属性设置一个数字。|
|城市|String|用户所在的城市。|
| CompanyName | String | 与用户关联的公司名称。 此属性可用于描述外部用户所属的公司。 最大长度为 64 个字符。 |
| consentProvidedForMinor | [consentProvidedForMinor](../resources/user.md#consentprovidedforminor-values) | 设置是否已获得未成年人的同意。 允许的值：`null`、`Granted`、`Denied` 和 `NotRequired`。 请参阅[法定年龄组属性定义](../resources/user.md#legal-age-group-property-definitions)以了解详细信息。 |
|country|String|用户所在的国家/地区;例如， `US` 或 `UK`。|
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|保留分配给目录对象的自定义安全属性的值的开放式复杂类型。<br/><br/>若要更新此属性，必须为调用主体分配"属性分配管理员"角色，并且必须向其授予 *CustomSecAttributeAssignment.ReadWrite.All* 权限。|
|department|String|用户工作部门的名称。|
|displayName|String|用户通讯簿中显示的名称，通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。|
|employeeId|String|由组织分配给该用户的员工标识符。 最大长度为 16 个字符。|
| employeeType | String | 捕获企业员工类型。 例如，`Employee`、`Contractor`、`Consultant` 或 `Vendor`。|
|givenName|String|用户的名。|
|employeeHireDate|DateTimeOffset|用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|identities|[objectIdentity](../resources/objectidentity.md) 集合| 表示可用于登录此用户帐户的标识。 标识可由 Microsoft、组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供，并绑定到用户帐户。 对标识 **的任何** 更新都将替换整个集合，并且您必须在集合中提供 userPrincipalName **signInType** 标识。|
|interests|String collection|用户介绍自身兴趣的列表。|
|jobTitle|String|用户的职务。|
|mail|String|用户的 SMTP 地址，例如， `jeff@contoso.onmicrosoft.com`。 对于 Azure AD B2C 帐户，此属性最多可以使用唯一的 SMTP 地址更新 10 次。 对此属性的更改也将更新用户的 **proxyAddresses** 集合，以便将该值包含为 SMTP 地址。|
|mailNickname|String|用户的邮件别名。创建用户时必须指定此属性。|
|mobilePhone|String|用户的主要移动电话号码。|
|mySite|String|用户个人网站的 URL。|
|officeLocation|String|用户公司地点的办公室位置。|
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md) | 包含用户的 extensionAttributes 1-15。 请注意，单个扩展属性既不可选择，也不可筛选。 对于 `onPremisesSyncEnabled` 用户，这组属性集的授权来源是本地，并且为只读。 这些扩展属性也称 Exchange 自定义属性 1-15。|
|onPremisesImmutableId|String|此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，在 Graph 中创建新用户帐户时必须指定此属性。**重要事项：** 指定该属性时不能使用 **$** 和 **_** 字符。                            |
|otherMails|字符串集合|用户的其他电子邮件地址列表；例如：`["bob@contoso.com", "Robert@fabrikam.com"]`。|
|passwordPolicies|String|指定用户的密码策略。此值是一个枚举，其中一个可能的值为 `DisableStrongPassword`，这允许指定比默认策略更弱的密码。也可指定 `DisablePasswordExpiration`。两者可以一起指定，例如：`DisablePasswordExpiration, DisableStrongPassword`。|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。<br><br>必须为调用用户分配 *Directory.AccessAsUser.All* 委派权限才能更新此属性。 无法仅使用应用程序权限更新此属性。|
|pastProjects|String collection|供用户枚举其过去项目的列表。|
|postalCode|String|用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。|
|preferredLanguage|String|用户的首选语言。应遵循 ISO 639-1 代码，例如 `en-US`。 |
|responsibilities|String collection|供用户枚举其职责的列表。|
|schools|String collection|供用户枚举其学习过的学校列表。|
|skills|String collection|供用户枚举其技能的列表。|
|state|String|用户地址中的省/市/自治区或省。|
|streetAddress|String|用户公司地点的街道地址。|
|surname|String|用户的姓氏。|
|usageLocation|String|两个字母的国家/地区代码（ISO 标准 3166）。 由于法律要求，将被分配许可证的用户需要检查国家/地区的服务可用性。 示例包括：`US`、`JP`、`GB`。不可为 null。 |
|userPrincipalName|String|用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中 domain 必须位于租户的已验证域集合中。 可从 [组织](../resources/organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。 <br>注意：此属性不能包含突出字符。 仅支持使用以下字符：`A - Z`、`a - z`、`0 - 9`、` ' . - _ ! # ^ ~`。 有关允许字符的完整列表，请参阅[用户名策略](/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts)。|
|userType|String|可用于对目录中的用户类型进行分类的字符串值，例如`Member``Guest`。          |

由于 **用户** 资源 [支持扩展](/graph/extensibility-overview)`PATCH`，因此可以使用 操作在现有用户实例的扩展的自定义属性中添加、更新或删除你自己的特定于 **应用** 的数据。

> [!NOTE] 
> - 只有应用程序权限的应用无法更新以下属性：**aboutMe**、 **birthday**、 **employeeHireDate**、 **interests**、 **mySite**、 **pastProjects**、 **preferredName**、 **responsibilities**、 **schools**、 and **skills**。
> - 若要更新以下属性，您必须在其自己的 PATCH 请求中指定这些属性，而不包括上表中列出的其他属性： **aboutMe**、 **birthday**、 **interests**、 **mySite**、 **pastProjects**、 **preferredName**、 **responsibilities**、 **schools** 和 **skills**。

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
PATCH https://graph.microsoft.com/beta/me
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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-user-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

以下示例显示了相应的响应。
<!-- {
  "blockType": "response"
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
PATCH https://graph.microsoft.com/beta/users/{id}
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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-other-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-other-user-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

以下示例显示了相应的响应。
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-the-passwordprofile-of-a-user-to-reset-their-password"></a>示例 3：更新用户的 passwordProfile 以重置其密码

以下示例显示重置其他用户密码的请求。 必须为调用用户分配 *Directory.AccessAsUser.All* 委派权限才能更新此属性。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
  "passwordProfile": {
    "forceChangePasswordNextSignIn": false,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-passwordprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-passwordprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-passwordprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-passwordprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-user-passwordprofile-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-user-passwordprofile-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-4-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>示例 4：向用户分配具有字符串值的自定义安全属性

以下示例演示如何向用户分配具有字符串值的自定义安全属性。

+ 属性集：`Engineering`
+ 属性：`ProjectDate`
+ 属性数据类型：字符串
+ 属性值： `"2022-10-01"`

若要分配自定义安全属性，必须为调用主体分配"属性分配管理员"角色，并且必须授予 *CustomSecAttributeAssignment.ReadWrite.All* 权限。

有关用户的更多示例，请参阅使用 Microsoft Graph API 分配、更新[或删除自定义安全属性](/graph/custom-security-attributes-examples)。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/assign-user-customsecurityattribute-string-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-user-customsecurityattribute-string-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/assign-user-customsecurityattribute-string-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/assign-user-customsecurityattribute-string-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
