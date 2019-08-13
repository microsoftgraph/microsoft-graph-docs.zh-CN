---
title: 创建用户
description: 新建用户。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6eb65544ed26e0b08802fbc84ce8dbcabf0a8ed1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362055"
---
# <a name="create-user"></a>创建用户

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新[用户](../resources/user.md)。
请求正文包含要创建的用户。 至少必须指定必需的用户属性。 可以选择指定其他任意可写属性。

>[!NOTE]
>若要创建外部用户, 请使用[邀请 API](invitation-post.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。

下表显示创建用户时所需的属性。

| 参数 | 类型 | 说明|
|:---------------|:--------|:----------|
|accountEnabled |Boolean |启用此帐户时为 true，否则为 false。|
|displayName |string |要在用户的通讯簿中显示的名称。|
|onPremisesImmutableId |string |如果你对用户的 userPrincipalName (UPN) 属性使用联盟域，只需在创建新用户帐户时指定。|
|mailNickname |string |用户的邮件别名。|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md) |用户的密码配置文件。|
|userPrincipalName |string |用户主体名称 (someuser@contoso.com)。|

由于**用户**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用`POST`操作, 并在创建用户实例时将自己的数据添加到用户实例中的自定义属性。

>[!NOTE]
>默认情况下, 使用此 API 创建的联合用户将被强制每隔12小时登录一次。 有关如何更改此操作的详细信息, 请参阅[令牌生存期异常](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes#exceptions)。

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/user.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-user-from-users-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-user-from-users-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-user-from-users-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-user-from-users-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

在请求正文中，提供 [user](../resources/user.md) 对象的 JSON 表示形式。
##### <a name="response"></a>响应
下面是一个响应示例。 

[!NOTE]
为了提高可读性, 可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
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
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
