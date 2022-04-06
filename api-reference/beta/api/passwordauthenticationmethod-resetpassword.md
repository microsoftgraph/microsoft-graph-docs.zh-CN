---
title: passwordAuthenticationMethod：resetPassword
description: 重置用户密码
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3e07320950184a89c9d8000145b75af978a4e1e1
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646583"
---
# <a name="passwordauthenticationmethod-resetpassword"></a>passwordAuthenticationMethod：resetPassword

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为与密码身份验证方法对象关联的 [密码启动重置](../resources/passwordauthenticationmethod.md) 。 这只能由具有适当权限的管理员完成，并且不能对用户自己的帐户执行。

此流将新密码写入Azure Active Directory，如果已使用密码写回本地 Active Directory则推送到新密码。 管理员可以提供新密码或使系统生成一个密码。 系统将提示用户在下次登录时更改其密码。

此重置是一项长时间运行的操作，它将返回一个 **Location** 标头，其中具有一个链接，调用方可以在其中定期检查重置操作的状态。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

> [!IMPORTANT]
> 不能在用户自己的帐户上执行该操作。 只有具有适当权限的管理员才能执行此操作。

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

对于管理员正在操作其他用户的委派方案，管理员需要以下角色Azure AD[之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Content-type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|newPassword|String|新密码。 对于具有混合密码方案的租户，此为必需项。 如果省略仅云密码，系统将返回系统生成的密码。 这是一个没有其他编码的 unicode 字符串。 在验收之前，将针对租户的禁止密码系统验证它，并且必须遵守租户的云和/或本地密码要求。|

## <a name="response"></a>响应

如果成功，此方法返回 响应 `202 Accepted` 代码和 **包含 URL 的位置** 标头，以检查重置操作的状态。

如果调用方未提交密码，则响应正文中的 JSON 对象中会提供 Microsoft 生成的密码。

### <a name="response-headers"></a>响应标头

| 名称        | 说明     |
|:------------|:----------------|
|Location     | 要调用以检查操作状态的 URL。 必需。|
|重试后  | 持续时间（以秒表示）。 可选。|

## <a name="examples"></a>示例

### <a name="example-1-user-submitted-password"></a>示例 1：用户提交的密码

以下示例显示当调用方提交密码时如何调用此 API。

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-type: application/json

{
    "newPassword": "Cuyo5459"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-adminprovided-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/operations/88e7560c-9ebf-435c-8089-c3998ac1ec51?aadgdc=DUB02P&aadgsu=ssprprod-a

{}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-system-generated-password"></a>示例 2：系统生成的密码

以下示例演示当调用方不提交密码时如何调用此 API。

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-systemgenerated-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/operations/77bafe36-3ac0-4f89-96e4-a4a5a48da851?aadgdc=DUB02P&aadgsu=ssprprod-a
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.passwordResetResponse",
    "newPassword": "Cuyo5459"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
