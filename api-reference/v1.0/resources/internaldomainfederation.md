---
title: internalDomainFederation 资源类型
description: 表示与 Azure AD 联合的租户中域的配置。
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: eb5788ebd83810834d19fe9500f13f11df9f6554
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447399"
---
# <a name="internaldomainfederation-resource-type"></a>internalDomainFederation 资源类型

命名空间：microsoft.graph

表示与 Azure AD 联合的租户域的配置。 使用此资源在设置与 Azure AD 的联合身份验证时配置联合身份验证设置。 有关联合身份验证的信息，[请参阅什么是与 Azure AD 的联合？](/azure/active-directory/hybrid/whatis-fed)


继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 federationConfiguration](../api/domain-post-federationconfiguration.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|创建新的 [internalDomainFederation](../resources/internaldomainfederation.md) 对象。|
|[获取 internalDomainFederation](../api/internaldomainfederation-get.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|读取 [internalDomainFederation](../resources/internaldomainfederation.md) 对象的属性和关系。|
|[更新 internalDomainFederation](../api/internaldomainfederation-update.md)|[internalDomainFederation](../resources/internaldomainfederation.md)|更新 [internalDomainFederation](../resources/internaldomainfederation.md) 对象的属性。|
|[删除 internalDomainFederation](../api/internaldomainfederation-delete.md)|无|删除 [internalDomainFederation](../resources/internaldomainfederation.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|activeSignInUri|String|使用 Azure Active Directory (Azure AD) 中为单一登录设置的联合域进行身份验证时，活动客户端使用的终结点 URL。 对应于 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **ActiveLogOnUri** 属性。|
|displayName|String|联合标识提供者 (IdP) 的显示名称。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|federatedIdpMfaBehavior|federatedIdpMfaBehavior|确定当联合用户访问受需要 MFA 的条件访问策略管理的应用程序时，Azure AD 是否接受联合 IdP 执行的 MFA。 可能的值包括 `acceptIfMfaDoneByFederatedIdp`、`enforceMfaByFederatedIdp`、`rejectMfaByFederatedIdp`、`unknownFutureValue`。 有关详细信息，请参阅 [federatedIdpMfaBehavior 值](#federatedidpmfabehavior-values)。|
|id|String|联合标识提供者的标识符。 继承自 [entity](../resources/entity.md)。|
|isSignedAuthenticationRequestRequired|Boolean|如果 `true`将 SAML 身份验证请求发送到联合 SAML IdP 时，Azure AD 将使用 OrgID 签名密钥对这些请求进行签名。 如果 `false` (默认) ，则发送到联合 IdP 的 SAML 身份验证请求不会签名。|
|issuerUri|String|联合服务器的颁发者 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|metadataExchangeUri|String|用于从丰富的客户端应用程序进行身份验证的元数据交换终结点的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|nextSigningCertificate|String|回退令牌签名证书，该证书用于在主签名证书过期时对令牌进行签名。 格式化为联合 IdP 令牌签名证书公共部分的 Base64 编码字符串。 需要与 X509Certificate2 类兼容。 与 signingCertificate 非常类似，如果需要在自动滚动更新之外进行滚动更新、正在设置新的联合身份验证服务，或者在联合身份验证服务证书更新后联合身份验证属性中不存在新的令牌签名证书，则使用 nextSigningCertificate 属性。|
|passiveSignInUri|String|登录到 Azure AD 服务时基于 Web 的客户端定向到的 URI。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
|preferredAuthenticationProtocol|authenticationProtocol|首选身份验证协议。 可能的值包括 `wsFed`、`saml`、`unknownFutureValue`。 继承自 [samlOrWsFedProvider](../resources/samlorwsfedprovider.md)。|
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

>[!NOTE]
>**federatedIdpMfaBehavior** 是 [Set-MsolDomainFederationSettings MSOnline v1 PowerShell cmdlet](/powershell/module/msonline/set-msoldomainfederationsettings) 的 **SupportsMfa** 属性的进化版本。 
>+ 不支持在 **federatedIdpMfaBehavior** 和 **SupportsMfa** 之间切换。
>+ 设置 **federatedIdpMfaBehavior** 属性时，Azure AD 会忽略 **SupportsMfa** 设置。
>+ 如果从未设置 **FederatedIdpMfaBehavior** 属性，Azure AD 将继续遵循 **SupportsMfa** 设置。
>+ 如果既未设置 **federatedIdpMfaBehavior** ，也不设置 **SupportsMfa** ，则 Azure AD 将默认为 `acceptIfMfaDoneByFederatedIdp` 行为。

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.internalDomainFederation",
  "baseType": "microsoft.graph.samlOrWsFedProvider",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.internalDomainFederation",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String",
  "activeSignInUri": "String",
  "signOutUri": "String",
  "promptLoginBehavior": "String",
  "isSignedAuthenticationRequestRequired": "Boolean",
  "nextSigningCertificate": "String",
  "signingCertificateUpdateStatus": {
    "certificateUpdateResult": "String",
    "@odata.type": "microsoft.graph.signingCertificateUpdateStatus"
  },
  "federatedIdpMfaBehavior": "String"
}
```

