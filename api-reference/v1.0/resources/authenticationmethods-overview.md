---
title: Azure AD 身份验证方法 API 概述
description: 身份验证方法是用户在 Azure AD 中进行身份验证的方式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: b258d9985f1adf60c74e5de26bdbe7c17380ffd139cd681689a9c9f82a3f4393
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218819"
---
# <a name="azure-ad-authentication-methods-api-overview"></a>Azure AD 身份验证方法 API 概述

命名空间：microsoft.graph

[身份验证](/azure/active-directory/authentication/concept-authentication-methods)方法是用户在 AD Azure Active Directory (中) 。 Azure AD 中的身份验证方法包括密码和电话 (例如，短信和语音呼叫) ，这些呼叫现在在 Microsoft Graph beta 终结点中可管理，此外，还包括 FIDO2 安全密钥和 Microsoft Authenticator 应用等。 身份验证方法用于主要、双重因素和分步身份验证，此外还适用于自助式密码重置 (SSPR) 流程。

身份验证方法 API 用于管理用户的身份验证方法。 例如：

* 可以检索用户的 FIDO2 安全密钥的详细信息，如果用户丢失了该密钥，则将其删除。
* 可以检索用户注册Microsoft Authenticator的详细信息，如果用户丢失了电话，可将其删除。

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a>Microsoft Graph 中可以管理哪些身份验证Graph？

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|[fido2AuthenticationMethod](fido2authenticationmethod.md)|FIDO2 安全密钥可用于登录 Azure AD。|删除丢失的 FIDO2 安全密钥。|
|[microsoftAuthenticatorAuthenticationMethod](microsoftauthenticatorauthenticationmethod.md)|Microsoft Authenticator Azure AD 的登录或执行多重身份验证时，用户可以使用密码|删除Microsoft Authenticator身份验证方法。|
|[windowsHelloForBusinessAuthenticationMethod](windowsHelloForBusinessAuthenticationMethod.md)|Windows Hello For Business 是设备上无密码Windows方法。|请参阅用户已启用适用于Windows Hello登录的设备。 删除Windows Hello企业凭据。|

Microsoft Graph v1.0 中尚不支持以下身份验证方法。

|身份验证方法       | 说明 |示例     |
|:---------------------------|:------------|:------------|
|密码 | 密码当前是 Azure AD 中默认的主身份验证方法。|重置用户密码。|
|phoneAuthenticationMethod (尚不支持)  |用户可以使用电话通过短信或语音呼叫进行身份验证， ([](/azure/active-directory/authentication/concept-authentication-methods#phone-options)策略策略允许) 。|查看用户的身份验证电话号码。 向用户添加、更新或删除电话号码。 启用或禁用用于短信登录的主移动电话。|
|电子邮件 |电子邮件地址可以是用户作为 SSPR 密码重置过程Self-Service密码重置 (用户) 过程。|请参阅用户的身份验证电子邮件地址。 向用户添加、更新或删除电子邮件地址。|
|临时访问传递 |临时访问传递是一种有时间限制的密码，用作强凭据并允许载入无密码凭据。 | 为用户设置新的临时访问传递。|
|硬件令牌 | 允许用户使用提供一次代码的物理设备执行多重身份验证。 | 获取分配给用户的硬件令牌。|
|软件令牌 | 允许用户使用满足一系列函数的一次代码的应用程序执行多重身份验证。 | 获取并删除分配给用户的软件令牌。|
|安全问题和解答 | 允许用户在执行自助服务密码重置时验证其身份。 |删除用户注册的安全问题。|
|默认方法 | 表示用户已选择作为执行多重身份验证的默认方法。| 更改用户的默认 MFA 方法。|

## <a name="next-steps"></a>后续步骤

* 查看身份验证方法类型及其各种方法。
* 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。
