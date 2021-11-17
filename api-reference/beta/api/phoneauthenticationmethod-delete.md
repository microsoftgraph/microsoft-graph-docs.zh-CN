---
title: 删除 phoneAuthenticationMethod
description: 删除用户的电话身份验证方法。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f8e70fb8d04ce33561f4a23bd7c36b9de7c265c6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024771"
---
# <a name="delete-phoneauthenticationmethod"></a>删除 phoneAuthenticationMethod

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除用户的电话 [身份验证方法](../resources/phoneauthenticationmethod.md)。 

>**注意：** 这将删除用户的电话号码，他们将不再能够使用该号码进行身份验证，无论是通过短信还是语音呼叫。

请记住，用户不能有 `alternateMobile` 没有数字 `mobile` 的号码。 如果要从也具有号码的用户中删除号码，请首先将号码更新为新号码，然后 `mobile` `alternateMobile` [](phoneauthenticationmethod-update.md) `mobile` 删除该 `alternateMobile` 号码。

如果电话号码是用户的默认 Azure 多重身份验证 (MFA) 身份验证方法，则不能将其删除。 让用户更改其默认身份验证方法，然后删除该号码。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-acting-on-self"></a>自行操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

### <a name="permissions-acting-on-other-users"></a>对其他用户操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | UserAuthenticationMethod.ReadWrite.All |

对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：
* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
与要 `id` 删除的 phoneType 对应的值是下列值之一：
+ `b6332ec1-7057-4abe-9331-3d72feddfe41` 删除 `alternateMobile` **phoneType**。
+ `e37fc753-ff3b-4958-9484-eaa9425c82bc` 删除 `office` **phoneType**。
+ `3179e48a-750b-4051-897c-87b9720928f7` 删除 `mobile` **phoneType**。

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-phoneauthenticationmethod-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
