---
title: 创建 samlOrWsFedExternalDomainFederation
description: 创建新的 samlOrWsFedExternalDomainFederation 对象。
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7ab1a56c83e580ffdabfc687b65e6d5a10a958d5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315723"
---
# <a name="create-samlorwsfedexternaldomainfederation"></a>创建 samlOrWsFedExternalDomainFederation
命名空间：microsoft.graph

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
* 外部标识提供者管理员

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

下表显示了创建 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|基于 SAML/WS-Fed 的标识提供者的显示名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|issuerUri|String|联合服务器的颁发者 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|metadataExchangeUri|String|用于从丰富的客户端应用程序进行身份验证的元数据交换终结点的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|passiveSignInUri|String|登录到 Azure AD 服务时基于 Web 的客户端定向到的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|preferredAuthenticationProtocol|authenticationProtocol|首选身份验证协议。 可能的值为： `wsFed`. `saml` 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|signingCertificate|String|用于对传递给Microsoft 标识平台的令牌进行签名的当前证书。 该证书的格式设置为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。  <br/><br/> 此属性在以下方案中使用： <ul><li> 如果自动滚动更新外部需要滚动更新 <li>正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后，联合身份验证属性中不存在新的令牌签名证书。 </ul> <br/><br/> Azure AD 通过自动滚动更新过程更新证书，在此过程中，Azure AD 会尝试在当前证书过期前 30 天从联合身份验证服务元数据中检索新证书。 如果新证书不可用，Azure AD 将每天监视元数据，并在有新证书可用时更新域的联合身份验证设置。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。

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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-samlorwsfedexternaldomainfederation-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-samlorwsfedexternaldomainfederation-from--powershell-snippets.md)]
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
