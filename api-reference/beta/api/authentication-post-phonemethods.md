---
title: 创建 phoneAuthenticationMethod
description: 添加新的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a855289f058454c0e7ff1fb301349f9e49ee12e6
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589228"
---
# <a name="create-phoneauthenticationmethod"></a>创建 phoneAuthenticationMethod

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加新的[电话身份验证方法](../resources/phoneauthenticationmethod.md)。 用户的每种类型只能有一个电话，在**phoneType**属性中捕获。 这意味着， `mobile` 向具有预先存在的手机的用户添加电话将会 `mobile` 失败。 此外，在添加电话之前，用户必须始终具有 `mobile` 电话 `alternateMobile` 。

通过添加电话号码，可以在 Azure 多重身份验证 (MFA) 和自助服务密码重置 (SSPR) （如果已启用）中使用。

此外，如果用户启用了策略以使用 SMS 登录并添加了一个 `mobile` 号码，则系统会尝试注册该号码以在该系统中使用。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 从最高特权到最高特权) 对自己 (的权限 | 对其他人进行操作的权限 (从至少到最高特权) |
|:---------------------------------------|:-------------------------|:-----------------|
| 委派（工作或学校帐户）     | 不支持。 | UserAuthenticationMethod |
| 委派（个人 Microsoft 帐户） | 不支持。 | 不支持。 |
| 应用程序                            | 不支持。 | 不支持。 |

对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id}/authentication/phoneMethods
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)对象的 JSON 表示形式。 JSON 必须包括 `phoneNumber` 和 `phoneType` ，但不 `smsSignInState` 是只读) 的 (。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|phoneNumber|String|将电话号码设为文本或呼叫以进行身份验证。 电话号码使用格式 "+ \<country code\> \<number\> x \<extension\> "，扩展名为可选。 例如，+ 1 5555551234 或 + 1 5555551234x123 是有效的。 如果创建/更新时编号不符合要求的格式，则会拒绝编号。|
|phoneType|String|可能的值为： `mobile` 、 `alternateMobile` 和 `office` 。|

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)对象。

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
