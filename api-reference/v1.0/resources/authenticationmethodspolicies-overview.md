---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 25aea5d4492df1961e5ab3f0f869b334baf0db3e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469113"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD 身份验证方法策略 API 概述

命名空间：microsoft.graph

身份验证 [方法策略定义](/azure/active-directory/authentication/concept-authentication-methods) 身份验证方法以及允许其登录并执行 Azure Active Directory () Azure AD (中的多重身份验证) 的用户。 可以在 Microsoft Graph 中管理的身份验证方法策略包括 FIDO2 安全密钥和 Microsoft Authenticator 应用的无密码电话登录。

身份验证方法策略 API 用于管理策略设置。 例如：

* 定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。
* 定义允许使用 FIDO2 安全密钥或无密码电话登录登录 Azure AD 的用户或用户组。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>可以在 Microsoft Graph 中管理哪些身份验证方法策略？

|身份验证方法策略       | 说明 |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制以及可以使用它们登录到 Azure AD 的用户。|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|定义可以在 Azure AD 租户上使用 Microsoft Authenticator 的用户。|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|定义可以在 Azure AD 租户上使用电子邮件 OTP 的用户。|

## <a name="next-steps"></a>后续步骤

* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。
