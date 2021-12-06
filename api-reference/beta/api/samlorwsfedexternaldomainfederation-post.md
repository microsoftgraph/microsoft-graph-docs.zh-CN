---
title: 创建 samlOrWsFedExternalDomainFederation
description: 创建新的 samlOrWsFedExternalDomainFederation 对象。
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 470df7e15dc702b884e7a524e6fbae76a6fa2532
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002692"
---
# <a name="create-samlorwsfedexternaldomainfederation"></a>创建 samlOrWsFedExternalDomainFederation
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|Domain.Read.All、Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|Domain.Read.All、Domain.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：

* 全局管理员
* 外部标识提供程序管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /directory/federationConfigurations
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象的 JSON 表示形式。

下表显示创建 [samlOrWsFedExternalDomainFederation 时所需的属性](../resources/samlorwsfedexternaldomainfederation.md)。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|基于显示名称 SAML/WS-Fed 的标识提供程序的名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|issuerUri|String|联合服务器的颁发者 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|metadataExchangeUri|String|用于从富客户端应用程序进行身份验证的元数据交换终结点的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|passiveSignInUri|String|登录服务时，基于 Web 的客户端定向到Azure AD URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|preferredAuthenticationProtocol|String|首选身份验证协议。 支持的值包括 `saml` 或 `wsfed` 。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|signingCertificate|String|用于对传递到令牌的令牌进行签名的当前Microsoft 标识平台。 证书的格式设置为联合 IdP 令牌签名证书的公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。  <br/><br/> 此属性用于以下方案： <ul><li> 如果在自动注册更新之外需要滚动 <li>正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后联合身份验证属性中不存在新的令牌签名证书。 </ul> <br/><br/> Azure AD通过自动注册过程更新证书，其中它尝试从联合身份验证服务元数据中检索新证书，即当前证书到期前 30 天。 如果新证书不可用，Azure AD每天监视元数据，并且将在新证书可用时更新域的联盟设置。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_samlorwsfedexternaldomainfederation_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations
Content-Type: application/json

{
    "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
    "issuerUri": "https://contoso.com/issuerUri",
    "displayName": "contoso display name",
    "metadataExchangeUri": "https://contoso.com/metadataExchangeUri",
    "passiveSignInUri": "https://contoso.com/signin",
    "preferredAuthenticationProtocol": "wsFed",
    "domains": [
        {
            "@odata.type": "microsoft.graph.externalDomainName",
            "id": "contoso.com"
        }
    ],
    "signingCertificate": "MIIDADCCAeigAwIBAgIQEX41y8r6"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-samlorwsfedexternaldomainfederation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-samlorwsfedexternaldomainfederation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-samlorwsfedexternaldomainfederation-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-samlorwsfedexternaldomainfederation-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "3c41f317-9af3-4266-8ccf-26283ceec888",
    "displayName": "contoso display name"
}
```
