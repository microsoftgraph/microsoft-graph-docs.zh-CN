---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: f9ed7f29b3a6c2afd945383f64b539370047a446
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050687"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD 身份验证方法策略 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

身份验证方法策略定义[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法以及允许使用它们登录并执行 Azure AD) 中的多重身份验证 (Azure Active Directory (用户) 。 可以在 Microsoft 应用中管理的身份验证方法策略Graph FIDO2 安全密钥和无密码电话登录应用Microsoft Authenticator策略。

身份验证方法策略 API 用于管理策略设置。 例如：

* 定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。
* 定义允许用户或用户组使用 FIDO2 安全密钥或无密码电话登录 Azure AD。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法策略       | 说明 |
|:---------------------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| 定义可以在 Azure AD 租户上使用短信的用户。|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制以及可以使用它们登录到 Azure AD 的用户。|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|定义可以在 Azure AD Microsoft Authenticator使用租户的用户。|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|定义可以在 Azure AD 租户上使用电子邮件 OTP 的用户。|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration (](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 弃) |定义可以使用无密码登录电话登录 Azure AD 的用户。|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|定义可以使用临时访问通道登录 Azure AD 的用户。|

## <a name="next-steps"></a>后续步骤

* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。
