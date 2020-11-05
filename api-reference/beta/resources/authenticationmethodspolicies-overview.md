---
title: Azure AD 身份验证方法策略 API 概述
description: 身份验证方法策略定义了 Azure AD 中的用户可以使用哪些身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 730368b4e47c34353882e5e601644133dbb38225
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921569"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Azure AD 身份验证方法策略 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

身份验证方法策略定义 [身份验证方法](/azure/active-directory/authentication/concept-authentication-methods) 以及允许使用它们登录并在 Azure Active Directory (azure AD) 中执行多重身份验证 (MFA) 的用户。 可以在 Microsoft Graph 中管理的身份验证方法策略包括 FIDO2 Security Keys and Passwordless Phone 登录与 Microsoft 鉴别应用程序。

身份验证方法策略 Api 用于管理策略设置。 例如：

* 定义可在 Azure AD 租户中使用的 FIDO2 安全密钥的类型。
* 定义允许使用 FIDO2 Security Keys 或 Passwordless Phone 登录以登录到 Azure AD 的用户或用户组。

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>可以在 Microsoft Graph 中管理哪些身份验证方法策略？

|身份验证方法策略       | 说明 |
|:---------------------------|:------------|:------------|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| 定义 FIDO2 安全密钥限制和可使用这些限制登录到 Azure AD 的用户。|
|[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|定义可使用 Passwordless Phone 登录登录 Azure AD 的用户。|

## <a name="next-steps"></a>后续步骤

* 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中使用 API。
