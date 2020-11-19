---
title: 创建 emailAuthenticationMethod
description: 创建新的 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e66a0254240c852ab364a97d5d246f2714687afe
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352153"
---
# <a name="create-emailauthenticationmethod"></a>创建 emailAuthenticationMethod
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置用户的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。 电子邮件身份验证是一种自助密码重置方法。 一个用户可能只有一种电子邮件身份验证方法。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|从最高特权到最少特权) 对自己 (的权限|对其他人进行操作的权限 (从至少到最高特权) |
|:---|:---|:--|
|委派（工作或学校帐户）|不支持。|UserAuthenticationMethod
|委派（个人 Microsoft 帐户）|不支持。|不支持。
|应用程序|不支持。|不支持。

对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：

* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有所需电子邮件地址的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象的 JSON 表示形式。

下表显示创建 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md)时所需的属性。

|属性|类型|Description|
|:---|:---|:---|
|emailAddress|String|电子邮件地址|



## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
