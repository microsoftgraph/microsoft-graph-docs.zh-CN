---
title: 更新 identityProvider
description: 更新 identityProvider 的属性。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4056229ecb748ff9c99a3b332298d32e67fdaf66
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921225"
---
# <a name="update-identityprovider"></a>更新 identityProvider
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 Azure AD [中的 socialIdentityProvider](../resources/socialidentityprovider.md) 对象的属性。

对于 Azure AD B2C，更新 [socialIdentityProvider](../resources/socialidentityprovider.md) [、openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider 对象](../resources/appleidentityprovider.md) 的属性。

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
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，为 JSON 对象提供一个或多个属性，这些属性需要针对 Azure AD 租户中的 [socialIdentityProvider](../resources/socialidentityprovider.md) 对象进行更新。

在 Azure AD B2C 中，为 JSON 对象提供一个或多个属性，这些属性需要针对 socialIdentityProvider、openIdConnectIdentityProvider 或[appleIdentityProvider](../resources/appleidentityprovider.md)对象进行更新。 [](../resources/socialidentityprovider.md) [](../resources/openidconnectidentityprovider.md)

### <a name="socialidentityprovider-object"></a>socialIdentityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|向标识提供程序注册应用程序时，获取应用程序的客户端标识符。|
|clientSecret|字符串|向标识提供程序注册时获取的应用程序的客户端密码。 这是只读的。 读取操作返回"\*\*\*\*"。|
|displayName|字符串|标识提供程序的显示名称。|

### <a name="openidconnectidentityprovider-object"></a>openIdConnectIdentityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|向标识提供程序注册应用程序时，获取应用程序的客户端标识符。|
|clientSecret|字符串|使用身份提供程序注册应用时获取的应用客户端密码。 clientSecret 依赖于 **responseType**。 <ul><li>当 **responseType** `code` 为 时，身份验证代码交换需要密码。</li><li>当 **responseType** `id_token` 为密码时不是必需的，因为没有代码交换。 授权id_token返回授权请求。</li></ul>|
|displayName|字符串|标识提供程序的显示名称。|
|domainHint|String|域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。 此复杂类型捕获该映射。|
|metadataUrl|String|OpenID Connect 标识提供程序的元数据文档的 URL。 每个 OpenID Connect 标识提供程序都描述一个元数据文档，该文档包含执行登录所需的大部分信息。 这包括要使用的 URL 以及服务的公共签名密钥的位置等信息。 OpenID Connect 元数据文档始终位于 以 结尾的终结点 `.well-known/openid-configuration` 。 提供您添加的 OpenID Connect 标识提供程序的元数据 URL。|
|responseMode|String|响应模式定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。 可能的值 `form_post` `query` ：、。|
|responseType|String|响应类型描述在初始调用中发送回自定义标识提供程序authorization_endpoint类型。 可能的值 `code` `id_token` `token` ：、、。|
|scope|String|范围定义要从自定义标识提供程序收集的信息和权限。|

### <a name="applemanagedidentityprovider-object"></a>appleManagedIdentityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|displayName|字符串|标识提供程序的显示名称。|
|developerId|String|Apple 开发人员标识符。|
|服务 Id|String|Apple 开发人员标识符。|
|keyId|String|Apple 密钥标识符。|
|certificateData|String|证书中长文本字符串的证书数据可能是 null。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="examples"></a>示例

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a>示例 1：使用 Azure AD 或 Azure AD B2C **(特定** 社会标识) 

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-socialidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-socialidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-socialidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-socialidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a>示例 2：仅为 Azure AD B2C (特定 **OpenID Connect** 标识提供程序) 

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a>示例 3：仅为 **Azure** AD B2C (特定 Apple 标识提供程序) 

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json
Content-length: 41

{
  "displayName": "Apple"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-appleidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-appleidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-appleidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-appleidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
