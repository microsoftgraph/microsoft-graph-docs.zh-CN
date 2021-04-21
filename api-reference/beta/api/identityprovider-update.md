---
title: 更新 identityProvider
description: 更新 identityProvider 的属性。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: eb441c036fd4d555a7991c30a986258300282c35
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921565"
---
# <a name="update-identityprovider-deprecated"></a>更新 identityProvider (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

更新 [identityProvider 对象](../resources/identityprovider.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityProvider.ReadWrite.All|
|委派（Microsoft 个人帐户）| 不支持。|
|应用程序| IdentityProvider.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：

* 全局管理员
* 外部标识提供程序管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，为 JSON 对象提供一个或多个属性，这些属性需要针对仅针对 Azure AD B2C ([identityProvider](../resources/identityprovider.md) 或 [openIdConnectProvider](../resources/openidconnectprovider.md)) 更新。

### <a name="identityprovider-object"></a>identityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|应用程序的客户端 ID。 这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|应用程序的客户端密码。 这是向标识提供程序注册应用程序时获取的客户端密码。|
|name|字符串|标识提供程序的显示名称。|
|type|字符串|标识提供程序类型。<ul>对于 B2B 方案：<li/>Google<li/>Facebook</ul><ul>对于 B2C 方案：<li/>Microsoft<li/>Google<li/>Amazon<li/>领英<li/>Facebook<li/>GitHub<li/>Twitter<li/>微博<li/>QQ<li/>微信<li/>OpenIDConnect</ul>|

### <a name="openidconnectprovider-object"></a>openIdConnectProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|应用程序的客户端 ID。 这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|应用程序的客户端密码。 这是向标识提供程序注册应用程序时获取的客户端密码。|
|name|字符串|标识提供程序的显示名称。|
|type|字符串|标识提供程序类型。 值必须为 `OpenIdConnect` 。|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。 此复杂类型捕获该映射。|
|domainHint|String|域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。|
|metadataUrl|String|Open Id Connect 标识提供程序的元数据文档的 URL。|
|responseMode|String|定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。 可以使用以下响应模式： <ul><li/>`form_post` ：建议采用此响应模式，以获得最佳安全性。 响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。<li/>`query` ：代码或令牌作为查询参数返回。</ul>|
|responseType|String|描述在初始调用自定义标识提供程序的 authorization_endpoint发送回的信息类型。 可以使用以下响应类型：<ul><li/> `code` ：根据授权代码流，代码将返回到 Azure AD B2C。 Azure AD B2C 继续调用 token_endpoint 以交换令牌代码。<li/> `id_token` ：ID 令牌从自定义标识提供程序返回回 Azure AD B2C。 <li/>`token` ：访问令牌从自定义标识提供程序返回回 Azure AD B2C。  (当前 Azure AD B2C 不支持) </ul>|
|scope|String|范围定义要从自定义标识提供程序收集的信息和权限。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="examples"></a>示例

### <a name="example-1-update-a-specific-identityprovider"></a>示例 1：更新特定 **identityProvider**

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a>示例 2：仅为 Azure AD B2C (更新特定的 **openIDConnectProvider**) 

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
