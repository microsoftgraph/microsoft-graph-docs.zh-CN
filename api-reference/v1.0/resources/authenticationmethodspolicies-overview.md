---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义哪些身份验证方法可由 Azure AD 中的用户使用。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: cd3e67f249a4afabc946aaa09c1c4e7448ad99f7
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971075"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD 身份验证方法策略 API 概述

命名空间：microsoft.graph

身份验证方法策略定义 [身份验证方法](/azure/active-directory/authentication/concept-authentication-methods) 以及允许用户在 Azure Active Directory (Azure AD) 中登录和执行多重身份验证 (MFA) 。 可在 Microsoft Graph 中管理的身份验证方法策略包括 FIDO2 安全密钥和 Microsoft Authenticator 应用的无密码电话登录。

身份验证方法策略 API 用于管理策略设置。 例如：

* 定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。
* 定义允许使用 FIDO2 安全密钥或无密码电话登录到 Azure AD 的用户或用户组。
* 定义用户或用户组，这些用户应被提醒使用推送通知设置适用于 MFA 的 Microsoft Authenticator。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>可在 Microsoft Graph 中管理哪些身份验证方法策略？

|身份验证方法策略       | 说明 |
|:---------------------------|:------------|:------------|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|定义可在 Azure AD 租户上使用电子邮件 OTP 的用户。|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制以及可以使用它们登录到 Azure AD 的用户。|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|定义可在 Azure AD 租户上使用 Microsoft Authenticator 的用户。|
|[temporaryAccessPassAuthenticationMethod](temporaryaccesspassauthenticationmethodconfiguration.md)|定义配置设置以及启用了使用临时访问传递身份验证方法的用户或组。|

## <a name="policies-available-for-authentication-methods-registration-campaign"></a>可用于身份验证方法注册活动的策略：
|Policy       | 说明 |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| 定义应提醒其设置身份验证方法的用户 (当前仅支持 Microsoft Authenticator) 。|

## <a name="next-steps"></a>后续步骤

* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。
