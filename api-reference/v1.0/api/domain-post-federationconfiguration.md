---
title: 创建 federationConfiguration
description: 创建新的 internalDomainFederation 对象。
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 94a74aa85d38895a19b85eabf9a2068bdb239117
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447421"
---
# <a name="create-federationconfiguration"></a>创建 federationConfiguration
命名空间：microsoft.graph

创建新的 [internalDomainFederation](../resources/internaldomainfederation.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Domain.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|Application|Domain.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /domains/{domainsId}/federationConfiguration
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [internalDomainFederation](../resources/internaldomainfederation.md) 对象的 JSON 表示形式。

创建 **internalDomainFederation** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|联合标识提供者的显示名称。|
|issuerUri|String|联合服务器的颁发者 URI。|
|metadataExchangeUri|String|用于从丰富的客户端应用程序进行身份验证的元数据交换终结点的 URI。|
|signingCertificate|String|用于对传递给Microsoft 标识平台的令牌进行签名的当前证书。 该证书的格式设置为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串，并且必须与 X509Certificate2 类兼容。 <br>此属性在以下方案中使用： <li> 如果需要在自动滚动更新之外进行滚动更新 <li> 正在设置新的联合身份验证服务 <li> 如果更新联合身份验证服务证书后，联合身份验证属性中不存在新的令牌签名证书。<br>Azure AD 通过自动滚动更新过程更新证书，在此过程中，Azure AD 会尝试在当前证书过期前 30 天从联合身份验证服务元数据中检索新证书。 如果新证书不可用，Azure AD 将每天监视元数据，并在有新证书可用时更新域的联合身份验证设置。|
|passiveSignInUri|String|登录到 Azure AD 服务时基于 Web 的客户端定向到的 URI。|
|preferredAuthenticationProtocol|authenticationProtocol|首选身份验证协议。 可能的值包括 `wsFed`、`saml`、`unknownFutureValue`。|
|activeSignInUri|String|使用 Azure Active Directory (Azure AD) 中为单一登录设置的联合域进行身份验证时，活动客户端使用的终结点 URL。 对应于 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **ActiveLogOnUri** 属性。|
|signOutUri|String|客户端注销 Azure AD 服务时重定向到的 URI。 对应于 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **LogOffUri** 属性。|
|promptLoginBehavior|promptLoginBehavior|设置登录提示的首选行为。 可能的值包括 `translateToFreshPasswordAuthentication`、`nativeSupport`、`disabled`、`unknownFutureValue`。|
|isSignedAuthenticationRequestRequired|Boolean|如果为 true，则当 SAML 身份验证请求发送到联合 SAML IDP 时，Azure AD 将使用 OrgID 签名密钥对这些请求进行签名。 如果为 false (默认) ，则发送到联合 IDP 的 SAML 身份验证请求不会签名。|
|nextSigningCertificate|String|回退令牌签名证书，该证书用于在主签名证书过期时对令牌进行签名。 格式化为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串。 需要与 X509Certificate2 类兼容。 与 **signingCertificate** 非常类似，如果需要在自动滚动更新之外进行滚动更新、正在设置新的联合身份验证服务，或者在联合身份验证服务证书更新后联合身份验证属性中不存在新的令牌签名证书，则使用 **nextSigningCertificate** 属性。|
|signingCertificateUpdateStatus|[signingCertificateUpdateStatus](../resources/signingcertificateupdatestatus.md)|提供签名证书上次更新的状态和时间戳。|
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|确定当联合用户访问受需要 MFA 的条件访问策略管理的应用程序时，Azure AD 是否接受联合 IdP 执行的 MFA。 可能的值包括 `acceptIfMfaDoneByFederatedIdp`、`enforceMfaByFederatedIdp`、`rejectMfaByFederatedIdp`、`unknownFutureValue`。 有关详细信息，请参阅 [federatedIdpMfaBehavior 值](#federatedidpmfabehavior-values)。|

### <a name="federatedidpmfabehavior-values"></a>federatedIdpMfaBehavior 值

| 成员 | 说明 |
| :--- | :--- |
| acceptIfMfaDoneByFederatedIdp | Azure AD 接受联合标识提供者执行的 MFA。 如果联合标识提供者未执行 MFA，Azure AD 将执行 MFA。 |
| enforceMfaByFederatedIdp | Azure AD 接受联合标识提供者执行的 MFA。 如果联合标识提供者未执行 MFA，它将请求重定向到联合标识提供者以执行 MFA。 |
| rejectMfaByFederatedIdp | Azure AD 始终执行 MFA 并拒绝联合标识提供者执行的 MFA。 |

>[!NOTE]
>**federatedIdpMfaBehavior** 是 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **SupportsMfa** 属性的进化版本。 
>+ 不支持在 **federatedIdpMfaBehavior** 和 **SupportsMfa** 之间切换。
>+ 设置 **federatedIdpMfaBehavior** 属性时，Azure AD 会忽略 **SupportsMfa** 设置。
>+ 如果从未设置 **FederatedIdpMfaBehavior** 属性，Azure AD 将继续遵循 **SupportsMfa** 设置。
>+ 如果既未设置 **federatedIdpMfaBehavior** ，也不设置 **SupportsMfa** ，则 Azure AD 将默认为 `acceptIfMfaDoneByFederatedIdp` 行为。


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [internalDomainFederation](../resources/internaldomainfederation.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_internaldomainfederation_from_"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/domains/contoso.com/federationConfiguration
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "displayName": "Contoso",
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
  "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.internalDomainFederation"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "6601d14b-d113-8f64-fda2-9b5ddda18ecc",
   "displayName": "Contoso",
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
   "federatedIdpMfaBehavior": "rejectMfaByFederatedIdp"
}
```

