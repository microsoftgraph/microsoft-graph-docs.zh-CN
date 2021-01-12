---
title: 创建 phoneAuthenticationMethod
description: 添加新的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 41a419425d9d4368aae34a5af0ed3c2b778165d8
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796459"
---
# <a name="create-phoneauthenticationmethod"></a>创建 phoneAuthenticationMethod

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加新的电话 [身份验证方法](../resources/phoneauthenticationmethod.md)。 用户在 **phoneType** 属性中捕获的每种类型只能有一部电话。 这意味着，例如，向具有预先不存在的电话的用户添加电话 `mobile` `mobile` 将失败。 此外，在添加电话之前，用户 `mobile` 必须始终拥有 `alternateMobile` 电话。

通过添加电话号码，可以在 Azure 多重身份验证 (MFA) 和 SSPR (自助服务密码重置（如果启用) ）中使用它。

此外，如果策略允许用户使用短信登录并添加号码，系统将尝试注册号码以用于 `mobile` 该系统。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 对自身执行 (权限从最低特权到最多特权)  | 对他人操作的权限 (权限从最低特权到最多特权) |
|:---------------------------------------|:-------------------------|:-----------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite | UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 | 不支持。 |
| 应用程序                            | 不适用 | UserAuthenticationMethod.ReadWrite.All |

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

在请求正文中，提供 [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象的 JSON 表示形式。 JSON 必须包含 `phoneNumber` 和 `phoneType` ， (只读的 JSON `smsSignInState`) 。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|phoneNumber|String|发短信或呼叫进行身份验证的电话号码。 电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机是可选的。 例如，+1 5555551234 或 +1 5555551234x123 有效。 如果数字与所需格式不匹配，则创建/更新时将拒绝数字。|
|phoneType|String|可能的值是： `mobile` 和 `alternateMobile` `office` 。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和新 `201 Created` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。

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
