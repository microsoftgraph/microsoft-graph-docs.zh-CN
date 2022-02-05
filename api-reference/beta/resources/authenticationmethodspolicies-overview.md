---
title: Azure AD身份验证方法策略 API 概述
description: 身份验证方法策略定义哪些身份验证方法可用于 Azure AD。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
---

# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD身份验证方法策略 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

身份验证方法策略定义[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法以及允许使用这些方法登录和在 Azure Active Directory (Azure AD) 中的 MFA (执行多重) 身份验证。 可以在 Microsoft 应用商店中管理的身份验证方法策略Graph FIDO2 安全密钥和无密码电话登录时Microsoft Authenticator应用。

身份验证方法策略 API 用于管理策略设置。 例如：

* 定义可在租户租户中使用的 FIDO2 Azure AD类型。
* 定义允许用户或用户组使用 FIDO2 安全密钥或无密码电话登录以登录Azure AD。
* 定义应提醒其使用推送通知为 MFA Microsoft Authenticator用户或用户组。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法策略       | Description |
|:---------------------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| 定义可以在租户上使用短信Azure AD用户。|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制以及可以使用它们登录安全密钥Azure AD。|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|定义可以在租户Microsoft Authenticator使用Azure AD的用户。|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|定义可以在租户上使用电子邮件 OTP Azure AD用户。|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration (](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 弃) |定义可以使用无密码登录电话登录的用户Azure AD。|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|定义可以使用临时访问通道登录用户Azure AD。|
|[x509CertificateAuthenticationMethodConfiguration](x509CertificateAuthenticationMethodConfiguration.md)|定义可以使用 X.509 证书登录到 Azure AD。|

## <a name="policies-available-to-push-users-to-set-up-authentication-methods"></a>可用于推送用户设置身份验证方法的策略：
|Policy       | Description |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| 定义应提醒其设置身份验证方法的用户 (仅支持Microsoft Authenticator) 。|

## <a name="next-steps"></a>后续步骤

* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。
