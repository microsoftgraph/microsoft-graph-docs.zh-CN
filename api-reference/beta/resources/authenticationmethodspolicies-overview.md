---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 35d3beecb26a5ae4455502ed0535c959cf7f502e
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682129"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD 身份验证方法策略 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

身份验证方法策略定义[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法以及允许使用它们登录并执行 Azure AD) 中的多重身份验证 (Azure Active Directory (用户) 。 可以在 Microsoft 应用中管理的身份验证方法策略Graph FIDO2 安全密钥和无密码电话登录应用Microsoft Authenticator策略。

身份验证方法策略 API 用于管理策略设置。 例如：

* 定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。
* 定义允许用户或用户组使用 FIDO2 安全密钥或无密码电话登录 Azure AD。
* 定义应提醒其使用推送通知设置 MFA Microsoft Authenticator用户或用户组。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法策略       | 说明 |
|:---------------------------|:------------|
|[smsAuthenticationMethodConfiguration](smsAuthenticationMethodConfiguration.md)| 定义可以在 Azure AD 租户上使用短信的用户。|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制以及可以使用它们登录到 Azure AD 的用户。|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|定义可以在 Azure AD Microsoft Authenticator使用租户的用户。|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|定义可以在 Azure AD 租户上使用电子邮件 OTP 的用户。|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration (](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 弃) |定义可以使用无密码登录电话登录 Azure AD 的用户。|
|[temporaryaccesspassauthenticationmethodconfiguration](temporaryaccesspassauthenticationmethodconfiguration.md)|定义可以使用临时访问通道登录 Azure AD 的用户。|

## <a name="policies-available-to-push-users-to-set-up-authentication-methods"></a>可用于推送用户设置身份验证方法的策略：
|策略       | 说明 |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| 定义应提醒其设置身份验证方法的用户 (仅支持Microsoft Authenticator) 。|

## <a name="next-steps"></a>后续步骤

* 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。
