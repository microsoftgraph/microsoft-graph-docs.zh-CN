---
title: 更新 phoneAuthenticationMethod
description: 更新与 phoneAuthenticationMethod 对象关联的电话号码。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6be00410dfc32e13faf7d686c93fbeb3bd160096
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805838"
---
# <a name="update-phoneauthenticationmethod"></a>更新 phoneAuthenticationMethod

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新与[电话身份验证方法](../resources/phoneauthenticationmethod.md)关联的电话号码。

无法更改电话类型。 若要更改电话类型，请添加所需类型的新号码，然后使用原始类型删除该对象。

如果用户通过策略启用，以使用 SMS 登录，并且更改了`mobile`号码，则系统将尝试注册该号码以在该系统中使用。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 作用于自助的权限（从最高特权到最高特权） | 对其他用户的权限（从最低到最高特权）|
|:---------------------------------------|:-------------------------|:-----------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod，UserAuthenticationMethod。 | UserAuthenticationMethod |
| 委派（个人 Microsoft 帐户） | 不支持。 | 不支持。 |
| 应用程序                            | 不支持。 | 不支持。 |

对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |
| Content-type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 将根据其他属性值的更改重新计算未包含在请求正文中的现有属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|phoneNumber|String|将电话号码设为文本或呼叫以进行身份验证。 \<电话号码使用 "+ 国家/地区代码\> \<号码\>x\<分机\>" 格式，扩展名为可选。 例如，+ 1 5555551234 或 + 1 5555551234x123 是有效的。 如果创建/更新时编号不符合要求的格式，则会拒绝编号。|
|phoneType|string| 可能的值包括`mobile`： `alternateMobile`、或`office`。|

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
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
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
