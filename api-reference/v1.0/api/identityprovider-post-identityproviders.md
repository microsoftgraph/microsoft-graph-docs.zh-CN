---
title: 创建 identityProvider
description: 新建 identityProvider
ms.localizationpriority: high
author: namkedia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5442e2a05d87e22f7c6f545ff68c78dbb1f4158f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080028"
---
# <a name="create-identityprovider-deprecated"></a>创建 identityProvider（已弃用）
命名空间：microsoft.graph

[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

通过指定显示名称、identityProvider 类型、客户端 ID 和客户端密码，创建新的 [identityProvider](../resources/identityprovider.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityProvider.ReadWrite.All|
|委派（Microsoft 个人帐户）| 不支持。|
|应用程序|不支持。|

工作或学校帐户必须是租户的全局管理员。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [identityProvider](../resources/identityprovider.md) 对象的 JSON 表示形式。 下表中列出的所有属性均未必需属性。

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|应用程序的客户端 ID。这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|应用程序的客户端密码。这是向标识提供程序注册应用程序时获取的客户端密码。|
|name|字符串|标识提供程序的显示名称。|
|type|String|标识提供程序类型。它必须是 B2C 方案的下列值之一： <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>领英<li/>Facebook<li/>GitHub<li/>Twitter<li/>微博<li/>QQ<li/>微信</ul>在 B2B 中，它只能是 Google|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [identityProvider](../resources/identityprovider.md) 对象。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例

以下示例会创建 **identityProvider**。

##### <a name="request"></a>请求

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a>响应

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
