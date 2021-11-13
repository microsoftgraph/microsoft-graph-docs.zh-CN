---
title: 更新 identityProvider
description: 更新 identityProvider 的属性。
ms.localizationpriority: medium
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 246e15f88dae9f30c23de7a4fb384ac602094e02
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890323"
---
# <a name="update-identityprovider"></a>更新 identityProvider
命名空间：microsoft.graph

更新在租户中配置的指定标识提供程序的属性。

在从 identityProviderBase 派生的提供程序类型中，当前可以在 Azure AD 中更新[socialIdentityProvider](../resources/socialidentityprovider.md)资源。 在 Azure AD B2C 中，此操作当前可以更新[socialIdentityProvider](../resources/socialidentityprovider.md)或[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)资源。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityProvider.ReadWrite.All|
|委派（Microsoft 个人帐户）| 不支持。|
|Application| IdentityProvider.ReadWrite.All|

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

在请求正文中，为 JSON 对象提供一个或多个属性，这些属性需要在租户中为[socialIdentityProvider](../resources/socialidentityprovider.md) Azure AD更新。

在 Azure AD B2C 中，为 JSON 对象提供一个或多个属性，这些属性需要针对[socialIdentityProvider](../resources/socialidentityprovider.md)或[appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)对象进行更新。

### <a name="socialidentityprovider-object"></a>socialIdentityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|向标识提供程序注册应用程序时获取的客户端应用程序的标识符。|
|clientSecret|字符串|向标识提供程序注册时获取的应用程序的客户端密码。 这是只读的。 读取操作返回 `****`。|
|displayName|字符串|标识提供程序的显示名称。|

### <a name="applemanagedidentityprovider-object"></a>appleManagedIdentityProvider 对象

|属性|类型|说明|
|:---------------|:--------|:----------|
|displayName|字符串|标识提供程序的显示名称。|
|developerId|String|Apple 开发人员标识符。|
|服务 Id|String|Apple 服务标识符。|
|keyId|String|Apple 密钥标识符。|
|certificateData|String|证书中长文本字符串的证书数据可能是 null。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="examples"></a>示例

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a>示例 1：更新特定 **社会标识提供程序 (Azure AD** 或Azure AD B2C) 

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/identityProviders/Amazon-OAUTH
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.socialIdentityProvider",
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

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a>示例 2：仅为B2C (更新Azure AD Apple 标识) 

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json

{
  "displayName": "Apple"
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
