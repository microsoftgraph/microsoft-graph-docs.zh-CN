---
title: Azure AD身份验证方法策略 API 概述
description: 身份验证方法策略定义哪些身份验证方法可用于 Azure AD。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: e01a054de05f4a553775364aa2f7e8cf36ba19d5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015809"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD身份验证方法策略 API 概述

命名空间：microsoft.graph

身份验证方法策略定义[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法以及允许使用它们登录并执行多重身份验证的用户 (MFA) 中Azure Active Directory (Azure AD) 。 可以在 Microsoft 应用商店中管理的身份验证方法策略Graph FIDO2 安全密钥和无密码电话使用 Microsoft Authenticator登录。

身份验证方法策略 API 用于管理策略设置。 例如：

* 定义可在租户租户中使用的 FIDO2 安全Azure AD类型。
* 定义允许用户或用户组使用 FIDO2 安全密钥或无密码电话登录以登录Azure AD。
* 定义应提醒其使用推送通知设置 MFA Microsoft Authenticator用户或用户组。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法策略       | 说明 |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制以及可以使用它们登录安全密钥Azure AD。|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|定义可以在租户Microsoft Authenticator使用Azure AD的用户。|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|定义可以在租户上使用电子邮件 OTP Azure AD用户。|

## <a name="policies-available-for-authentication-methods-registration-campaign"></a>可用于身份验证方法注册活动的策略：
|Policy       | 说明 |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| 定义应提醒其设置身份验证方法的用户 (当前仅受 Microsoft Authenticator) 。|

## <a name="next-steps"></a>后续步骤

* 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
