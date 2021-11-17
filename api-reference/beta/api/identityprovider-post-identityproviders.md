---
title: 创建 identityProvider
description: 创建新的 identityProvider 对象。
ms.localizationpriority: medium
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 73ccec79e3c68ccc35d8d81261de9f80d2d0411f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978157"
---
# <a name="create-identityprovider-deprecated"></a>创建 identityProvider（已弃用）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

创建新的 [identityProvider](../resources/identityprovider.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityProvider.ReadWrite.All|
|委派（Microsoft 个人帐户）| 不支持。|
|应用程序|IdentityProvider.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：
* 全局管理员
* 外部标识提供程序管理员

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

在请求正文中，仅为 Azure AD B2C 对象提供[identityProvider](../resources/identityprovider.md)或[openIdConnectProvider](../resources/openidconnectprovider.md) (JSON) 表示形式。 下表中列出的所有属性均未必需属性。

### <a name="identityprovider-object"></a>identityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|应用程序的客户端 ID。这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|应用程序的客户端密码。这是向标识提供程序注册应用程序时获取的客户端密码。|
|name|字符串|标识提供程序的显示名称。|
|type|字符串|标识提供程序类型。 <ul>对于 B2B 方案：<li/>Google<li/>Facebook</ul><ul>对于 B2C 方案：<li/>Microsoft<li/>Google<li/>Amazon<li/>领英<li/>Facebook<li/>GitHub<li/>Twitter<li/>微博<li/>QQ<li/>微信<li/>OpenIDConnect</ul>|

### <a name="openidconnectprovider-object"></a>openIdConnectProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|应用程序的客户端 ID。这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|应用程序的客户端密码。这是向标识提供程序注册应用程序时获取的客户端密码。|
|name|字符串|标识提供程序的显示名称。|
|type|字符串|标识提供程序类型。 值必须为 `OpenIdConnect` 。|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|和 `userId` `displayname` 属性在 claimsMapping 对象中是必需的。|
|metadataUrl|String|开放 ID 和标识提供程序的元数据连接 URL。|
|responseMode|String|定义用于将数据从自定义标识提供程序发送回 B2C Azure AD的方法。 可以使用以下响应模式： <ul><li/>`form_post` ：建议采用此响应模式，以获得最佳安全性。 响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。<li/>`query` ：代码或令牌作为查询参数返回。</ul>|
|responseType|String|描述在初始调用自定义标识提供程序的 authorization_endpoint发送回的信息类型。 可以使用以下响应类型：<ul><li/> `code`：根据授权代码流，代码将返回到 Azure AD B2C。 Azure AD B2C 继续调用 token_endpoint 以交换令牌代码。<li/> `id_token`：ID 令牌从自定义标识Azure AD返回给 B2C。 <li/>`token`：访问令牌从自定义标识提供程序Azure AD返回给 B2C。  (当前 B2C 不支持Azure AD此值) </ul>|
|scope|String|范围定义要从自定义标识提供程序收集的信息和权限。|

## <a name="response"></a>响应

如果成功，此方法仅对响应正文中的 Azure AD B2C) 对象返回 响应代码和 `201 Created` [identityProvider](../resources/identityprovider.md)或[openIdConnectProvider](../resources/openidconnectprovider.md) (。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="examples"></a>示例

### <a name="example-1-create-a-specific-identityprovider"></a>示例 1：创建特定 **identityProvider**

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.identityProvider",
  "name": "Login with Amazon",
  "type": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-identityprovider-from-identityproviders-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.type": "microsoft.graph.identityProvider",
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a>示例 2：仅为 B2C (创建Azure AD **openIDConnectProvider**) 

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_openidconnectprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
    "name": "Login with the Contoso identity provider",
    "type": "OpenIDConnect",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "claimsMapping": {
        "userId": "myUserId",
        "givenName": "myGivenName",
        "surname": "mySurname",
        "email": "myEmail",
        "displayName": "myDisplayName"
    },
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid"
}

```

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-openidconnectprovider-from-identityproviders-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```
