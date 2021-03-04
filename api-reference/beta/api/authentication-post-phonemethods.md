---
title: 创建 phoneAuthenticationMethod
description: 添加新的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 541feb0aee2f0ea76b92b097b1a2a794111dff2f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438573"
---
# <a name="create-phoneauthenticationmethod"></a>创建 phoneAuthenticationMethod

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加新的电话 [身份验证方法](../resources/phoneauthenticationmethod.md)。 用户可能只有一种类型的电话，在 **phoneType** 属性中捕获。 这意味着，向具有预先不存在的电话的用户添加电话将 `mobile` `mobile` 失败。 此外，在添加电话之前，用户 `mobile` 必须始终拥有 `alternateMobile` 电话。

添加电话号码使其可用于 Azure 多重身份验证 (MFA) 和自助服务密码重置 (SSPR) （如果已启用）。

此外，如果策略允许用户使用短信登录并添加号码，系统将尝试注册号码 `mobile` 以用于该系统。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 自操作权限 (权限从最低到最特权)  | 对他人 (权限从最低到最特权) |
|:---------------------------------------|:-------------------------|:-----------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite | UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 | 不支持。 |
| Application                            | 不适用。 | UserAuthenticationMethod.ReadWrite.All |

对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [phoneAuthenticationMethod 对象的](../resources/phoneauthenticationmethod.md) JSON 表示形式。 JSON 必须包含 `phoneNumber` `phoneType` 和，但不能 `smsSignInState` (只读的) 。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|phoneNumber|String|用于文本或身份验证呼叫的电话号码。 电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机是可选的。 例如，+1 5555551234 或 +1 5555551234x123 有效。 如果数字与所需格式不匹配，则创建/更新时将拒绝这些号码。|
|phoneType|String|可能的值是： `mobile` 和 `alternateMobile` `office` 。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` 新的 [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-phoneauthenticationmethod-from-authentication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "phoneType-value",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
