---
title: 更新 internalDomainFederation
description: 更新 internalDomainFederation 对象的属性。
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 47df12b2dc19e56890b026662b02505f42c9ae97
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556276"
---
# <a name="update-internaldomainfederation"></a>更新 internalDomainFederation
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [internalDomainFederation](../resources/internaldomainfederation.md) 对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|Domain.ReadWrite.All|

必须为调用用户或应用分配全局管理员 [Azure AD 角色](/azure/active-directory/roles/permissions-reference)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /domains/{domainsId}/federationConfiguration/{internalDomainFederationId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|activeSignInUri|String|使用 Azure Active Directory (Azure AD) 中为单一登录设置的联合域进行身份验证时，活动客户端使用的终结点 URL。 对应于 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **ActiveLogOnUri** 属性。|
|displayName|String|联合标识提供者 (IdP) 的显示名称。 |
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|确定当联合用户访问受需要 MFA 的条件访问策略管理的应用程序时，Azure AD 是否接受联合 IdP 执行的 MFA。 可能的值包括 `acceptIfMfaDoneByFederatedIdp`、`enforceMfaByFederatedIdp`、`rejectMfaByFederatedIdp`、`unknownFutureValue`。 有关详细信息，请参阅 [federatedIdpMfaBehavior 值](#federatedidpmfabehavior-values)。|
|isSignedAuthenticationRequestRequired|布尔|如果 `true`将 SAML 身份验证请求发送到联合 SAML IdP 时，Azure AD 将使用 OrgID 签名密钥对这些请求进行签名。 如果 `false` (默认) ，则发送到联合 IdP 的 SAML 身份验证请求不会签名。|
|issuerUri|String|联合服务器的颁发者 URI。|
|metadataExchangeUri|String|用于从丰富的客户端应用程序进行身份验证的元数据交换终结点的 URI。|
|nextSigningCertificate|String|回退令牌签名证书，该证书用于在主签名证书过期时对令牌进行签名。 格式化为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串。 需要与 X509Certificate2 类兼容。 与 **signingCertificate** 非常类似，如果需要在自动滚动更新之外进行滚动更新、正在设置新的联合身份验证服务，或者在联合身份验证服务证书更新后联合身份验证属性中不存在新的令牌签名证书，则使用 **nextSigningCertificate** 属性。|
|passiveSignInUri|String|登录到 Azure AD 服务时基于 Web 的客户端定向到的 URI。 |
|preferredAuthenticationProtocol|authenticationProtocol|首选身份验证协议。 可能的值包括 `wsFed`、`saml`、`unknownFutureValue`。 |
|promptLoginBehavior|promptLoginBehavior|设置登录提示的首选行为。 可能的值包括 `translateToFreshPasswordAuthentication`、`nativeSupport`、`disabled`、`unknownFutureValue`。|
|signingCertificate|String|用于对传递给Microsoft 标识平台的令牌进行签名的当前证书。 该证书的格式设置为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。 <br>此属性在以下方案中使用： <li> 如果需要在自动滚动更新之外进行滚动更新 <li> 正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后，联合身份验证属性中不存在新的令牌签名证书。<br>Azure AD 通过自动滚动更新过程更新证书，在此过程中，Azure AD 会尝试在当前证书过期前 30 天从联合身份验证服务元数据中检索新证书。 如果新证书不可用，Azure AD 将每天监视元数据，并在有新证书可用时更新域的联合身份验证设置。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|提供签名证书上次更新的状态和时间戳。|
|signOutUri|String|客户端注销 Azure AD 服务时重定向到的 URI。 对应于 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **LogOffUri** 属性。|

### <a name="federatedidpmfabehavior-values"></a>federatedIdpMfaBehavior 值

| 成员 | 说明 |
| :--- | :--- |
| acceptIfMfaDoneByFederatedIdp | Azure AD 接受联合标识提供者执行的 MFA。 如果联合标识提供者未执行 MFA，Azure AD 将执行 MFA。 |
| enforceMfaByFederatedIdp | Azure AD 接受联合标识提供者执行的 MFA。 如果联合标识提供者未执行 MFA，它将请求重定向到联合标识提供者以执行 MFA。 |
| rejectMfaByFederatedIdp | Azure AD 始终执行 MFA 并拒绝联合标识提供者执行的 MFA。 |

**注意：****federatedIdpMfaBehavior** 是 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **SupportsMfa** 属性的进化版本。 
+ 不支持在 **federatedIdpMfaBehavior** 和 **SupportsMfa** 之间切换。
+ 设置 **federatedIdpMfaBehavior** 属性后，Azure AD 将忽略 **SupportsMfa** 设置。
+ 如果从未设置 **FederatedIdpMfaBehavior** 属性，Azure AD 将继续遵循 **SupportsMfa** 设置。
+ 如果既未设置 **federatedIdpMfaBehavior** ，也不设置 **SupportsMfa** ，则 Azure AD 将默认为 `acceptIfMfaDoneByFederatedIdp` 行为。



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [internalDomainFederation](../resources/internaldomainfederation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_internaldomainfederation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc
Content-Type: application/json

{
  "displayName": "Contoso name change",  
  "federatedIdpMfaBehavior": "acceptIfMfaDoneByFederatedIdp"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-internaldomainfederation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-internaldomainfederation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-internaldomainfederation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-internaldomainfederation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-internaldomainfederation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-internaldomainfederation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.internalDomainFederation"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
   "displayName": "Contoso name change",
   "issuerUri": "http://contoso.com/adfs/services/trust",
   "metadataExchangeUri": "https://sts.contoso.com/adfs/services/trust/mex",
   "signingCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
   "passiveSignInUri": "https://sts.contoso.com/adfs/ls",
   "preferredAuthenticationProtocol": "wsFed",
   "activeSignInUri": "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
   "signOutUri": "https://sts.contoso.com/adfs/ls",
   "promptLoginBehavior": "nativeSupport",
   "isSignedAuthenticationRequestRequired": true,
   "nextSigningCertificate": "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
   "signingCertificateUpdateStatus": {
        "certificateUpdateResult": "Success",
        "lastRunDateTime": "2021-08-25T07:44:46.2616778Z"
    },
   "federatedIdpMfaBehavior": "acceptIfMfaDoneByFederatedIdp"
}
```

