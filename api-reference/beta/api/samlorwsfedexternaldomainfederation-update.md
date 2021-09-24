---
title: 更新 samlOrWsFedExternalDomainFederation
description: 更新 samlOrWsFedExternalDomainFederation 对象的属性。
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b5997fc1a2f3d4f47d03b2c37df8c87a09419477
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508638"
---
# <a name="update-samlorwsfedexternaldomainfederation"></a>更新 samlOrWsFedExternalDomainFederation
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [samlOrWsFedExternalDomainFederation 对象](../resources/samlorwsfedexternaldomainfederation.md) 的属性。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|Domain.ReadWrite.All|

工作或学校帐户需要属于以下 Azure [AD Azure Active Directory (角色) 之一](/azure/active-directory/roles/permissions-reference)：

* 全局管理员
* 外部标识提供程序管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/{samlOrWsFedExternalDomainFederation ID}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，为 JSON 对象提供一个或多个属性，这些属性需要针对 Azure AD 租户中的 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象进行更新。

下表显示了您可以为 [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象更新的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|基于显示名称 SAML/WS-Fed 的标识提供程序的名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|issuerUri|String|联合服务器的颁发者 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|metadataExchangeUri|String|用于从富客户端应用程序进行身份验证的元数据交换终结点的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|passiveSignInUri|String|登录 Azure AD 服务时基于 Web 的客户端定向到的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|preferredAuthenticationProtocol|String|首选身份验证协议。 支持的值包括 `saml` 或 `wsfed` 。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|signingCertificate|String|用于对传递到证书的令牌进行签名的当前Microsoft 标识平台。 证书的格式设置为联合 IdP 令牌签名证书的公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。  <br/><br/> 此属性用于以下方案： <ul><li> 如果在自动注册更新之外需要滚动 <li>正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后，联合身份验证属性中不存在新的令牌签名证书。 </ul> <br/><br/> Azure AD 通过自动注册过程更新证书，其中它尝试从联合身份验证服务元数据检索新证书，即当前证书到期前 30 天。 如果新证书不可用，Azure AD 将每天监视元数据，并且将在新证书可用时更新域的联盟设置。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [samlOrWsFedExternalDomainFederation](../resources/samlorwsfedexternaldomainfederation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_samlorwsfedexternaldomainfederation"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/d5a56845-6845-d5a5-4568-a5d54568a5d5
Content-Type: application/json

{
  "displayName": "Contoso name change",
  "issuerUri": "http://contoso-test.com/adfs/services/trust",
  "metadataExchangeUri": null,
  "signingCertificate": "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
  "passiveSignInUri": "https://contoso-test.com/adfs/ls/",
  "preferredAuthenticationProtocol": "wsFed"
}


```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-samlorwsfedexternaldomainfederation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-samlorwsfedexternaldomainfederation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-samlorwsfedexternaldomainfederation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-samlorwsfedexternaldomainfederation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "id": "d5a56845-6845-d5a5-4568-a5d54568a5d5",
  "displayName": "Contoso name change",
  "issuerUri": "http://contoso-test.com/adfs/services/trust",
  "metadataExchangeUri": null,
  "signingCertificate": "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
  "passiveSignInUri": "https://contoso-test.com/adfs/ls/",
  "preferredAuthenticationProtocol": "wsFed",
  "domains": [
      {
          "id": "contoso.com"
      }
  ]
}
```
